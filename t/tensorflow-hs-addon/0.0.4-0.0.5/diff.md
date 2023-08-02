# Comparing `tmp/tensorflow_hs_addon-0.0.4-cp36-cp36m-macosx_10_15_x86_64.whl.zip` & `tmp/tensorflow_hs_addon-0.0.5-cp37-cp37m-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 78074 bytes, number of entries: 10
--rw-r--r--  2.0 unx      165 b- defN 21-Dec-02 05:20 tensorflow_hs_addon/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Dec-02 05:20 tensorflow_hs_addon/python/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Dec-02 05:20 tensorflow_hs_addon/python/ops/__init__.py
--rwxr-xr-x  2.0 unx   240080 b- defN 21-Dec-02 05:27 tensorflow_hs_addon/python/ops/_reco_ops.so
--rw-r--r--  2.0 unx     1205 b- defN 21-Dec-02 05:20 tensorflow_hs_addon/python/ops/reco_ops.py
--rw-r--r--  2.0 unx    11357 b- defN 21-Dec-02 05:28 tensorflow_hs_addon-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx      998 b- defN 21-Dec-02 05:28 tensorflow_hs_addon-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx      111 b- defN 21-Dec-02 05:28 tensorflow_hs_addon-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 21-Dec-02 05:28 tensorflow_hs_addon-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      923 b- defN 21-Dec-02 05:28 tensorflow_hs_addon-0.0.4.dist-info/RECORD
-10 files, 254859 bytes uncompressed, 76462 bytes compressed:  70.0%
+Zip file size: 172875 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      216 b- defN 23-Apr-19 10:19 tensorflow_hs_addon/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-18 09:48 tensorflow_hs_addon/python/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-18 09:48 tensorflow_hs_addon/python/ops/__init__.py
+-rwxr-xr-x  2.0 unx   454424 b- defN 23-Apr-20 07:01 tensorflow_hs_addon/python/ops/_reco_ops.so
+-rw-r--r--  2.0 unx     1320 b- defN 23-Apr-18 10:29 tensorflow_hs_addon/python/ops/reco_ops.py
+-rw-r--r--  2.0 unx     6951 b- defN 23-Apr-19 10:51 tensorflow_hs_addon/python/ops/test.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-26 05:54 tensorflow_hs_addon-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx      952 b- defN 23-Jul-26 05:54 tensorflow_hs_addon-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      104 b- defN 23-Jul-26 05:54 tensorflow_hs_addon-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Jul-26 05:54 tensorflow_hs_addon-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1018 b- defN 23-Jul-26 05:54 tensorflow_hs_addon-0.0.5.dist-info/RECORD
+11 files, 476362 bytes uncompressed, 171111 bytes compressed:  64.1%
```

## zipnote {}

```diff
@@ -9,23 +9,26 @@
 
 Filename: tensorflow_hs_addon/python/ops/_reco_ops.so
 Comment: 
 
 Filename: tensorflow_hs_addon/python/ops/reco_ops.py
 Comment: 
 
-Filename: tensorflow_hs_addon-0.0.4.dist-info/LICENSE
+Filename: tensorflow_hs_addon/python/ops/test.py
 Comment: 
 
-Filename: tensorflow_hs_addon-0.0.4.dist-info/METADATA
+Filename: tensorflow_hs_addon-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: tensorflow_hs_addon-0.0.4.dist-info/WHEEL
+Filename: tensorflow_hs_addon-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: tensorflow_hs_addon-0.0.4.dist-info/top_level.txt
+Filename: tensorflow_hs_addon-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: tensorflow_hs_addon-0.0.4.dist-info/RECORD
+Filename: tensorflow_hs_addon-0.0.5.dist-info/top_level.txt
+Comment: 
+
+Filename: tensorflow_hs_addon-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tensorflow_hs_addon/__init__.py

```diff
@@ -1,5 +1,7 @@
 from tensorflow_hs_addon.python.ops.reco_ops import (
-    group_by_slots, split_ragged_block,
     pooling_by_slots, pooling_by_slots_grad,
-    get_slot_fids, isin
+    get_slot_fids, isin,
+    feature_vec_to_segments,
+    unsorted_feature_vec_to_segments,
+    parse_feature_vec,
 )
```

## tensorflow_hs_addon/python/ops/_reco_ops.so

### strings -a -n 8 {}

```diff
@@ -1,1327 +1,1148 @@
-__stub_helper
-__gcc_except_tab__TEXT
-__cstring
-__unwind_info
-__DATA_CONST
-__DATA_CONST
-__mod_init_func
-__DATA_CONST
-__DATA_CONST
-__la_symbol_ptr
-__LINKEDIT
-tensorflow_hs_addon/python/ops/_reco_ops.so
-@rpath/libtensorflow_framework.2.dylib
-/usr/lib/libc++.1.dylib
-/usr/lib/libSystem.B.dylib
-AWAVAUATSH
-[A\A]A^A_]
-AWAVATSH
-[A\A^A_]
-AWAVATSH
-[A\A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-([A\A]A^A_]
-([A\A]A^A_]
-AWAVAUATSH
-([A\A]A^A_]
-AWAVAUATSH
-8[A\A]A^A_]
-AWAVAUATSPI
-[A\A]A^A_]
-AWAVATSI
-u	[A\A^A_]
-[A\A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSPH
-[A\A]A^A_]
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVATSH
-[A\A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVATSH
-0[A\A^A_]
-AWAVATSH
-0[A\A^A_]
-AWAVATSH
-[A\A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-x[A\A]A^A_]
-AWAVAUATSH
-([A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-[A\A]A^A_]
-AWAVAUATSH
-H;\$0|LL+T$HI)
-L;d$0|%I)
-L;l$0|&I)
-H;t$0|JI)
-[A\A]A^A_]
-AWAVATSH
-[A\A^A_]
-AWAVAUATSH
-T$xL;W uJL
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVATSH
-[A\A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSPM
-[A\A]A^A_]
-AWAVAUATSH
-H;D$HugD9y
-H;D$Hu%D9y
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-[A\A]A^A_]
-AWAVAUATSH
-8[A\A]A^A_]
-AWAVATSH
-values: L
-pad_valuH
-alues: TH
-block_vaH
-slots: iL
-fids: inH
- float32L
-grads: fH
-slot: inH
-filter: H
-mask: boH
-[A\A^A_]
-AWAVATSI
-[A\A^A_]
-AWAVATSI
-[A\A^A_]
-AWAVATSI
-[A\A^A_]
-AWAVATSI
-[A\A^A_]
-AWAVATSI
-[A\A^A_]
-?16PoolingBySlotsOp
-NSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEEE
-NSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEEE
-NSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-NSt3__110__function6__baseIFvxxEEE
-ZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-20PoolingBySlotsGradOp
-13GetSlotFidsOp
-NSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-ZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-14GroupBySlotsOp
-NSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-ZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-_6IsInOpIiE
-6IsInOpIxE
-18SplitRaggedBlockOpIfE
-NSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-ZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-18SplitRaggedBlockOpIiE
-NSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-ZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-18SplitRaggedBlockOpIxE
-NSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-ZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-NSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-NSt3__110__function6__baseIFN10tensorflow6StatusEPNS2_15shape_inference16InferenceContextEEEE
-NSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-NSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-NSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-NSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-NSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
+__gmon_start__
+_ITM_deregisterTMCloneTable
+_ITM_registerTMCloneTable
+__cxa_finalize
+_ZN10tensorflow8OpKernel7AsAsyncEv
+_ZN10tensorflow8OpKernel11IsExpensiveEv
+_ZNK10tensorflow8OpKernel12const_tensorEv
+_ZN16PoolingBySlotsOpD2Ev
+_ZTV16PoolingBySlotsOp
+_ZN10tensorflow8OpKernelD2Ev
+_ZN16PoolingBySlotsOpD1Ev
+_ZN16PoolingBySlotsOpD0Ev
+_ZN20PoolingBySlotsGradOpD2Ev
+_ZTV20PoolingBySlotsGradOp
+_ZN20PoolingBySlotsGradOpD1Ev
+_ZN20PoolingBySlotsGradOpD0Ev
+_ZNSs4_Rep10_M_destroyERKSaIcE
+_ZN10tensorflow8OpKernelC2EPNS_20OpKernelConstructionE
+_Unwind_Resume
+__gxx_personality_v0
+_ZNSt14_Function_base13_Base_managerIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation
+_ZTIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_
+__assert_fail
+_ZGVZN5Eigen8internal20manage_caching_sizesENS_6ActionEPlS2_S2_E12m_cacheSizes
+_ZZN5Eigen8internal20manage_caching_sizesENS_6ActionEPlS2_S2_E12m_cacheSizes
+__cxa_guard_acquire
+__cxa_guard_release
+__stack_chk_fail
+_ZN5Eigen8internal19throw_std_bad_allocEv
+__cxa_allocate_exception
+_ZTVSt9bad_alloc
+_ZTISt9bad_alloc
+_ZNSt9bad_allocD1Ev
+__cxa_throw
+_ZN5Eigen8internal21queryCacheSizes_intelERiS1_S1_i
+_ZZN4absl14lts_2020_09_2311string_view19CheckLengthInternalEmENKUlvE_clEv
+_ZZN4absl14lts_2020_09_2311string_view19CheckLengthInternalEmENUlvE_4_FUNEv
+_ZN10tensorflow14kernel_factory17OpKernelRegistrarC2EPKNS_9KernelDefEN4absl14lts_2020_09_2311string_viewEPFPNS_8OpKernelEPNS_20OpKernelConstructionEE
+_ZTVN10tensorflow14kernel_factory17OpKernelRegistrar18PtrOpKernelFactoryE
+_ZN10tensorflow14kernel_factory17OpKernelRegistrar12InitInternalEPKNS_9KernelDefEN4absl14lts_2020_09_2311string_viewESt10unique_ptrINS0_15OpKernelFactoryESt14default_deleteIS9_EE
+_ZN10tensorflow14kernel_factory17OpKernelRegistrarC1EPKNS_9KernelDefEN4absl14lts_2020_09_2311string_viewEPFPNS_8OpKernelEPNS_20OpKernelConstructionEE
+_ZNSt10unique_ptrIN10tensorflow6Status5StateESt14default_deleteIS2_EED2Ev
+_ZNSs4_Rep20_S_empty_rep_storageE
+_ZNSt10unique_ptrIN10tensorflow6Status5StateESt14default_deleteIS2_EED1Ev
+_ZNSt6vectorIN10tensorflow10StackFrameESaIS1_EED2Ev
+_ZNSt6vectorIN10tensorflow10StackFrameESaIS1_EED1Ev
+_ZZNK4absl14lts_2020_09_234SpanIKlEixEmENKUlvE_clEv
+_ZZNK4absl14lts_2020_09_234SpanIKlEixEmENUlvE_4_FUNEv
+_ZN10tensorflow6errors15InvalidArgumentIJPKcEEENS_6StatusEDpT_
+_ZNSt8ios_baseC2Ev
+_ZTTSt18basic_stringstreamIcSt11char_traitsIcESaIcEE
+_ZTVSt9basic_iosIcSt11char_traitsIcEE
+_ZNSt9basic_iosIcSt11char_traitsIcEE4initEPSt15basic_streambufIcS1_E
+_ZTVSt15basic_streambufIcSt11char_traitsIcEE
+_ZTVSt18basic_stringstreamIcSt11char_traitsIcESaIcEE
+_ZNSt6localeC1Ev
+_ZTVSt15basic_stringbufIcSt11char_traitsIcESaIcEE
+_ZSt16__ostream_insertIcSt11char_traitsIcEERSt13basic_ostreamIT_T0_ES6_PKS3_l
+_ZNSs4_Rep9_S_createEmmRKSaIcE
+_ZNSs4swapERSs
+_ZNSt6localeD1Ev
+_ZNSt8ios_baseD2Ev
+_ZN10tensorflow7strings6StrCatERKNS0_8AlphaNumE
+_ZN10tensorflow6StatusC1ENS_5error4CodeEN4absl14lts_2020_09_2311string_viewEOSt6vectorINS_10StackFrameESaIS7_EE
+_ZNSt9basic_iosIcSt11char_traitsIcEE5clearESt12_Ios_Iostate
+_ZNSs6assignERKSs
+_ZSt19__throw_logic_errorPKc
+_ZNSt18basic_stringstreamIcSt11char_traitsIcESaIcEED1Ev
+_ZN10tensorflow8internal17MakeCheckOpStringImmEEPSsRKT_RKT0_PKc
+_ZN10tensorflow8internal21CheckOpMessageBuilderC1EPKc
+_ZNSo9_M_insertImEERSoT_
+_ZN10tensorflow8internal21CheckOpMessageBuilder7ForVar2Ev
+_ZN10tensorflow8internal21CheckOpMessageBuilder9NewStringEv
+_ZN10tensorflow8internal21CheckOpMessageBuilderD1Ev
+_ZN10tensorflow8internal17MakeCheckOpStringIliEEPSsRKT_RKT0_PKc
+_ZNSo9_M_insertIlEERSoT_
+_ZNSolsEi
+_ZN10tensorflow8internal17MakeCheckOpStringIllEEPSsRKT_RKT0_PKc
+_ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEED2Ev
+_ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEED1Ev
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERS8_RKS9_
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERSA_RKSB_
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERS8_RKS9_
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERS9_RKSA_
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC1ERS9_RKSA_
+_ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS3_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKSA_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSI_EEEEKNS3_ILln1EKNS4_INS5_ISI_Li2ELi1ElEELi16ES7_EEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE0EE3runERSV_RKSW_
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERSA_RKSB_
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERSC_RKSD_
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC1ERSC_RKSD_
+_ZN5Eigen8internal13TensorBlockIOIflLi2ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi2EEE
+_ZNSt6vectorIN5Eigen8internal27TensorBlockScratchAllocatorINS0_13DefaultDeviceEE10AllocationESaIS5_EE17_M_realloc_insertIJRKS5_EEEvN9__gnu_cxx17__normal_iteratorIPS5_S7_EEDpOT_
+_ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEE8allocateEm
+_ZN5Eigen8internal13TensorBlockIOIflLi3ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi3EEE
+_ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKS9_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSH_EEEEKNS3_ILln1EKNS3_ILln1EKNS4_INS5_ISH_Li3ELi1ElEELi16ES7_EEEEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE1EE3runERSW_RKSX_
+_ZNSt8ios_base4InitC1Ev
+_ZNSt8ios_base4InitD1Ev
+__cxa_atexit
+_ZN10tensorflow16KernelDefBuilderC2EPKc
+_ZN10tensorflow10DEVICE_CPUE
+_ZN10tensorflow16KernelDefBuilder6DeviceEPKc
+_ZN10tensorflow16KernelDefBuilder5BuildEv
+_ZN10tensorflow16KernelDefBuilderD2Ev
+_ZN10tensorflow4core10RefCountedD2Ev
+_ZTVN10tensorflow4core10RefCountedE
+_ZN10tensorflow8internal15LogMessageFatalC1EPKci
+_ZN10tensorflow8internal15LogMessageFatalD1Ev
+_ZN10tensorflow4core10RefCountedD1Ev
+_ZN10tensorflow4core10RefCountedD0Ev
+_ZNK10tensorflow10DeviceBase29tensorflow_cpu_worker_threadsEv
+_ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm2EEEvN4absl14lts_2020_09_234SpanIKlEEPSt5arrayIlXT_EE
+_ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm1EEEvN4absl14lts_2020_09_234SpanIKlEEPSt5arrayIlXT_EE
+_ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm3EEEvN4absl14lts_2020_09_234SpanIKlEEPSt5arrayIlXT_EE
+_ZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextE
+_ZNK10tensorflow15OpKernelContext5inputEi
+_ZNK10tensorflow11TensorShape10IsSameSizeERKS0_
+_ZNK10tensorflow15TensorShapeBaseINS_11TensorShapeEE8dim_sizeEi
+_ZN10tensorflow15TensorShapeBaseINS_11TensorShapeEEC1EN4absl14lts_2020_09_234SpanIKlEE
+_ZN10tensorflow15OpKernelContext15allocate_outputEiRKNS_11TensorShapeEPPNS_6TensorE
+_ZNK10tensorflow6Tensor9CheckTypeENS_8DataTypeE
+_ZNK10tensorflow6Tensor21CheckTypeAndIsAlignedENS_8DataTypeE
+_ZNSt17_Function_handlerIFvllEZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_E9_M_invokeERKSt9_Any_dataOlSA_
+_ZN10tensorflow6thread10ThreadPool11ParallelForEllRKSt8functionIFvllEE
+_ZGVZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZN10tensorflow8internal10LogMessageC1EPKcii
+_ZN10tensorflow8internal10LogMessageD1Ev
+_ZN10tensorflow14TensorShapeRep19DestructorOutOfLineEv
+_ZN10tensorflow22CheckNotInComputeAsyncEPNS_15OpKernelContextEPKc
+_ZN10tensorflow15OpKernelContext10CtxFailureEPKciRKNS_6StatusE
+_ZN10tensorflow15OpKernelContext21CtxFailureWithWarningEPKciRKNS_6StatusE
+_ZN10tensorflow8internal10LogMessage16VmoduleActivatedEPKci
+__cxa_guard_abort
+_ZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE0_clEll
+_ZGVZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE0_clEllENKUliPKcE_clEiS5_E17vmodule_activated
+_ZZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE0_clEllENKUliPKcE_clEiS5_E17vmodule_activated
+_ZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextE
+_ZGVZZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZZZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZTSN10tensorflow4core10RefCountedE
+_ZTIN10tensorflow4core10RefCountedE
+_ZTVN10__cxxabiv117__class_type_infoE
+_ZTS16PoolingBySlotsOp
+_ZTI16PoolingBySlotsOp
+_ZTVN10__cxxabiv120__si_class_type_infoE
+_ZTIN10tensorflow8OpKernelE
+_ZTS20PoolingBySlotsGradOp
+_ZTI20PoolingBySlotsGradOp
+_ZTSZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_
+_ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb
+__pthread_key_create
+_ZNSt17_Function_handlerIFvllEZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_E9_M_invokeERKSt9_Any_dataOlSA_
+_ZN13GetSlotFidsOpD2Ev
+_ZTV13GetSlotFidsOp
+_ZN13GetSlotFidsOpD1Ev
+_ZN13GetSlotFidsOpD0Ev
+_ZNSt14_Function_base13_Base_managerIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation
+_ZTIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_
+_ZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextE
+_ZNK10tensorflow6Tensor30CheckIsAlignedAndSingleElementEv
+_ZTS13GetSlotFidsOp
+_ZTI13GetSlotFidsOp
+_ZTSZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_
+_ZN18SplitRaggedBlockOpIfED2Ev
+_ZTV18SplitRaggedBlockOpIfE
+_ZN18SplitRaggedBlockOpIfED1Ev
+_ZN18SplitRaggedBlockOpIfED0Ev
+_ZN18SplitRaggedBlockOpIiED2Ev
+_ZTV18SplitRaggedBlockOpIiE
+_ZN18SplitRaggedBlockOpIiED1Ev
+_ZN18SplitRaggedBlockOpIiED0Ev
+_ZN18SplitRaggedBlockOpIlED2Ev
+_ZTV18SplitRaggedBlockOpIlE
+_ZN18SplitRaggedBlockOpIlED1Ev
+_ZN18SplitRaggedBlockOpIlED0Ev
+_ZNSt14_Function_base13_Base_managerIZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E10_M_managerERSt9_Any_dataRKS8_St18_Manager_operation
+_ZTIZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_
+_ZNSt14_Function_base13_Base_managerIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E10_M_managerERSt9_Any_dataRKS8_St18_Manager_operation
+_ZTIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_
+_ZNSt14_Function_base13_Base_managerIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E10_M_managerERSt9_Any_dataRKS8_St18_Manager_operation
+_ZTIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_
+_ZN10tensorflow16KernelDefBuilder14TypeConstraintEPKcNS_8DataTypeE
+_ZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextE
+_ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
+_ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
+_ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
+_ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
+_ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
+_ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
+_ZNSt17_Function_handlerIFvllEZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E9_M_invokeERKSt9_Any_dataOlSB_
+_ZNSo9_M_insertIdEERSoT_
+_ZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEll
+_ZGVZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated
+_ZZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated
+_ZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextE
+_ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
+_ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
+_ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
+_ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
+_ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
+_ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
+_ZNSt17_Function_handlerIFvllEZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E9_M_invokeERKSt9_Any_dataOlSB_
+_ZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEll
+_ZGVZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated
+_ZZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated
+_ZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextE
+_ZGVZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
+_ZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
+_ZGVZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
+_ZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
+_ZGVZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
+_ZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
+_ZNSt17_Function_handlerIFvllEZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E9_M_invokeERKSt9_Any_dataOlSB_
+_ZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEll
+_ZGVZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated
+_ZZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated
+_ZTSZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_
+_ZTSZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_
+_ZTSZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_
+_ZTS18SplitRaggedBlockOpIfE
+_ZTI18SplitRaggedBlockOpIfE
+_ZTS18SplitRaggedBlockOpIiE
+_ZTI18SplitRaggedBlockOpIiE
+_ZTS18SplitRaggedBlockOpIlE
+_ZTI18SplitRaggedBlockOpIlE
+_ZN22FeatureVecToSegmentsOpD2Ev
+_ZTV22FeatureVecToSegmentsOp
+_ZN22FeatureVecToSegmentsOpD1Ev
+_ZN22FeatureVecToSegmentsOpD0Ev
+_ZN30UnsortedFeatureVecToSegmentsOpD2Ev
+_ZTV30UnsortedFeatureVecToSegmentsOp
+_ZN30UnsortedFeatureVecToSegmentsOpD1Ev
+_ZN30UnsortedFeatureVecToSegmentsOpD0Ev
+_ZN22FeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextE
+_ZGVZZN22FeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZZZN22FeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZSt17__throw_bad_allocv
+_ZSt20__throw_length_errorPKc
+_ZN30UnsortedFeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextE
+_ZGVZZN30UnsortedFeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZZZN30UnsortedFeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZTS22FeatureVecToSegmentsOp
+_ZTI22FeatureVecToSegmentsOp
+_ZTS30UnsortedFeatureVecToSegmentsOp
+_ZTI30UnsortedFeatureVecToSegmentsOp
+_ZN14GroupBySlotsOpD2Ev
+_ZTV14GroupBySlotsOp
+_ZN14GroupBySlotsOpD1Ev
+_ZN14GroupBySlotsOpD0Ev
+_ZNSt14_Function_base13_Base_managerIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation
+_ZTIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_
+_ZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextE
+_ZGVZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZGVZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS4_E17vmodule_activated
+_ZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS4_E17vmodule_activated
+_ZNSt17_Function_handlerIFvllEZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_E9_M_invokeERKSt9_Any_dataOlSA_
+_ZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEll
+_ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE_clEiS5_E17vmodule_activated
+_ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE_clEiS5_E17vmodule_activated
+_ZGVZZN7FidIter7advanceEvENKUliPKcE_clEiS1_E17vmodule_activated
+_ZZZN7FidIter7advanceEvENKUliPKcE_clEiS1_E17vmodule_activated
+_ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE0_clEiS5_E17vmodule_activated
+_ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE0_clEiS5_E17vmodule_activated
+_ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE1_clEiS5_E17vmodule_activated
+_ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE1_clEiS5_E17vmodule_activated
+_ZTS14GroupBySlotsOp
+_ZTI14GroupBySlotsOp
+_ZTSZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_
+_ZN17ParseFeatureVecOpD2Ev
+_ZTV17ParseFeatureVecOp
+_ZN17ParseFeatureVecOpD1Ev
+_ZN17ParseFeatureVecOpD0Ev
+_ZNSt6vectorIlSaIlEE17_M_realloc_insertIJRKlEEEvN9__gnu_cxx17__normal_iteratorIPlS1_EEDpOT_
+_ZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_EC2ERKSF_m
+_ZNSt12length_errorC1EPKc
+_ZNSt12length_errorD1Ev
+_ZTISt12length_error
+__cxa_free_exception
+_ZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_EC1ERKSF_m
+_ZN17ParseFeatureVecOp7ComputeEPN10tensorflow15OpKernelContextE
+_ZGVZZN17ParseFeatureVecOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZZZN17ParseFeatureVecOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZNK10tensorflow6Tensor4dataEv
+_ZTS17ParseFeatureVecOp
+_ZTI17ParseFeatureVecOp
+_ZN6IsInOpIiED2Ev
+_ZTV6IsInOpIiE
+_ZN6IsInOpIiED1Ev
+_ZN6IsInOpIiED0Ev
+_ZN6IsInOpIlED2Ev
+_ZTV6IsInOpIlE
+_ZN6IsInOpIlED1Ev
+_ZN6IsInOpIlED0Ev
+_ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEED2Ev
+_ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev
+_ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEED2Ev
+_ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev
+_ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE9_M_rehashEmRKm
+__cxa_begin_catch
+__cxa_rethrow
+__cxa_end_catch
+_ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE21_M_insert_unique_nodeEmmPNS1_10_Hash_nodeIlLb0EEE
+_ZNKSt8__detail20_Prime_rehash_policy14_M_need_rehashEmmm
+_ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE9_M_rehashEmRKm
+_ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE21_M_insert_unique_nodeEmmPNS1_10_Hash_nodeIiLb0EEE
+_ZN6IsInOpIiE7ComputeEPN10tensorflow15OpKernelContextE
+_ZNKSt8__detail20_Prime_rehash_policy11_M_next_bktEm
+_ZN6IsInOpIlE7ComputeEPN10tensorflow15OpKernelContextE
+_ZTS6IsInOpIiE
+_ZTI6IsInOpIiE
+_ZTS6IsInOpIlE
+_ZTI6IsInOpIlE
+_ZN10tensorflow15shape_inference16InferenceContext8WithRankENS0_11ShapeHandleElPS2_
+_ZSt24__throw_out_of_range_fmtPKcz
+_ZN10tensorflow11register_op19OpDefBuilderWrapperC2EPKc
+_ZNSsC1EPKcRKSaIcE
+_ZN10tensorflow12OpDefBuilderC1ESs
+_ZN10tensorflow11register_op19OpDefBuilderWrapperC1EPKc
+_ZN10tensorflow11register_op19OpDefBuilderWrapper5InputESs
+_ZN10tensorflow12OpDefBuilder5InputESs
+_ZN10tensorflow11register_op19OpDefBuilderWrapper6OutputESs
+_ZN10tensorflow12OpDefBuilder6OutputESs
+_ZN10tensorflow11register_op19OpDefBuilderWrapper10SetShapeFnESt8functionIFNS_6StatusEPNS_15shape_inference16InferenceContextEEE
+_ZN10tensorflow12OpDefBuilder10SetShapeFnESt8functionIFNS_6StatusEPNS_15shape_inference16InferenceContextEEE
+_ZN10tensorflow8internal17MakeCheckOpStringIiiEEPSsRKT_RKT0_PKc
+_ZNSt6vectorIPN10tensorflow15shape_inference9DimensionESaIS3_EE17_M_realloc_insertIJS3_EEEvN9__gnu_cxx17__normal_iteratorIPS3_S5_EEDpOT_
+_ZN10tensorflow15shape_inference19DimensionOrConstantC2El
+_ZN10tensorflow15shape_inference19DimensionOrConstantC1El
+_ZN10tensorflow15shape_inference9DimensionC2El
+_ZN10tensorflow15shape_inference9DimensionC1El
+_ZN10tensorflow15shape_inference16InferenceContext10ReplaceDimENS0_11ShapeHandleElNS0_15DimensionHandleEPS2_
+_ZN10tensorflow15shape_inference19DimensionOrConstantC2ENS0_15DimensionHandleE
+_ZN10tensorflow15shape_inference19DimensionOrConstantC1ENS0_15DimensionHandleE
+_ZN10tensorflow15shape_inference16InferenceContext9MakeShapeESt16initializer_listINS0_19DimensionOrConstantEE
+_ZN10tensorflow12OpDefBuilderD2Ev
+_ZN10tensorflow5OpDefD1Ev
+_ZN10tensorflow12OpDefBuilderD1Ev
+_ZN10tensorflow11register_op19OpDefBuilderWrapperclEv
+_ZN10tensorflow12OpDefBuilder4AttrESs
+libtensorflow_framework.so.2
+libstdc++.so.6
+libgcc_s.so.1
+libc.so.6
+__bss_start
+GLIBC_2.4
+GLIBC_2.2.5
+GLIBC_2.14
+GLIBCXX_3.4.9
+CXXABI_1.3
+GLIBCXX_3.4
+[]A\A]A^A_
+AVAUATUSH
+ []A\A]A^
+AWAVAUATUSH
+([]A\A]A^A_
+AWAVAUATUSH
+([]A\A]A^A_
+AWAVAUATL
+[_A\A]A^A_]H
+ H;U0~_H
+AWAVAUATL
+[AZA\A]A^A_]I
+ H;U0~_H
+AWAVAUATARSH
+[A[A\A]A^A_]I
+[]A\A]A^A_
+([]A\A]A^A_
+AWAVAUATARSH
+[AXA\A]A^A_]I
+AWAVAUATL
+[_A\A]A^A_]H
+AVAUATUI
+[]A\A]A^
+AVAUATUI
+[]A\A]A^
+AVAUATUI
+[]A\A]A^
+AWAVAUATI
+[_A\A]A^A_]H
+AWAVAUATLc
+[]A\A]A^A_
+AWAVAUATARSH
+[AZA\A]A^A_]
+AVAUATUSH
+[]A\A]A^
+AWAVAUATARSH
+[XA\A]A^A_]H
+AWAVAUATUSH
+[]A\A]A^A_
+AWAVAUATI
+[ZA\A]A^A_]H
+AWAVAUATUSH
+[]A\A]A^A_
+AWAVAUATI
+[AYA\A]A^A_]I
+AWAVAUATUSH
+[]A\A]A^A_
+AWAVAUATI
+[ZA\A]A^A_]H
+AWAVAUATI
+[XA\A]A^A_]H
+AWAVAUATI
+[XA\A]A^A_]H
+AWAVAUATUSH
+[]A\A]A^A_
+|$49|$HI
+LcD$HLct$TL
+T$P+T$(D
+Lcl$ LcD$TL
+t$(D+t$P9D$
+[]A\A]A^A_
+[]A\A]A^A_
+taL;F u[H
+t<L;N u6H
+AWAVAUATARSH
+[ZA\A]A^A_]H
+AWAVAUATUSH
+[]A\A]A^A_
+AWAVAUATUSH
+[]A\A]A^A_
+AWAVAUATI
+|$8dH3<%(
+H[]A\A]A^A_
+|$HdH3<%(
+X[]A\A]A^A_
+AWAVAUATI
+h[]A\A]A^A_
+H[]A\A]A^A_
+AWAVAUATI
+h[]A\A]A^A_
+[]A\A]A^A_
+[]A\A]A^A_
+AWAVAUATUSH
+[]A\A]A^A_
+/usr/local/lib/python3.7/dist-packages/tensorflow/include/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h
+/usr/local/lib/python3.7/dist-packages/tensorflow/include/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h
+m_data_type_size == sizeof(Scalar)
+m_data != __null
 PoolingBySlots
-PoolingBySlotsGrad
 PoolingBySlotsOp
-operator()
-/Users/npbool/Projects/tensorflow-hs-addon/venv-368/lib/python3.6/site-packages/tensorflow/include/absl/strings/string_view.h
+PoolingBySlotsGrad
+PoolingBySlotsGradOp
+/usr/local/lib/python3.7/dist-packages/tensorflow/include/absl/strings/string_view.h
 false && "len <= kMaxSize"
-OP_REQUIRES_ASYNC
-tensorflow_hs_addon/cc/kernels/feature_pooling.cc
-fid and weights should have the same shape
-fid and slots should have the same shape
-OP_REQUIRES_OK_ASYNC
-Invalid requested slot id: 
-allocator<T>::allocate(size_t n) 'n' exceeds maximum supported size
-/Users/npbool/Projects/tensorflow-hs-addon/venv-368/lib/python3.6/site-packages/tensorflow/include/tensorflow/core/framework/tensor.h
-Check failed: IsAligned() 
-NDIMS == new_sizes.size()
-new_num_elements == NumElements()
-/Users/npbool/Projects/tensorflow-hs-addon/venv-368/lib/python3.6/site-packages/tensorflow/include/absl/types/span.h
+/usr/local/lib/python3.7/dist-packages/tensorflow/include/absl/types/span.h
 false && "i < size()"
-evalSubExprsIfNeeded
-/Users/npbool/Projects/tensorflow-hs-addon/venv-368/lib/python3.6/site-packages/tensorflow/include/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h
-dimensions_match(m_leftImpl.dimensions(), m_rightImpl.dimensions())
-coeffRef
-/Users/npbool/Projects/tensorflow-hs-addon/venv-368/lib/python3.6/site-packages/tensorflow/include/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h
-m_data != __null
-Invalid feature slot id: 
-DimensionId
-/Users/npbool/Projects/tensorflow-hs-addon/venv-368/lib/python3.6/site-packages/tensorflow/include/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h
-dim >= 0
-TensorEvaluator
+basic_string::_S_construct null not valid
+/usr/local/lib/python3.7/dist-packages/tensorflow/include/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h
 NumInputDims > m_dim.actualDim()
 op.offset() < input_dims[m_dim.actualDim()]
-writePacket
+dim >= 0
+dimensions_match(m_leftImpl.dimensions(), m_rightImpl.dimensions())
+/usr/local/lib/python3.7/dist-packages/tensorflow/include/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h
+index+PacketSize-1 < dimensions().TotalSize()
 this->m_stride == 1
 this->m_stride > index
-srcCoeff
-m_stride == 1
-m_stride > index
-index+PacketSize-1 < dimensions().TotalSize()
-PoolingBySlotsGradOp
-invalid grad shape
-InitializeBlockDimensions
-/Users/npbool/Projects/tensorflow-hs-addon/venv-368/lib/python3.6/site-packages/tensorflow/include/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h
-coeff_to_allocate == 1
-m_block_dimensions.TotalSize() >= numext::mini<IndexType>(target_block_size, m_tensor_dimensions.TotalSize())
-AddDestinationBuffer
-dst_base != __null
-m_data_type_size == sizeof(Scalar)
-m_data != NULL
-TensorMaterializedBlock
-m_kind == internal::TensorBlockKind::kView || m_kind == internal::TensorBlockKind::kMaterializedInScratch || m_kind == internal::TensorBlockKind::kMaterializedInOutput
-allocate
+dst.strides[inner_dim] == 1 || dst.strides[inner_dim] == 0
+src.strides[inner_dim] == 1 || src.strides[inner_dim] == 0
 m_allocation_index <= num_allocations
 m_allocations[m_allocation_index].ptr != __null
 m_allocations[m_allocation_index].size >= size
-dst.strides[inner_dim] == 1 || dst.strides[inner_dim] == 0
-src.strides[inner_dim] == 1 || src.strides[inner_dim] == 0
-dimensions_match(target.dims, eval.dimensions())
-target.strides[inner_dim_idx] == 1
-m_valid_expr
-writeBlock
+coeff_to_allocate == 1
+m_data != NULL
 this->m_impl.data() != NULL
-/Users/npbool/Projects/tensorflow-hs-addon/venv-368/lib/python3.6/site-packages/tensorflow/include/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h
+m_block_dimensions.TotalSize() >= numext::mini<IndexType>(target_block_size, m_tensor_dimensions.TotalSize())
+dimensions_match(target.dims, eval.dimensions())
+/usr/local/lib/python3.7/dist-packages/tensorflow/include/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h
 internal::array_prod(m_impl.dimensions()) == internal::array_prod(op.dimensions())
-GetSlotFids
+ref_.load() == 0
+/usr/local/lib/python3.7/dist-packages/tensorflow/include/tensorflow/core/platform/refcount.h
+/usr/local/lib/python3.7/dist-packages/tensorflow/include/tensorflow/core/framework/device_base.h
+Check failed: cpu_worker_threads_ != nullptr 
+NDIMS == new_sizes.size()
+/usr/local/lib/python3.7/dist-packages/tensorflow/include/tensorflow/core/framework/tensor.h
+new_num_elements == NumElements()
+OP_REQUIRES_ASYNC
+OP_REQUIRES_OK_ASYNC
+Check failed: IsAligned() 
+Invalid requested slot id: 
+fid and weights should have the same shape
+tensorflow_hs_addon/cc/kernels/feature_pooling.cc
+fid and slots should have the same shape
+Invalid feature slot id: 
+invalid grad shape
+Eigen::TensorEvaluator<const Derived, Device>::CoeffReturnType Eigen::TensorEvaluator<const Derived, Device>::coeff(Eigen::TensorEvaluator<const Derived, Device>::Index) const [with Derived = Eigen::TensorMap<const Eigen::Tensor<float, 1, 1, long int>, 0, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Derived, Device>::CoeffReturnType = float; Eigen::TensorEvaluator<const Derived, Device>::Index = long int]
+Eigen::TensorEvaluator<const Eigen::TensorReshapingOp<NewDimensions, XprType>, Device>::TensorEvaluator(const XprType&, const Device&) [with NewDimensions = const Eigen::DSizes<long int, 2>; ArgType = const Eigen::TensorCwiseBinaryOp<Eigen::internal::scalar_sum_op<float, float>, const Eigen::TensorMap<const Eigen::Tensor<float, 1, 1, long int>, 0, Eigen::MakePointer>, const Eigen::TensorCwiseUnaryOp<Eigen::internal::bind1st_op<Eigen::internal::scalar_product_op<const float, const float> >, const Eigen::TensorMap<const Eigen::Tensor<float, 1, 1, long int>, 0, Eigen::MakePointer> > >; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Eigen::TensorReshapingOp<NewDimensions, XprType>, Device>::XprType = Eigen::TensorReshapingOp<const Eigen::DSizes<long int, 2>, const Eigen::TensorCwiseBinaryOp<Eigen::internal::scalar_sum_op<float, float>, const Eigen::TensorMap<const Eigen::Tensor<float, 1, 1, long int>, 0, Eigen::MakePointer>, const Eigen::TensorCwiseUnaryOp<Eigen::internal::bind1st_op<Eigen::internal::scalar_product_op<const float, const float> >, const Eigen::TensorMap<const Eigen::Tensor<float, 1, 1, long int>, 0, Eigen::MakePointer> > > >]
+void Eigen::TensorEvaluator<Eigen::TensorChippingOp<DimId, XprType>, Device>::writeBlock(const TensorBlockDesc&, const TensorBlock&) [with TensorBlock = Eigen::internal::TensorCwiseBinaryBlock<Eigen::internal::scalar_sum_op<float, float>, Eigen::internal::TensorMaterializedBlock<float, 1, 1, long int>, Eigen::internal::TensorCwiseUnaryBlock<Eigen::internal::bind1st_op<Eigen::internal::scalar_product_op<const float, const float> >, Eigen::internal::TensorMaterializedBlock<float, 1, 1, long int> > >; long int DimId = -1; ArgType = Eigen::TensorMap<Eigen::Tensor<float, 2, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<Eigen::TensorChippingOp<DimId, XprType>, Device>::TensorBlockDesc = Eigen::internal::TensorBlockDescriptor<1, long int>; typename Eigen::TensorChippingOp<DimId, XprType>::Index = long int]
+static IndexType Eigen::internal::TensorBlockIO<Scalar, IndexType, NumDims, Layout>::Copy(const Eigen::internal::TensorBlockIO<Scalar, IndexType, NumDims, Layout>::Dst&, const Eigen::internal::TensorBlockIO<Scalar, IndexType, NumDims, Layout>::Src&, const DimensionsMap&) [with Scalar = float; IndexType = long int; int NumDims = 2; int Layout = 1; Eigen::internal::TensorBlockIO<Scalar, IndexType, NumDims, Layout>::DimensionsMap = Eigen::DSizes<int, 2>]
+Eigen::TensorEvaluator<Derived, Device>::TensorBlock Eigen::TensorEvaluator<Derived, Device>::block(Eigen::TensorEvaluator<Derived, Device>::TensorBlockDesc&, Eigen::TensorEvaluator<Derived, Device>::TensorBlockScratch&, bool) const [with Derived = Eigen::TensorMap<Eigen::Tensor<float, 2, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<Derived, Device>::TensorBlock = Eigen::internal::TensorMaterializedBlock<float, 2, 1, long int>; typename Derived::Index = long int; typename Eigen::internal::remove_const<typename Derived::Scalar>::type = float; Eigen::TensorEvaluator<Derived, Device>::TensorBlockDesc = Eigen::internal::TensorBlockDescriptor<2, long int>; Eigen::TensorEvaluator<Derived, Device>::TensorBlockScratch = Eigen::internal::TensorBlockScratchAllocator<Eigen::DefaultDevice>]
+Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::srcCoeff(Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index) const [with long int DimId = -1; ArgType = Eigen::TensorMap<Eigen::Tensor<float, 2, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index = long int]
+Eigen::TensorEvaluator<const Derived, Device>::CoeffReturnType Eigen::TensorEvaluator<const Derived, Device>::coeff(Eigen::TensorEvaluator<const Derived, Device>::Index) const [with Derived = Eigen::TensorMap<const Eigen::Tensor<float, 2, 1, long int>, 0, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Derived, Device>::CoeffReturnType = float; Eigen::TensorEvaluator<const Derived, Device>::Index = long int]
+Eigen::TensorEvaluator<const Derived, Device>::CoeffReturnType Eigen::TensorEvaluator<const Derived, Device>::coeff(Eigen::TensorEvaluator<const Derived, Device>::Index) const [with Derived = Eigen::TensorMap<const Eigen::Tensor<float, 3, 1, long int>, 0, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Derived, Device>::CoeffReturnType = float; Eigen::TensorEvaluator<const Derived, Device>::Index = long int]
+static void Eigen::internal::TensorBlockAssignment<Scalar, NumDims, TensorBlockExpr, IndexType>::Run(const Eigen::internal::TensorBlockAssignment<Scalar, NumDims, TensorBlockExpr, IndexType>::Target&, const TensorBlockExpr&) [with Scalar = float; int NumDims = 3; TensorBlockExpr = Eigen::TensorMap<const Eigen::Tensor<float, 3, 1, long int>, 0, Eigen::MakePointer>; IndexType = long int]
+static IndexType Eigen::internal::TensorBlockIO<Scalar, IndexType, NumDims, Layout>::Copy(const Eigen::internal::TensorBlockIO<Scalar, IndexType, NumDims, Layout>::Dst&, const Eigen::internal::TensorBlockIO<Scalar, IndexType, NumDims, Layout>::Src&, const DimensionsMap&) [with Scalar = float; IndexType = long int; int NumDims = 3; int Layout = 1; Eigen::internal::TensorBlockIO<Scalar, IndexType, NumDims, Layout>::DimensionsMap = Eigen::DSizes<int, 3>]
+void* Eigen::internal::TensorBlockScratchAllocator<Device>::allocate(std::size_t) [with Device = Eigen::DefaultDevice; std::size_t = long unsigned int]
+Scalar* Eigen::internal::TensorBlockDescriptor<NumDims, IndexType>::DestinationBuffer::data() const [with Scalar = float; int NumDims = 3; IndexType = long int]
+Eigen::TensorEvaluator<const Derived, Device>::TensorBlock Eigen::TensorEvaluator<const Derived, Device>::block(Eigen::TensorEvaluator<const Derived, Device>::TensorBlockDesc&, Eigen::TensorEvaluator<const Derived, Device>::TensorBlockScratch&, bool) const [with Derived = Eigen::TensorMap<Eigen::Tensor<const float, 3, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Derived, Device>::TensorBlock = Eigen::internal::TensorMaterializedBlock<float, 3, 1, long int>; typename Derived::Index = long int; typename Eigen::internal::remove_const<typename Derived::Scalar>::type = float; Eigen::TensorEvaluator<const Derived, Device>::TensorBlockDesc = Eigen::internal::TensorBlockDescriptor<3, long int>; Eigen::TensorEvaluator<const Derived, Device>::TensorBlockScratch = Eigen::internal::TensorBlockScratchAllocator<Eigen::DefaultDevice>]
+Scalar* Eigen::internal::TensorBlockDescriptor<NumDims, IndexType>::DestinationBuffer::data() const [with Scalar = float; int NumDims = 2; IndexType = long int]
+Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::srcCoeff(Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index) const [with long int DimId = -1; ArgType = const Eigen::TensorMap<Eigen::Tensor<const float, 3, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index = long int]
+Scalar* Eigen::internal::TensorBlockDescriptor<NumDims, IndexType>::DestinationBuffer::data() const [with Scalar = float; int NumDims = 1; IndexType = long int]
+Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::srcCoeff(Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index) const [with long int DimId = -1; ArgType = const Eigen::TensorChippingOp<-1, const Eigen::TensorMap<Eigen::Tensor<const float, 3, 1, long int>, 16, Eigen::MakePointer> >; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index = long int]
+void Eigen::internal::TensorBlockMapper<NumDims, Layout, IndexType>::InitializeBlockDimensions() [with int NumDims = 1; int Layout = 1; IndexType = long int]
+bool Eigen::TensorEvaluator<const Eigen::TensorAssignOp<LhsXprType, RhsXprType>, Device>::evalSubExprsIfNeeded(Eigen::TensorEvaluator<const Eigen::TensorAssignOp<LhsXprType, RhsXprType>, Device>::EvaluatorPointerType) [with LeftArgType = Eigen::TensorChippingOp<-1, Eigen::TensorMap<Eigen::Tensor<float, 2, 1, long int>, 16, Eigen::MakePointer> >; RightArgType = const Eigen::TensorCwiseBinaryOp<Eigen::internal::scalar_sum_op<float, float>, const Eigen::TensorChippingOp<-1, Eigen::TensorMap<Eigen::Tensor<float, 2, 1, long int>, 16, Eigen::MakePointer> >, const Eigen::TensorCwiseUnaryOp<Eigen::internal::bind1st_op<Eigen::internal::scalar_product_op<const float, const float> >, const Eigen::TensorChippingOp<-1, const Eigen::TensorChippingOp<-1, const Eigen::TensorMap<Eigen::Tensor<const float, 3, 1, long int>, 16, Eigen::MakePointer> > > > >; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Eigen::TensorAssignOp<LhsXprType, RhsXprType>, Device>::EvaluatorPointerType = float*]
+Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::TensorEvaluator(const XprType&, const Device&) [with long int DimId = -1; ArgType = const Eigen::TensorMap<Eigen::Tensor<const float, 3, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::XprType = Eigen::TensorChippingOp<-1, const Eigen::TensorMap<Eigen::Tensor<const float, 3, 1, long int>, 16, Eigen::MakePointer> >]
+Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::TensorEvaluator(const XprType&, const Device&) [with long int DimId = -1; ArgType = const Eigen::TensorChippingOp<-1, const Eigen::TensorMap<Eigen::Tensor<const float, 3, 1, long int>, 16, Eigen::MakePointer> >; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::XprType = Eigen::TensorChippingOp<-1, const Eigen::TensorChippingOp<-1, const Eigen::TensorMap<Eigen::Tensor<const float, 3, 1, long int>, 16, Eigen::MakePointer> > >]
+Eigen::TensorEvaluator<const Eigen::TensorCwiseBinaryOp<BinaryOp, LeftArgType, RightArgType>, Device>::TensorEvaluator(const XprType&, const Device&) [with BinaryOp = Eigen::internal::scalar_sum_op<float, float>; LeftArgType = const Eigen::TensorChippingOp<-1, Eigen::TensorMap<Eigen::Tensor<float, 2, 1, long int>, 16, Eigen::MakePointer> >; RightArgType = const Eigen::TensorCwiseUnaryOp<Eigen::internal::bind1st_op<Eigen::internal::scalar_product_op<const float, const float> >, const Eigen::TensorChippingOp<-1, const Eigen::TensorChippingOp<-1, const Eigen::TensorMap<Eigen::Tensor<const float, 3, 1, long int>, 16, Eigen::MakePointer> > > >; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Eigen::TensorCwiseBinaryOp<BinaryOp, LeftArgType, RightArgType>, Device>::XprType = Eigen::TensorCwiseBinaryOp<Eigen::internal::scalar_sum_op<float, float>, const Eigen::TensorChippingOp<-1, Eigen::TensorMap<Eigen::Tensor<float, 2, 1, long int>, 16, Eigen::MakePointer> >, const Eigen::TensorCwiseUnaryOp<Eigen::internal::bind1st_op<Eigen::internal::scalar_product_op<const float, const float> >, const Eigen::TensorChippingOp<-1, const Eigen::TensorChippingOp<-1, const Eigen::TensorMap<Eigen::Tensor<const float, 3, 1, long int>, 16, Eigen::MakePointer> > > > >]
+Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::TensorEvaluator(const XprType&, const Device&) [with long int DimId = -1; ArgType = Eigen::TensorMap<Eigen::Tensor<float, 2, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::XprType = Eigen::TensorChippingOp<-1, Eigen::TensorMap<Eigen::Tensor<float, 2, 1, long int>, 16, Eigen::MakePointer> >]
+Eigen::TensorEvaluator<Derived, Device>::CoeffReturnType& Eigen::TensorEvaluator<Derived, Device>::coeffRef(Eigen::TensorEvaluator<Derived, Device>::Index) [with Derived = Eigen::TensorMap<Eigen::Tensor<float, 2, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<Derived, Device>::CoeffReturnType = float; Eigen::TensorEvaluator<Derived, Device>::Index = long int]
+void Eigen::TensorEvaluator<Eigen::TensorChippingOp<DimId, XprType>, Device>::writePacket(Eigen::TensorEvaluator<Eigen::TensorChippingOp<DimId, XprType>, Device>::Index, const PacketReturnType&) [with int StoreMode = 0; long int DimId = -1; ArgType = Eigen::TensorMap<Eigen::Tensor<float, 3, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<Eigen::TensorChippingOp<DimId, XprType>, Device>::Index = long int; Eigen::TensorEvaluator<Eigen::TensorChippingOp<DimId, XprType>, Device>::PacketReturnType = __vector(8) float]
+void Eigen::TensorEvaluator<Eigen::TensorChippingOp<DimId, XprType>, Device>::writePacket(Eigen::TensorEvaluator<Eigen::TensorChippingOp<DimId, XprType>, Device>::Index, const PacketReturnType&) [with int StoreMode = 0; long int DimId = -1; ArgType = Eigen::TensorChippingOp<-1, Eigen::TensorMap<Eigen::Tensor<float, 3, 1, long int>, 16, Eigen::MakePointer> >; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<Eigen::TensorChippingOp<DimId, XprType>, Device>::Index = long int; Eigen::TensorEvaluator<Eigen::TensorChippingOp<DimId, XprType>, Device>::PacketReturnType = __vector(8) float]
+Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::srcCoeff(Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index) const [with long int DimId = -1; ArgType = Eigen::TensorChippingOp<-1, Eigen::TensorMap<Eigen::Tensor<float, 3, 1, long int>, 16, Eigen::MakePointer> >; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index = long int]
+Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::PacketReturnType Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::packet(Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index) const [with int LoadMode = 0; long int DimId = -1; ArgType = Eigen::TensorMap<Eigen::Tensor<float, 3, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::PacketReturnType = __vector(8) float; Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index = long int]
+Eigen::TensorEvaluator<Derived, Device>::CoeffReturnType Eigen::TensorEvaluator<Derived, Device>::coeff(Eigen::TensorEvaluator<Derived, Device>::Index) const [with Derived = Eigen::TensorMap<Eigen::Tensor<float, 3, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<Derived, Device>::CoeffReturnType = float; Eigen::TensorEvaluator<Derived, Device>::Index = long int]
+Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::srcCoeff(Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index) const [with long int DimId = -1; ArgType = Eigen::TensorMap<Eigen::Tensor<float, 3, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index = long int]
+Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::PacketReturnType Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::packet(Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index) const [with int LoadMode = 0; long int DimId = -1; ArgType = Eigen::TensorChippingOp<-1, Eigen::TensorMap<Eigen::Tensor<float, 3, 1, long int>, 16, Eigen::MakePointer> >; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::PacketReturnType = __vector(8) float; Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index = long int]
+Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::srcCoeff(Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index) const [with long int DimId = -1; ArgType = const Eigen::TensorMap<Eigen::Tensor<const float, 2, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index = long int]
+Eigen::TensorEvaluator<const Derived, Device>::CoeffReturnType Eigen::TensorEvaluator<const Derived, Device>::coeff(Eigen::TensorEvaluator<const Derived, Device>::Index) const [with Derived = Eigen::TensorMap<Eigen::Tensor<const float, 2, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Derived, Device>::CoeffReturnType = const float; Eigen::TensorEvaluator<const Derived, Device>::Index = long int]
+Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::PacketReturnType Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::packet(Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index) const [with int LoadMode = 0; long int DimId = -1; ArgType = const Eigen::TensorMap<Eigen::Tensor<const float, 2, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::PacketReturnType = __vector(8) float; Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::Index = long int]
+bool Eigen::TensorEvaluator<const Eigen::TensorAssignOp<LhsXprType, RhsXprType>, Device>::evalSubExprsIfNeeded(Eigen::TensorEvaluator<const Eigen::TensorAssignOp<LhsXprType, RhsXprType>, Device>::EvaluatorPointerType) [with LeftArgType = Eigen::TensorChippingOp<-1, Eigen::TensorChippingOp<-1, Eigen::TensorMap<Eigen::Tensor<float, 3, 1, long int>, 16, Eigen::MakePointer> > >; RightArgType = const Eigen::TensorCwiseBinaryOp<Eigen::internal::scalar_sum_op<float, float>, const Eigen::TensorChippingOp<-1, Eigen::TensorChippingOp<-1, Eigen::TensorMap<Eigen::Tensor<float, 3, 1, long int>, 16, Eigen::MakePointer> > >, const Eigen::TensorCwiseUnaryOp<Eigen::internal::bind1st_op<Eigen::internal::scalar_product_op<const float, const float> >, const Eigen::TensorChippingOp<-1, const Eigen::TensorMap<Eigen::Tensor<const float, 2, 1, long int>, 16, Eigen::MakePointer> > > >; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Eigen::TensorAssignOp<LhsXprType, RhsXprType>, Device>::EvaluatorPointerType = float*]
+Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::TensorEvaluator(const XprType&, const Device&) [with long int DimId = -1; ArgType = const Eigen::TensorMap<Eigen::Tensor<const float, 2, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::XprType = Eigen::TensorChippingOp<-1, const Eigen::TensorMap<Eigen::Tensor<const float, 2, 1, long int>, 16, Eigen::MakePointer> >]
+Eigen::TensorEvaluator<const Eigen::TensorCwiseBinaryOp<BinaryOp, LeftArgType, RightArgType>, Device>::TensorEvaluator(const XprType&, const Device&) [with BinaryOp = Eigen::internal::scalar_sum_op<float, float>; LeftArgType = const Eigen::TensorChippingOp<-1, Eigen::TensorChippingOp<-1, Eigen::TensorMap<Eigen::Tensor<float, 3, 1, long int>, 16, Eigen::MakePointer> > >; RightArgType = const Eigen::TensorCwiseUnaryOp<Eigen::internal::bind1st_op<Eigen::internal::scalar_product_op<const float, const float> >, const Eigen::TensorChippingOp<-1, const Eigen::TensorMap<Eigen::Tensor<const float, 2, 1, long int>, 16, Eigen::MakePointer> > >; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Eigen::TensorCwiseBinaryOp<BinaryOp, LeftArgType, RightArgType>, Device>::XprType = Eigen::TensorCwiseBinaryOp<Eigen::internal::scalar_sum_op<float, float>, const Eigen::TensorChippingOp<-1, Eigen::TensorChippingOp<-1, Eigen::TensorMap<Eigen::Tensor<float, 3, 1, long int>, 16, Eigen::MakePointer> > >, const Eigen::TensorCwiseUnaryOp<Eigen::internal::bind1st_op<Eigen::internal::scalar_product_op<const float, const float> >, const Eigen::TensorChippingOp<-1, const Eigen::TensorMap<Eigen::Tensor<const float, 2, 1, long int>, 16, Eigen::MakePointer> > > >]
+Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::TensorEvaluator(const XprType&, const Device&) [with long int DimId = -1; ArgType = Eigen::TensorMap<Eigen::Tensor<float, 3, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::XprType = Eigen::TensorChippingOp<-1, Eigen::TensorMap<Eigen::Tensor<float, 3, 1, long int>, 16, Eigen::MakePointer> >]
+Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::TensorEvaluator(const XprType&, const Device&) [with long int DimId = -1; ArgType = Eigen::TensorChippingOp<-1, Eigen::TensorMap<Eigen::Tensor<float, 3, 1, long int>, 16, Eigen::MakePointer> >; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<const Eigen::TensorChippingOp<DimId, XprType>, Device>::XprType = Eigen::TensorChippingOp<-1, Eigen::TensorChippingOp<-1, Eigen::TensorMap<Eigen::Tensor<float, 3, 1, long int>, 16, Eigen::MakePointer> > >]
+Eigen::internal::DimensionId<-1>::DimensionId(Eigen::DenseIndex)
+Eigen::TensorEvaluator<Derived, Device>::CoeffReturnType& Eigen::TensorEvaluator<Derived, Device>::coeffRef(Eigen::TensorEvaluator<Derived, Device>::Index) [with Derived = Eigen::TensorMap<Eigen::Tensor<int, 2, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<Derived, Device>::CoeffReturnType = int; Eigen::TensorEvaluator<Derived, Device>::Index = long int]
+Eigen::TensorEvaluator<Derived, Device>::CoeffReturnType& Eigen::TensorEvaluator<Derived, Device>::coeffRef(Eigen::TensorEvaluator<Derived, Device>::Index) [with Derived = Eigen::TensorMap<Eigen::Tensor<float, 3, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<Derived, Device>::CoeffReturnType = float; Eigen::TensorEvaluator<Derived, Device>::Index = long int]
+absl::lts_2020_09_23::Span<T>::operator[](absl::lts_2020_09_23::Span<T>::size_type) const::<lambda()> [with T = const long int]
+absl::lts_2020_09_23::string_view::CheckLengthInternal(absl::lts_2020_09_23::string_view::size_type)::<lambda()>
+N10tensorflow4core10RefCountedE
+16PoolingBySlotsOp
+20PoolingBySlotsGradOp
+ZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_
+@GetSlotFids
 GetSlotFidsOp
 tensorflow_hs_addon/cc/kernels/get_slot_fids.cc
-GroupBySlots
-GroupBySlotsOp
-tensorflow_hs_addon/cc/kernels/group_by_slots.cc
-fid/weighed_fid batch size should match
-Input size: 
-start shard 
-, slot: 
-, weight:
-TFHS>IsIn
-IsInOp<int32>
-tensorflow_hs_addon/cc/kernels/is_in.cc
-IsInOp<int64>
+Eigen::TensorEvaluator<Derived, Device>::CoeffReturnType& Eigen::TensorEvaluator<Derived, Device>::coeffRef(Eigen::TensorEvaluator<Derived, Device>::Index) [with Derived = Eigen::TensorMap<Eigen::Tensor<float, 2, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<Derived, Device>::CoeffReturnType = float; Eigen::TensorEvaluator<Derived, Device>::Index = long int]
+Eigen::TensorEvaluator<Derived, Device>::CoeffReturnType& Eigen::TensorEvaluator<Derived, Device>::coeffRef(Eigen::TensorEvaluator<Derived, Device>::Index) [with Derived = Eigen::TensorMap<Eigen::Tensor<int, 2, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<Derived, Device>::CoeffReturnType = int; Eigen::TensorEvaluator<Derived, Device>::Index = long int]
+absl::lts_2020_09_23::Span<T>::operator[](absl::lts_2020_09_23::Span<T>::size_type) const::<lambda()> [with T = const long int]
+absl::lts_2020_09_23::string_view::CheckLengthInternal(absl::lts_2020_09_23::string_view::size_type)::<lambda()>
+13GetSlotFidsOp
+ZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_
 SplitRaggedBlock
 SplitRaggedBlockOp<float>
+SplitRaggedBlockOp<int32>
+SplitRaggedBlockOp<int64>
 ./tensorflow_hs_addon/cc/kernels/split_ragged_block.h
 block index: 
 ; pad_value: 
 num rows doesn't match
 block_index out of range
+Input size: 
 padded block size: 
-SplitRaggedBlockOp<int32>
-SplitRaggedBlockOp<int64>
-values: T
-block_sizes: int32
-block_index: int32
-pad_value: T
-block_values: T
-T: {float32, int32, int64}
-slots: int32
-fids: int64
-weighted_fids: int64
-fid_weights: float32
-slot_size: int32
-ordered_fids: int64
-ordered_weights: float32
-fid_indices: int32
+start shard 
+absl::lts_2020_09_23::Span<T>::operator[](absl::lts_2020_09_23::Span<T>::size_type) const::<lambda()> [with T = const long int]
+absl::lts_2020_09_23::string_view::CheckLengthInternal(absl::lts_2020_09_23::string_view::size_type)::<lambda()>
+ZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_
+ZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_
+ZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_
+18SplitRaggedBlockOpIfE
+18SplitRaggedBlockOpIiE
+18SplitRaggedBlockOpIlE
+FeatureVecToSegmentsOp
+UnsortedFeatureVecToSegments
+UnsortedFeatureVecToSegmentsOp
+vector::reserve
+vector::_M_default_append
+tensorflow_hs_addon/cc/kernels/feature_vec_to_sparse.cc
+Eigen::TensorEvaluator<Derived, Device>::CoeffReturnType& Eigen::TensorEvaluator<Derived, Device>::coeffRef(Eigen::TensorEvaluator<Derived, Device>::Index) [with Derived = Eigen::TensorMap<Eigen::Tensor<float, 1, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<Derived, Device>::CoeffReturnType = float; Eigen::TensorEvaluator<Derived, Device>::Index = long int]
+Eigen::TensorEvaluator<Derived, Device>::CoeffReturnType& Eigen::TensorEvaluator<Derived, Device>::coeffRef(Eigen::TensorEvaluator<Derived, Device>::Index) [with Derived = Eigen::TensorMap<Eigen::Tensor<int, 1, 1, long int>, 16, Eigen::MakePointer>; Device = Eigen::DefaultDevice; Eigen::TensorEvaluator<Derived, Device>::CoeffReturnType = int; Eigen::TensorEvaluator<Derived, Device>::Index = long int]
+absl::lts_2020_09_23::Span<T>::operator[](absl::lts_2020_09_23::Span<T>::size_type) const::<lambda()> [with T = const long int]
+absl::lts_2020_09_23::string_view::CheckLengthInternal(absl::lts_2020_09_23::string_view::size_type)::<lambda()>
+22FeatureVecToSegmentsOp
+30UnsortedFeatureVecToSegmentsOp
+GroupBySlots
+GroupBySlotsOp
+tensorflow_hs_addon/cc/kernels/group_by_slots.cc
+fid/weighed_fid batch size should match
+, slot: 
+, weight:
+absl::lts_2020_09_23::Span<T>::operator[](absl::lts_2020_09_23::Span<T>::size_type) const::<lambda()> [with T = const long int]
+absl::lts_2020_09_23::string_view::CheckLengthInternal(absl::lts_2020_09_23::string_view::size_type)::<lambda()>
+14GroupBySlotsOp
+ZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_
+?/usr/include/sparsehash/internal/densehashtable.h
+(bucket_count() & (bucket_count()-1)) == 0
+settings.use_deleted() || num_deleted == 0
+num_probes < bucket_count() && "Hashtable is full: an error in key_equal<> or hash<>"
+ht.empty()
+resize overflow
+settings.use_empty()
+ParseFeatureVec
+ParseFeatureVecOp
+num_elements >= num_deleted
+insert overflow
+tensorflow_hs_addon/cc/kernels/parse_feature_vec.cc
+bucket_count() >= HT_MIN_BUCKETS
+(!settings.use_empty() || !equals(get_key(obj), get_key(val_info.emptyval))) && "Inserting the empty key"
+(!settings.use_deleted() || !equals(get_key(obj), key_info.delkey)) && "Inserting the deleted key"
+std::pair<google::dense_hashtable_iterator<V, K, HF, ExK, SetK, EqK, A>, bool> google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::insert_noresize(google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::const_reference) [with Value = std::pair<const long int, int>; Key = long int; HashFcn = std::tr1::hash<long int>; ExtractKey = google::dense_hash_map<long int, int>::SelectKey; SetKey = google::dense_hash_map<long int, int>::SetKey; EqualKey = std::equal_to<long int>; Alloc = google::libc_allocator_with_realloc<std::pair<const long int, int> >; google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::const_reference = const std::pair<const long int, int>&]
+bool google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::test_deleted(const const_iterator&) const [with Value = std::pair<const long int, int>; Key = long int; HashFcn = std::tr1::hash<long int>; ExtractKey = google::dense_hash_map<long int, int>::SelectKey; SetKey = google::dense_hash_map<long int, int>::SetKey; EqualKey = std::equal_to<long int>; Alloc = google::libc_allocator_with_realloc<std::pair<const long int, int> >; google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::const_iterator = google::dense_hashtable_const_iterator<std::pair<const long int, int>, long int, std::tr1::hash<long int>, google::dense_hash_map<long int, int>::SelectKey, google::dense_hash_map<long int, int>::SetKey, std::equal_to<long int>, google::libc_allocator_with_realloc<std::pair<const long int, int> > >]
+bool google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::test_empty(const const_iterator&) const [with Value = std::pair<const long int, int>; Key = long int; HashFcn = std::tr1::hash<long int>; ExtractKey = google::dense_hash_map<long int, int>::SelectKey; SetKey = google::dense_hash_map<long int, int>::SetKey; EqualKey = std::equal_to<long int>; Alloc = google::libc_allocator_with_realloc<std::pair<const long int, int> >; google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::const_iterator = google::dense_hashtable_const_iterator<std::pair<const long int, int>, long int, std::tr1::hash<long int>, google::dense_hash_map<long int, int>::SelectKey, google::dense_hash_map<long int, int>::SetKey, std::equal_to<long int>, google::libc_allocator_with_realloc<std::pair<const long int, int> > >]
+void google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::clear_to_size(google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::size_type) [with Value = std::pair<const long int, int>; Key = long int; HashFcn = std::tr1::hash<long int>; ExtractKey = google::dense_hash_map<long int, int>::SelectKey; SetKey = google::dense_hash_map<long int, int>::SetKey; EqualKey = std::equal_to<long int>; Alloc = google::libc_allocator_with_realloc<std::pair<const long int, int> >; google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::size_type = long unsigned int]
+void google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::copy_from(const google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>&, google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::size_type) [with Value = std::pair<const long int, int>; Key = long int; HashFcn = std::tr1::hash<long int>; ExtractKey = google::dense_hash_map<long int, int>::SelectKey; SetKey = google::dense_hash_map<long int, int>::SetKey; EqualKey = std::equal_to<long int>; Alloc = google::libc_allocator_with_realloc<std::pair<const long int, int> >; google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::size_type = long unsigned int]
+google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::dense_hashtable(const google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>&, google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::size_type) [with Value = std::pair<const long int, int>; Key = long int; HashFcn = std::tr1::hash<long int>; ExtractKey = google::dense_hash_map<long int, int>::SelectKey; SetKey = google::dense_hash_map<long int, int>::SetKey; EqualKey = std::equal_to<long int>; Alloc = google::libc_allocator_with_realloc<std::pair<const long int, int> >; google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::size_type = long unsigned int]
+bool google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::maybe_shrink() [with Value = std::pair<const long int, int>; Key = long int; HashFcn = std::tr1::hash<long int>; ExtractKey = google::dense_hash_map<long int, int>::SelectKey; SetKey = google::dense_hash_map<long int, int>::SetKey; EqualKey = std::equal_to<long int>; Alloc = google::libc_allocator_with_realloc<std::pair<const long int, int> >]
+bool google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::test_deleted(google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::size_type) const [with Value = std::pair<const long int, int>; Key = long int; HashFcn = std::tr1::hash<long int>; ExtractKey = google::dense_hash_map<long int, int>::SelectKey; SetKey = google::dense_hash_map<long int, int>::SetKey; EqualKey = std::equal_to<long int>; Alloc = google::libc_allocator_with_realloc<std::pair<const long int, int> >; google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::size_type = long unsigned int]
+bool google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::test_empty(google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::size_type) const [with Value = std::pair<const long int, int>; Key = long int; HashFcn = std::tr1::hash<long int>; ExtractKey = google::dense_hash_map<long int, int>::SelectKey; SetKey = google::dense_hash_map<long int, int>::SetKey; EqualKey = std::equal_to<long int>; Alloc = google::libc_allocator_with_realloc<std::pair<const long int, int> >; google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::size_type = long unsigned int]
+std::pair<typename Alloc::rebind<Value>::other::size_type, typename Alloc::rebind<Value>::other::size_type> google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::find_position(const key_type&) const [with Value = std::pair<const long int, int>; Key = long int; HashFcn = std::tr1::hash<long int>; ExtractKey = google::dense_hash_map<long int, int>::SelectKey; SetKey = google::dense_hash_map<long int, int>::SetKey; EqualKey = std::equal_to<long int>; Alloc = google::libc_allocator_with_realloc<std::pair<const long int, int> >; typename Alloc::rebind<Value>::other::size_type = long unsigned int; google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::key_type = long int]
+void google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::set_empty_key(google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::const_reference) [with Value = std::pair<const long int, int>; Key = long int; HashFcn = std::tr1::hash<long int>; ExtractKey = google::dense_hash_map<long int, int>::SelectKey; SetKey = google::dense_hash_map<long int, int>::SetKey; EqualKey = std::equal_to<long int>; Alloc = google::libc_allocator_with_realloc<std::pair<const long int, int> >; google::dense_hashtable<Value, Key, HashFcn, ExtractKey, SetKey, EqualKey, Alloc>::const_reference = const std::pair<const long int, int>&]
+absl::lts_2020_09_23::string_view::CheckLengthInternal(absl::lts_2020_09_23::string_view::size_type)::<lambda()>
+absl::lts_2020_09_23::Span<T>::operator[](absl::lts_2020_09_23::Span<T>::size_type) const::<lambda()> [with T = const long int]
+17ParseFeatureVecOp
+L>TFHS>IsIn
+IsInOp<int32>
+IsInOp<int64>
+tensorflow_hs_addon/cc/kernels/is_in.cc
+absl::lts_2020_09_23::Span<T>::operator[](absl::lts_2020_09_23::Span<T>::size_type) const::<lambda()> [with T = const long int]
+6IsInOpIiE
+6IsInOpIlE
+vector::_M_range_check: __n (which is %zu) >= this->size() (which is %zu)
+/usr/local/lib/python3.7/dist-packages/tensorflow/include/tensorflow/core/framework/shape_inference.h
+Check failed: val >= 0 || val == InferenceContext::kUnknownDim 
+Dimension must be non-negative or equal to InferenceContext::kUnknownDim but got 
+Check failed: value >= 0 || value == InferenceContext::kUnknownDim 
+Check failed: dim.IsSet() 
+Internal error: Got nullptr for Dimension.
+num slots is unknown
+embedding dim is unknown
 fid_slots: int32
-embeddings: float32
 pooled_embeddings: float32
 slot_sizes: int32
 pooled_grads: float32
-grads: float32
 slot: int32
 selected_fid_indices: int32
 selected_fid_weights: float32
+values: T
 filter: T
 T: {int32, int64}
 mask: bool
-tensorflow_hs_addon/cc/ops/reco_ops.cc
-/Users/npbool/Projects/tensorflow-hs-addon/venv-368/lib/python3.6/site-packages/tensorflow/include/tensorflow/core/framework/shape_inference.h
-Dimension must be non-negative or equal to InferenceContext::kUnknownDim but got 
-Check failed: val >= 0 || val == InferenceContext::kUnknownDim 
-num slots is known
-s->rank_ != kUnknownRank
-Check failed: dim.IsSet() 
-Internal error: Got nullptr for Dimension.
-num slots is unknown
-embedding dim is unknown
-@__ZN10tensorflow10DEVICE_CPUE
-@__ZN10tensorflow15TensorShapeBaseINS_11TensorShapeEEC2EN4absl14lts_2020_09_234SpanIKxEE
-@__ZNK10tensorflow15TensorShapeBaseINS_11TensorShapeEE8dim_sizeEi
-@__ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb
-@__ZTIN10tensorflow8OpKernelE
-@__ZTVN10tensorflow14kernel_factory17OpKernelRegistrar18PtrOpKernelFactoryE
-@__ZNSt12length_errorD1Ev
-@__ZNSt3__113basic_istreamIcNS_11char_traitsIcEEED0Ev
-@__ZNSt3__113basic_istreamIcNS_11char_traitsIcEEED1Ev
-@__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEED0Ev
-@__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEED1Ev
-@__ZNSt3__114basic_iostreamIcNS_11char_traitsIcEEED0Ev
-@__ZNSt3__114basic_iostreamIcNS_11char_traitsIcEEED1Ev
-@__ZNSt3__115basic_streambufIcNS_11char_traitsIcEEE4syncEv
-@__ZNSt3__115basic_streambufIcNS_11char_traitsIcEEE5imbueERKNS_6localeE
-@__ZNSt3__115basic_streambufIcNS_11char_traitsIcEEE5uflowEv
-@__ZNSt3__115basic_streambufIcNS_11char_traitsIcEEE6setbufEPcl
-@__ZNSt3__115basic_streambufIcNS_11char_traitsIcEEE6xsgetnEPcl
-@__ZNSt3__115basic_streambufIcNS_11char_traitsIcEEE6xsputnEPKcl
-@__ZNSt3__115basic_streambufIcNS_11char_traitsIcEEE9showmanycEv
-@__ZNSt3__15ctypeIcE2idE
-@__ZNSt9bad_allocD1Ev
-@__ZTINSt3__113basic_istreamIcNS_11char_traitsIcEEEE
-@__ZTINSt3__113basic_ostreamIcNS_11char_traitsIcEEEE
-@__ZTINSt3__114basic_iostreamIcNS_11char_traitsIcEEEE
-@__ZTINSt3__115basic_streambufIcNS_11char_traitsIcEEEE
-@__ZTISt12length_error
-@__ZTISt9bad_alloc
-@__ZTVN10__cxxabiv117__class_type_infoE
-@__ZTVN10__cxxabiv120__si_class_type_infoE
-@__ZTVSt12length_error
-@__ZThn16_NSt3__114basic_iostreamIcNS_11char_traitsIcEEED0Ev
-@__ZThn16_NSt3__114basic_iostreamIcNS_11char_traitsIcEEED1Ev
-@__ZTv0_n24_NSt3__113basic_istreamIcNS_11char_traitsIcEEED0Ev
-@__ZTv0_n24_NSt3__113basic_istreamIcNS_11char_traitsIcEEED1Ev
-@__ZTv0_n24_NSt3__113basic_ostreamIcNS_11char_traitsIcEEED0Ev
-@__ZTv0_n24_NSt3__113basic_ostreamIcNS_11char_traitsIcEEED1Ev
-@__ZTv0_n24_NSt3__114basic_iostreamIcNS_11char_traitsIcEEED0Ev
-@__ZTv0_n24_NSt3__114basic_iostreamIcNS_11char_traitsIcEEED1Ev
-@__ZdlPv
-@___gxx_personality_v0
-@___stack_chk_guard
-@dyld_stub_binder
-@__ZGVZN5Eigen8internal20manage_caching_sizesENS_6ActionEPlS2_S2_E12m_cacheSizes
-@__ZGVZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS4_E17vmodule_activated
-@__ZGVZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
-@__ZGVZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
-@__ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
-@__ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
-@__ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
-@__ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
-@__ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
-@__ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
-@__ZGVZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
-@__ZGVZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
-@__ZGVZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
-@__ZGVZZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
-@__ZGVZZN7FidIter7advanceEvENKUliPKcE_clEiS1_E17vmodule_activated
-@__ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE0_clEiS5_E17vmodule_activated
-@__ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE1_clEiS5_E17vmodule_activated
-@__ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS5_E17vmodule_activated
-@__ZGVZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS5_E17vmodule_activated
-@__ZGVZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated
-@__ZGVZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated
-@__ZGVZZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated
-@__ZN10tensorflow15TensorShapeBaseINS_11TensorShapeEEC2EN4absl14lts_2020_09_234SpanIKxEE
-@__ZNK10tensorflow15TensorShapeBaseINS_11TensorShapeEE8dim_sizeEi
-@__ZTI13GetSlotFidsOp
-@__ZTI14GroupBySlotsOp
-@__ZTI16PoolingBySlotsOp
-@__ZTI18SplitRaggedBlockOpIfE
-@__ZTI18SplitRaggedBlockOpIiE
-@__ZTI18SplitRaggedBlockOpIxE
-@__ZTI20PoolingBySlotsGradOp
-@__ZTI6IsInOpIiE
-@__ZTI6IsInOpIxE
-@__ZTINSt3__110__function6__baseIFN10tensorflow6StatusEPNS2_15shape_inference16InferenceContextEEEE
-@__ZTINSt3__110__function6__baseIFvxxEEE
-@__ZTINSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-@__ZTINSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-@__ZTINSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-@__ZTINSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-@__ZTINSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-@__ZTINSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-@__ZTINSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEEE
-@__ZTINSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEEE
-@__ZTISt12length_error
-@__ZTIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-@__ZTIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-@__ZTIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-@__ZTIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-@__ZTIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-@__ZTIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-@__ZTS13GetSlotFidsOp
-@__ZTS14GroupBySlotsOp
-@__ZTS16PoolingBySlotsOp
-@__ZTS18SplitRaggedBlockOpIfE
-@__ZTS18SplitRaggedBlockOpIiE
-@__ZTS18SplitRaggedBlockOpIxE
-@__ZTS20PoolingBySlotsGradOp
-@__ZTS6IsInOpIiE
-@__ZTS6IsInOpIxE
-@__ZTSNSt3__110__function6__baseIFN10tensorflow6StatusEPNS2_15shape_inference16InferenceContextEEEE
-@__ZTSNSt3__110__function6__baseIFvxxEEE
-@__ZTSNSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-@__ZTSNSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-@__ZTSNSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-@__ZTSNSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-@__ZTSNSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-@__ZTSNSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-@__ZTSNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEEE
-@__ZTSNSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEEE
-@__ZTSZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-@__ZTSZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-@__ZTSZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-@__ZTSZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-@__ZTSZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-@__ZTSZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-@__ZZN5Eigen8internal20manage_caching_sizesENS_6ActionEPlS2_S2_E12m_cacheSizes
-@__ZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS4_E17vmodule_activated
-@__ZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
-@__ZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
-@__ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
-@__ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
-@__ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
-@__ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
-@__ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
-@__ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
-@__ZZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
-@__ZZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
-@__ZZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
-@__ZZZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
-@__ZZZN7FidIter7advanceEvENKUliPKcE_clEiS1_E17vmodule_activated
-@__ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE0_clEiS5_E17vmodule_activated
-@__ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE1_clEiS5_E17vmodule_activated
-@__ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS5_E17vmodule_activated
-@__ZZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS5_E17vmodule_activated
-@__ZZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated
-@__ZZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated
-@__ZZZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated
-@__ZdlPv
-@__Unwind_Resume
-@__ZN10tensorflow11register_op19OpDefBuilderWrapperclEv
-@__ZN10tensorflow12OpDefBuilder10SetShapeFnENSt3__18functionIFNS_6StatusEPNS_15shape_inference16InferenceContextEEEE
-@__ZN10tensorflow12OpDefBuilder4AttrENSt3__112basic_stringIcNS1_11char_traitsIcEENS1_9allocatorIcEEEE
-@__ZN10tensorflow12OpDefBuilder5InputENSt3__112basic_stringIcNS1_11char_traitsIcEENS1_9allocatorIcEEEE
-@__ZN10tensorflow12OpDefBuilder6OutputENSt3__112basic_stringIcNS1_11char_traitsIcEENS1_9allocatorIcEEEE
-@__ZN10tensorflow12OpDefBuilderC1ENSt3__112basic_stringIcNS1_11char_traitsIcEENS1_9allocatorIcEEEE
-@__ZN10tensorflow14TensorShapeRep19DestructorOutOfLineEv
-@__ZN10tensorflow14kernel_factory17OpKernelRegistrar12InitInternalEPKNS_9KernelDefEN4absl14lts_2020_09_2311string_viewENSt3__110unique_ptrINS0_15OpKernelFactoryENS8_14default_deleteISA_EEEE
-@__ZN10tensorflow15OpKernelContext10CtxFailureEPKciRKNS_6StatusE
-@__ZN10tensorflow15OpKernelContext15allocate_outputEiRKNS_11TensorShapeEPPNS_6TensorE
-@__ZN10tensorflow15OpKernelContext21CtxFailureWithWarningEPKciRKNS_6StatusE
-@__ZN10tensorflow15shape_inference16InferenceContext10ReplaceDimENS0_11ShapeHandleExNS0_15DimensionHandleEPS2_
-@__ZN10tensorflow15shape_inference16InferenceContext8WithRankENS0_11ShapeHandleExPS2_
-@__ZN10tensorflow15shape_inference16InferenceContext9MakeShapeESt16initializer_listINS0_19DimensionOrConstantEE
-@__ZN10tensorflow16KernelDefBuilder14TypeConstraintEPKcNS_8DataTypeE
-@__ZN10tensorflow16KernelDefBuilder5BuildEv
-@__ZN10tensorflow16KernelDefBuilder6DeviceEPKc
-@__ZN10tensorflow16KernelDefBuilderC2EPKc
-@__ZN10tensorflow16KernelDefBuilderD2Ev
-@__ZN10tensorflow22CheckNotInComputeAsyncEPNS_15OpKernelContextEPKc
-@__ZN10tensorflow5OpDefD1Ev
-@__ZN10tensorflow6StatusC1ENS_5error4CodeEN4absl14lts_2020_09_2311string_viewEONSt3__16vectorINS_10StackFrameENS6_9allocatorIS8_EEEE
-@__ZN10tensorflow6thread10ThreadPool11ParallelForExxRKNSt3__18functionIFvxxEEE
-@__ZN10tensorflow7strings6StrCatERKNS0_8AlphaNumE
-@__ZN10tensorflow8OpKernelC2EPNS_20OpKernelConstructionE
-@__ZN10tensorflow8OpKernelD2Ev
-@__ZN10tensorflow8internal10LogMessage16VmoduleActivatedEPKci
-@__ZN10tensorflow8internal10LogMessageC1EPKcii
-@__ZN10tensorflow8internal10LogMessageD1Ev
-@__ZN10tensorflow8internal15LogMessageFatalC1EPKci
-@__ZN10tensorflow8internal15LogMessageFatalD1Ev
-@__ZN10tensorflow8internal21CheckOpMessageBuilder7ForVar2Ev
-@__ZN10tensorflow8internal21CheckOpMessageBuilder9NewStringEv
-@__ZN10tensorflow8internal21CheckOpMessageBuilderC1EPKc
-@__ZN10tensorflow8internal21CheckOpMessageBuilderD1Ev
-@__ZNK10tensorflow11TensorShape10IsSameSizeERKS0_
-@__ZNK10tensorflow15OpKernelContext5inputEi
-@__ZNK10tensorflow6Tensor21CheckTypeAndIsAlignedENS_8DataTypeE
-@__ZNK10tensorflow6Tensor30CheckIsAlignedAndSingleElementEv
-@__ZNK10tensorflow6Tensor9CheckTypeENS_8DataTypeE
-@__ZNKSt3__120__vector_base_commonILb1EE20__throw_length_errorEv
-@__ZNKSt3__120__vector_base_commonILb1EE20__throw_out_of_rangeEv
-@__ZNKSt3__121__basic_string_commonILb1EE20__throw_length_errorEv
-@__ZNKSt3__16locale9use_facetERNS0_2idE
-@__ZNKSt3__18ios_base6getlocEv
-@__ZNSt11logic_errorC2EPKc
-@__ZNSt3__112__next_primeEm
-@__ZNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEE6resizeEmc
-@__ZNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEE9push_backEc
-@__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEE6sentryC1ERS3_
-@__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEE6sentryD1Ev
-@__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEElsEf
-@__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEElsEi
-@__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEElsEm
-@__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEElsEx
-@__ZNSt3__114basic_iostreamIcNS_11char_traitsIcEEED2Ev
-@__ZNSt3__115basic_streambufIcNS_11char_traitsIcEEEC2Ev
-@__ZNSt3__115basic_streambufIcNS_11char_traitsIcEEED2Ev
-@__ZNSt3__16localeD1Ev
-@__ZNSt3__18ios_base33__set_badbit_and_consider_rethrowEv
-@__ZNSt3__18ios_base4initEPv
-@__ZNSt3__18ios_base5clearEj
-@__ZNSt3__19basic_iosIcNS_11char_traitsIcEEED2Ev
-@__ZNSt9bad_allocC1Ev
-@__ZSt9terminatev
-@___assert_rtn
-@___bzero
-@___cxa_allocate_exception
-@___cxa_begin_catch
-@___cxa_end_catch
-@___cxa_free_exception
-@___cxa_guard_abort
-@___cxa_guard_acquire
-@___cxa_guard_release
-@___cxa_throw
-@___stack_chk_fail
-@_malloc
-@_memcpy
-@_memset
-@_strlen
-YNSt3__11
-20PoolingBySlotsGradOp
-6IsInOpI
-6PoolingBySlotsOp
-3GetSlotFidsOp
-4GroupBySlotsOp
-8SplitRaggedBlockOpI
-8basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEEE
-5basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEEE
-0__function6__
-funcIZN1
-6PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-3GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-4GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-8SplitRaggedBlockOpI
-N10tensorflow6StatusEPNS2_15shape_inference16InferenceContextEEEE
-6PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-3GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-4GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-8SplitRaggedBlockOpI
-fE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-iE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-xE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-fE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-iE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-xE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-NSt3__11
-20PoolingBySlotsGradOp
-6IsInOpI
-6PoolingBySlotsOp
-3GetSlotFidsOp
-4GroupBySlotsOp
-8SplitRaggedBlockOpI
-8basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEEE
-5basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEEE
-0__function6__
-funcIZN1
-N10tensorflow6StatusEPNS2_15shape_inference16InferenceContextEEEE
-6PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-3GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-4GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-8SplitRaggedBlockOpI
-6PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-3GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-4GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-8SplitRaggedBlockOpI
-fE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-iE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-xE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-fE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-iE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-xE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-N5Eigen8internal20manage_caching_sizesENS_6ActionEPlS2_S2_E12m_cacheSizes
-20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
-"7FidIter7advanceEvENKUliPKcE_clEiS1_E17vmodule_activated
-6PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
-4GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE
-"8SplitRaggedBlockOpI
-N5Eigen8internal20manage_caching_sizesENS_6ActionEPlS2_S2_E12m_cacheSizes
-20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
-"7FidIter7advanceEvENKUliPKcE_clEiS1_E17vmodule_activated
-6PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
-4GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE
-"8SplitRaggedBlockOpI
-6PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS5_E17vmodule_activated
- 4GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE
-#8SplitRaggedBlockOpI
-6PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS5_E17vmodule_activated
-"4GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE
-$8SplitRaggedBlockOpI
-_clEiS4_E17vmodule_activated
-"0_clEiS4_E17vmodule_activated
-_clEiS4_E17vmodule_activated
-#0_clEiS4_E17vmodule_activated
-_clEiS5_E17vmodule_activated
-$0_clEiS5_E17vmodule_activated
-%1_clEiS5_E17vmodule_activated
-_clEiS5_E17vmodule_activated
-%0_clEiS5_E17vmodule_activated
-%1_clEiS5_E17vmodule_activated
-fE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE
-&iE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE
-.xE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE
-_clEiS5_E17vmodule_activated
-'0_clEiS5_E17vmodule_activated
-)1_clEiS5_E17vmodule_activated
-fE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE
-(iE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE
-/xE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE
-_clEiS5_E17vmodule_activated
-)0_clEiS5_E17vmodule_activated
-)1_clEiS5_E17vmodule_activated
-fE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated
-,iE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated
-0xE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated
-fE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated
-.iE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated
-0xE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated
-_clEiS5_E17vmodule_activated
-/0_clEiS5_E17vmodule_activated
-01_clEiS5_E17vmodule_activated
-_clEiS5_E17vmodule_activated
-00_clEiS5_E17vmodule_activated
-01_clEiS5_E17vmodule_activated
-_clEiS5_E17vmodule_activated
-10_clEiS5_E17vmodule_activated
-21_clEiS5_E17vmodule_activated
-_clEiS5_E17vmodule_activated
-20_clEiS5_E17vmodule_activated
-21_clEiS5_E17vmodule_activated
-'`00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000 `` `   
-__ZGVZN5Eigen8internal20manage_caching_sizesENS_6ActionEPlS2_S2_E12m_cacheSizes
-__ZGVZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS4_E17vmodule_activated
-__ZGVZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
-__ZGVZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
-__ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
-__ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
-__ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
-__ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
-__ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
-__ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
-__ZGVZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
-__ZGVZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
-__ZGVZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
-__ZGVZZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
-__ZGVZZN7FidIter7advanceEvENKUliPKcE_clEiS1_E17vmodule_activated
-__ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE0_clEiS5_E17vmodule_activated
-__ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE1_clEiS5_E17vmodule_activated
-__ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS5_E17vmodule_activated
-__ZGVZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS5_E17vmodule_activated
-__ZGVZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated
-__ZGVZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated
-__ZGVZZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated
-__ZTI13GetSlotFidsOp
-__ZTI14GroupBySlotsOp
-__ZTI16PoolingBySlotsOp
-__ZTI18SplitRaggedBlockOpIfE
-__ZTI18SplitRaggedBlockOpIiE
-__ZTI18SplitRaggedBlockOpIxE
-__ZTI20PoolingBySlotsGradOp
-__ZTI6IsInOpIiE
-__ZTI6IsInOpIxE
-__ZTINSt3__110__function6__baseIFN10tensorflow6StatusEPNS2_15shape_inference16InferenceContextEEEE
-__ZTINSt3__110__function6__baseIFvxxEEE
-__ZTINSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-__ZTINSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-__ZTINSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-__ZTINSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-__ZTINSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-__ZTINSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-__ZTINSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEEE
-__ZTINSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEEE
-__ZTIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-__ZTIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-__ZTIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-__ZTIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-__ZTIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-__ZTIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-__ZTS13GetSlotFidsOp
-__ZTS14GroupBySlotsOp
-__ZTS16PoolingBySlotsOp
-__ZTS18SplitRaggedBlockOpIfE
-__ZTS18SplitRaggedBlockOpIiE
-__ZTS18SplitRaggedBlockOpIxE
-__ZTS20PoolingBySlotsGradOp
-__ZTS6IsInOpIiE
-__ZTS6IsInOpIxE
-__ZTSNSt3__110__function6__baseIFN10tensorflow6StatusEPNS2_15shape_inference16InferenceContextEEEE
-__ZTSNSt3__110__function6__baseIFvxxEEE
-__ZTSNSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-__ZTSNSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-__ZTSNSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-__ZTSNSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-__ZTSNSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-__ZTSNSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-__ZTSNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEEE
-__ZTSNSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEEE
-__ZTSZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-__ZTSZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-__ZTSZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-__ZTSZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-__ZTSZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-__ZTSZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_
-__ZZN5Eigen8internal20manage_caching_sizesENS_6ActionEPlS2_S2_E12m_cacheSizes
-__ZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS4_E17vmodule_activated
-__ZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
-__ZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
-__ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
-__ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
-__ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
-__ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
-__ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
-__ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
-__ZZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
-__ZZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
-__ZZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
-__ZZZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
-__ZZZN7FidIter7advanceEvENKUliPKcE_clEiS1_E17vmodule_activated
-__ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE0_clEiS5_E17vmodule_activated
-__ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE1_clEiS5_E17vmodule_activated
-__ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS5_E17vmodule_activated
-__ZZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS5_E17vmodule_activated
-__ZZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated
-__ZZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated
-__ZZZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated
-__Unwind_Resume
-__ZN10tensorflow10DEVICE_CPUE
-__ZN10tensorflow11register_op19OpDefBuilderWrapperclEv
-__ZN10tensorflow12OpDefBuilder10SetShapeFnENSt3__18functionIFNS_6StatusEPNS_15shape_inference16InferenceContextEEEE
-__ZN10tensorflow12OpDefBuilder4AttrENSt3__112basic_stringIcNS1_11char_traitsIcEENS1_9allocatorIcEEEE
-__ZN10tensorflow12OpDefBuilder5InputENSt3__112basic_stringIcNS1_11char_traitsIcEENS1_9allocatorIcEEEE
-__ZN10tensorflow12OpDefBuilder6OutputENSt3__112basic_stringIcNS1_11char_traitsIcEENS1_9allocatorIcEEEE
-__ZN10tensorflow12OpDefBuilderC1ENSt3__112basic_stringIcNS1_11char_traitsIcEENS1_9allocatorIcEEEE
-__ZN10tensorflow14TensorShapeRep19DestructorOutOfLineEv
-__ZN10tensorflow14kernel_factory17OpKernelRegistrar12InitInternalEPKNS_9KernelDefEN4absl14lts_2020_09_2311string_viewENSt3__110unique_ptrINS0_15OpKernelFactoryENS8_14default_deleteISA_EEEE
-__ZN10tensorflow15OpKernelContext10CtxFailureEPKciRKNS_6StatusE
-__ZN10tensorflow15OpKernelContext15allocate_outputEiRKNS_11TensorShapeEPPNS_6TensorE
-__ZN10tensorflow15OpKernelContext21CtxFailureWithWarningEPKciRKNS_6StatusE
-__ZN10tensorflow15TensorShapeBaseINS_11TensorShapeEEC2EN4absl14lts_2020_09_234SpanIKxEE
-__ZN10tensorflow15shape_inference16InferenceContext10ReplaceDimENS0_11ShapeHandleExNS0_15DimensionHandleEPS2_
-__ZN10tensorflow15shape_inference16InferenceContext8WithRankENS0_11ShapeHandleExPS2_
-__ZN10tensorflow15shape_inference16InferenceContext9MakeShapeESt16initializer_listINS0_19DimensionOrConstantEE
-__ZN10tensorflow16KernelDefBuilder14TypeConstraintEPKcNS_8DataTypeE
-__ZN10tensorflow16KernelDefBuilder5BuildEv
-__ZN10tensorflow16KernelDefBuilder6DeviceEPKc
-__ZN10tensorflow16KernelDefBuilderC2EPKc
-__ZN10tensorflow16KernelDefBuilderD2Ev
-__ZN10tensorflow22CheckNotInComputeAsyncEPNS_15OpKernelContextEPKc
-__ZN10tensorflow5OpDefD1Ev
-__ZN10tensorflow6StatusC1ENS_5error4CodeEN4absl14lts_2020_09_2311string_viewEONSt3__16vectorINS_10StackFrameENS6_9allocatorIS8_EEEE
-__ZN10tensorflow6thread10ThreadPool11ParallelForExxRKNSt3__18functionIFvxxEEE
-__ZN10tensorflow7strings6StrCatERKNS0_8AlphaNumE
-__ZN10tensorflow8OpKernelC2EPNS_20OpKernelConstructionE
-__ZN10tensorflow8OpKernelD2Ev
-__ZN10tensorflow8internal10LogMessage16VmoduleActivatedEPKci
-__ZN10tensorflow8internal10LogMessageC1EPKcii
-__ZN10tensorflow8internal10LogMessageD1Ev
-__ZN10tensorflow8internal15LogMessageFatalC1EPKci
-__ZN10tensorflow8internal15LogMessageFatalD1Ev
-__ZN10tensorflow8internal21CheckOpMessageBuilder7ForVar2Ev
-__ZN10tensorflow8internal21CheckOpMessageBuilder9NewStringEv
-__ZN10tensorflow8internal21CheckOpMessageBuilderC1EPKc
-__ZN10tensorflow8internal21CheckOpMessageBuilderD1Ev
-__ZNK10tensorflow11TensorShape10IsSameSizeERKS0_
-__ZNK10tensorflow15OpKernelContext5inputEi
-__ZNK10tensorflow15TensorShapeBaseINS_11TensorShapeEE8dim_sizeEi
-__ZNK10tensorflow6Tensor21CheckTypeAndIsAlignedENS_8DataTypeE
-__ZNK10tensorflow6Tensor30CheckIsAlignedAndSingleElementEv
-__ZNK10tensorflow6Tensor9CheckTypeENS_8DataTypeE
-__ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb
-__ZNKSt3__120__vector_base_commonILb1EE20__throw_length_errorEv
-__ZNKSt3__120__vector_base_commonILb1EE20__throw_out_of_rangeEv
-__ZNKSt3__121__basic_string_commonILb1EE20__throw_length_errorEv
-__ZNKSt3__16locale9use_facetERNS0_2idE
-__ZNKSt3__18ios_base6getlocEv
-__ZNSt11logic_errorC2EPKc
-__ZNSt12length_errorD1Ev
-__ZNSt3__112__next_primeEm
-__ZNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEE6resizeEmc
-__ZNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEE9push_backEc
-__ZNSt3__113basic_istreamIcNS_11char_traitsIcEEED0Ev
-__ZNSt3__113basic_istreamIcNS_11char_traitsIcEEED1Ev
-__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEE6sentryC1ERS3_
-__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEE6sentryD1Ev
-__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEED0Ev
-__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEED1Ev
-__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEElsEf
-__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEElsEi
-__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEElsEm
-__ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEElsEx
-__ZNSt3__114basic_iostreamIcNS_11char_traitsIcEEED0Ev
-__ZNSt3__114basic_iostreamIcNS_11char_traitsIcEEED1Ev
-__ZNSt3__114basic_iostreamIcNS_11char_traitsIcEEED2Ev
-__ZNSt3__115basic_streambufIcNS_11char_traitsIcEEE4syncEv
-__ZNSt3__115basic_streambufIcNS_11char_traitsIcEEE5imbueERKNS_6localeE
-__ZNSt3__115basic_streambufIcNS_11char_traitsIcEEE5uflowEv
-__ZNSt3__115basic_streambufIcNS_11char_traitsIcEEE6setbufEPcl
-__ZNSt3__115basic_streambufIcNS_11char_traitsIcEEE6xsgetnEPcl
-__ZNSt3__115basic_streambufIcNS_11char_traitsIcEEE6xsputnEPKcl
-__ZNSt3__115basic_streambufIcNS_11char_traitsIcEEE9showmanycEv
-__ZNSt3__115basic_streambufIcNS_11char_traitsIcEEEC2Ev
-__ZNSt3__115basic_streambufIcNS_11char_traitsIcEEED2Ev
-__ZNSt3__15ctypeIcE2idE
-__ZNSt3__16localeD1Ev
-__ZNSt3__18ios_base33__set_badbit_and_consider_rethrowEv
-__ZNSt3__18ios_base4initEPv
-__ZNSt3__18ios_base5clearEj
-__ZNSt3__19basic_iosIcNS_11char_traitsIcEEED2Ev
-__ZNSt9bad_allocC1Ev
-__ZNSt9bad_allocD1Ev
-__ZSt9terminatev
-__ZTIN10tensorflow8OpKernelE
-__ZTINSt3__113basic_istreamIcNS_11char_traitsIcEEEE
-__ZTINSt3__113basic_ostreamIcNS_11char_traitsIcEEEE
-__ZTINSt3__114basic_iostreamIcNS_11char_traitsIcEEEE
-__ZTINSt3__115basic_streambufIcNS_11char_traitsIcEEEE
-__ZTISt12length_error
-__ZTISt9bad_alloc
-__ZTVN10__cxxabiv117__class_type_infoE
-__ZTVN10__cxxabiv120__si_class_type_infoE
-__ZTVN10tensorflow14kernel_factory17OpKernelRegistrar18PtrOpKernelFactoryE
-__ZTVSt12length_error
-__ZThn16_NSt3__114basic_iostreamIcNS_11char_traitsIcEEED0Ev
-__ZThn16_NSt3__114basic_iostreamIcNS_11char_traitsIcEEED1Ev
-__ZTv0_n24_NSt3__113basic_istreamIcNS_11char_traitsIcEEED0Ev
-__ZTv0_n24_NSt3__113basic_istreamIcNS_11char_traitsIcEEED1Ev
-__ZTv0_n24_NSt3__113basic_ostreamIcNS_11char_traitsIcEEED0Ev
-__ZTv0_n24_NSt3__113basic_ostreamIcNS_11char_traitsIcEEED1Ev
-__ZTv0_n24_NSt3__114basic_iostreamIcNS_11char_traitsIcEEED0Ev
-__ZTv0_n24_NSt3__114basic_iostreamIcNS_11char_traitsIcEEED1Ev
-___assert_rtn
-___bzero
-___cxa_allocate_exception
-___cxa_begin_catch
-___cxa_end_catch
-___cxa_free_exception
-___cxa_guard_abort
-___cxa_guard_acquire
-___cxa_guard_release
-___cxa_throw
-___gxx_personality_v0
-___stack_chk_fail
-___stack_chk_guard
-dyld_stub_binder
-__ZNSt3__1lsIN10tensorflow8internal15LogMessageFatalENS_12basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEEEEENS_9enable_ifIXaantsr19is_lvalue_referenceIT_EE5valuesr10is_base_ofINS_8ios_baseESB_EE5valueEOSB_E4typeESD_RKT0_
-___clang_call_terminate
-__ZZNK3$_0clEPKN10tensorflow9KernelDefEENUlPNS0_20OpKernelConstructionEE_8__invokeES5_
-__ZN20PoolingBySlotsGradOpD1Ev
-__ZN13GetSlotFidsOpD1Ev
-__ZN14GroupBySlotsOpD1Ev
-__ZN6IsInOpIiED1Ev
-__ZN6IsInOpIxED1Ev
-__ZN18SplitRaggedBlockOpIfED1Ev
-__ZN18SplitRaggedBlockOpIiED1Ev
-__ZN18SplitRaggedBlockOpIxED1Ev
-__ZN16PoolingBySlotsOpD1Ev
-__ZN20PoolingBySlotsGradOpD0Ev
-__ZN13GetSlotFidsOpD0Ev
-__ZN14GroupBySlotsOpD0Ev
-__ZN6IsInOpIiED0Ev
-__ZN6IsInOpIxED0Ev
-__ZN18SplitRaggedBlockOpIfED0Ev
-__ZN18SplitRaggedBlockOpIiED0Ev
-__ZN18SplitRaggedBlockOpIxED0Ev
-__ZN16PoolingBySlotsOpD0Ev
-__ZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextE
-__ZNK10tensorflow8OpKernel12const_tensorEv
-__ZN10tensorflow8OpKernel7AsAsyncEv
-__ZN10tensorflow8OpKernel11IsExpensiveEv
-__ZN10tensorflow6errors15InvalidArgumentIJPKcEEENS_6StatusEDpT_
-__ZNK10tensorflow6Tensor6shapedIiLm2EEENS_6TTypesIT_XT0_ElE11ConstTensorEN4absl14lts_2020_09_234SpanIKxEE
-__ZNK10tensorflow6Tensor6shapedIfLm2EEENS_6TTypesIT_XT0_ElE11ConstTensorEN4absl14lts_2020_09_234SpanIKxEE
-__ZN10tensorflow6errors8internal16PrepareForStrCatIPKcEENSt3__19enable_ifIXntsr3std14is_convertibleIT_NS_7strings8AlphaNumEEE5valueENS5_12basic_stringIcNS5_11char_traitsIcEENS5_9allocatorIcEEEEE4typeERKS7_
-__ZN10tensorflow6StatusC1ENS_5error4CodeEN4absl14lts_2020_09_2311string_viewE
-__ZNSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEED1Ev
-__ZNSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEED0Ev
-__ZThn16_NSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEED1Ev
-__ZThn16_NSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEED0Ev
-__ZTv0_n24_NSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEED1Ev
-__ZTv0_n24_NSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEED0Ev
-__ZNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEED1Ev
-__ZNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEED0Ev
-__ZNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEE7seekoffExNS_8ios_base7seekdirEj
-__ZNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEE7seekposENS_4fposI11__mbstate_tEEj
-__ZNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEE9underflowEv
-__ZNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEE9pbackfailEi
-__ZNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEE8overflowEi
-__ZNSt3__124__put_character_sequenceIcNS_11char_traitsIcEEEERNS_13basic_ostreamIT_T0_EES7_PKS4_m
-__ZNSt3__116__pad_and_outputIcNS_11char_traitsIcEEEENS_19ostreambuf_iteratorIT_T0_EES6_PKS4_S8_S8_RNS_8ios_baseES4_
-__ZNSt3__1L20__throw_length_errorEPKc
-__ZNSt12length_errorC1EPKc
-__ZNKSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEE3strEv
-__ZN10tensorflow6Status5StateD2Ev
-__ZNSt3__1lsIN10tensorflow8internal15LogMessageFatalEA27_cEENS_9enable_ifIXaantsr19is_lvalue_referenceIT_EE5valuesr10is_base_ofINS_8ios_baseES6_EE5valueEOS6_E4typeES8_RKT0_
-__ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm2EEEvN4absl14lts_2020_09_234SpanIKxEEPNSt3__15arrayIlXT_EEE
-__ZN10tensorflow8internal17MakeCheckOpStringImmEEPNSt3__112basic_stringIcNS2_11char_traitsIcEENS2_9allocatorIcEEEERKT_RKT0_PKc
-__ZN10tensorflow8internal17MakeCheckOpStringIxxEEPNSt3__112basic_stringIcNS2_11char_traitsIcEENS2_9allocatorIcEEEERKT_RKT0_PKc
-__ZNK10tensorflow6Tensor6shapedIiLm1EEENS_6TTypesIT_XT0_ElE11ConstTensorEN4absl14lts_2020_09_234SpanIKxEE
-__ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm1EEEvN4absl14lts_2020_09_234SpanIKxEEPNSt3__15arrayIlXT_EEE
-__ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm3EEEvN4absl14lts_2020_09_234SpanIKxEEPNSt3__15arrayIlXT_EEE
-__ZNSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE7destroyEv
-__ZNSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEED1Ev
-__ZNSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE7destroyEv
-__ZNSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEED1Ev
-__ZNSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE7destroyEv
-__ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEED1Ev
-__ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE7destroyEv
-__ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEED1Ev
-__ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE7destroyEv
-__ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEED1Ev
-__ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE7destroyEv
-__ZNSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEED1Ev
-__ZNSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE18destroy_deallocateEv
-__ZNSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEED0Ev
-__ZNSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE18destroy_deallocateEv
-__ZNSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEED0Ev
-__ZNSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE18destroy_deallocateEv
-__ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEED0Ev
-__ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE18destroy_deallocateEv
-__ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEED0Ev
-__ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE18destroy_deallocateEv
-__ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEED0Ev
-__ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE18destroy_deallocateEv
-__ZNSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEED0Ev
-__ZNKSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE7__cloneEv
-__ZNKSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE7__cloneEPNS0_6__baseIS9_EE
-__ZNSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEclEOxSB_
-__ZNKSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE6targetERKSt9type_info
-__ZNKSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE11target_typeEv
-__ZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExx
-__ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS3_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKSA_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSI_EEEEKNS3_ILln1EKNS4_INS5_ISI_Li2ELi1ElEELi16ES7_EEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE0EE3runERSV_RKSW_
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERS9_RKSA_
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE8coeffRefEl
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5coeffEl
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl
-__ZZNK3$_1clEPKN10tensorflow9KernelDefEENUlPNS0_20OpKernelConstructionEE_8__invokeES5_
-__ZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextE
-__ZNK10tensorflow6Tensor6shapedIfLm3EEENS_6TTypesIT_XT0_ElE11ConstTensorEN4absl14lts_2020_09_234SpanIKxEE
-__ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKS9_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSH_EEEEKNS3_ILln1EKNS3_ILln1EKNS4_INS5_ISH_Li3ELi1ElEELi16ES7_EEEEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE1EE3runERSW_RKSX_
-__ZNK5Eigen15TensorEvaluatorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEEKNS_19TensorCwiseBinaryOpINS_8internal13scalar_sum_opIffEEKS8_KNS_18TensorCwiseUnaryOpINSA_10bind1st_opINSA_17scalar_product_opIKfSH_EEEEKNS2_ILln1EKNS2_ILln1EKNS3_INS4_ISH_Li3ELi1ElEELi16ES6_EEEEEEEEEEEENS_13DefaultDeviceEE23getResourceRequirementsEv
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERSC_RKSD_
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_
-__ZNK5Eigen15TensorEvaluatorIKNS_19TensorCwiseBinaryOpINS_8internal13scalar_sum_opIffEEKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEEKNS_18TensorCwiseUnaryOpINS2_10bind1st_opINS2_17scalar_product_opIKfSG_EEEEKNS5_ILln1EKNS5_ILln1EKNS6_INS7_ISG_Li3ELi1ElEELi16ES9_EEEEEEEEEENS_13DefaultDeviceEE23getResourceRequirementsEv
-__ZN5Eigen8internal15queryCacheSizesERiS1_S1_
-__ZN5Eigen8internal27queryCacheSizes_intel_codesERiS1_S1_
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE23getResourceRequirementsEv
-__ZN5Eigen8internal17TensorBlockMapperILi1ELi1ElE25InitializeBlockDimensionsEv
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE10writeBlockINS_8internal22TensorCwiseBinaryBlockINSB_13scalar_sum_opIffEENSB_23TensorMaterializedBlockIfLi1ELi1ElEENSB_21TensorCwiseUnaryBlockINSB_10bind1st_opINSB_17scalar_product_opIKfSK_EEEESG_EEEEEEvRKNSB_21TensorBlockDescriptorILi1ElEERKT_
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSB_27TensorBlockScratchAllocatorIS9_EEb
-__ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_9TensorMapIKNS_6TensorIfLi2ELi1ElEELi0ENS_11MakePointerEEElE3RunERKNS8_6TargetERKS7_
-__ZN5Eigen8internal23TensorMaterializedBlockIfLi2ELi1ElE11materializeINS_6DSizesIlLi2EEENS0_27TensorBlockScratchAllocatorINS_13DefaultDeviceEEEEES2_PKfRKT_RNS0_21TensorBlockDescriptorILi2ElEERT0_
-__ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEE8allocateEm
-__ZNSt3__16vectorIN5Eigen8internal27TensorBlockScratchAllocatorINS1_13DefaultDeviceEE10AllocationENS_9allocatorIS6_EEE21__push_back_slow_pathIRKS6_EEvOT_
-__ZN5Eigen8internal13TensorBlockIOIflLi2ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi2EEE
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSF_27TensorBlockScratchAllocatorISD_EEb
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi2ElEERNSD_27TensorBlockScratchAllocatorISB_EEb
-__ZN5Eigen8internal21TensorBlockAssignmentIfLi3ENS_9TensorMapIKNS_6TensorIfLi3ELi1ElEELi0ENS_11MakePointerEEElE3RunERKNS8_6TargetERKS7_
-__ZN5Eigen8internal23TensorMaterializedBlockIfLi3ELi1ElE11materializeINS_6DSizesIlLi3EEENS0_27TensorBlockScratchAllocatorINS_13DefaultDeviceEEEEES2_PKfRKT_RNS0_21TensorBlockDescriptorILi3ElEERT0_
-__ZN5Eigen8internal13TensorBlockIOIflLi3ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi3EEE
-__ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_17TensorReshapingOpIKNS_6DSizesIlLi2EEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKNS_9TensorMapIKNS_6TensorIfLi1ELi1ElEELi0ENS_11MakePointerEEEKNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSJ_EEEESF_EEEEEElE3RunERKNSR_6TargetERKSQ_
-__GLOBAL__sub_I_feature_pooling.cc
-__ZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextE
-__ZNKSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE7__cloneEv
-__ZNKSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE7__cloneEPNS0_6__baseIS9_EE
-__ZNSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEclEOxSB_
-__ZNKSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE6targetERKSt9type_info
-__ZNKSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE11target_typeEv
-__GLOBAL__sub_I_get_slot_fids.cc
-__ZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextE
-__ZNK10tensorflow6Tensor6shapedIxLm2EEENS_6TTypesIT_XT0_ElE11ConstTensorEN4absl14lts_2020_09_234SpanIKxEE
-__ZNKSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE7__cloneEv
-__ZNKSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE7__cloneEPNS0_6__baseIS9_EE
-__ZNSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEclEOxSB_
-__ZNKSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE6targetERKSt9type_info
-__ZNKSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE11target_typeEv
-__ZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExx
-__ZN14GroupBySlotsOp12process_slotEiR7FidIteriRiS2_RN5Eigen9TensorMapINS3_6TensorIxLi2ELi1ElEELi16ENS3_11MakePointerEEERNS4_INS5_IfLi2ELi1ElEELi16ES7_EE
-__ZN7FidIter7advanceEv
-__GLOBAL__sub_I_group_by_slots.cc
-__ZN6IsInOpIiE7ComputeEPN10tensorflow15OpKernelContextE
-__ZNSt3__112__hash_tableIiNS_4hashIiEENS_8equal_toIiEENS_9allocatorIiEEE6rehashEm
-__ZNSt3__112__hash_tableIiNS_4hashIiEENS_8equal_toIiEENS_9allocatorIiEEE8__rehashEm
-__ZN6IsInOpIxE7ComputeEPN10tensorflow15OpKernelContextE
-__ZNK10tensorflow6Tensor6shapedIxLm1EEENS_6TTypesIT_XT0_ElE11ConstTensorEN4absl14lts_2020_09_234SpanIKxEE
-__ZNSt3__112__hash_tableIxNS_4hashIxEENS_8equal_toIxEENS_9allocatorIxEEE6rehashEm
-__ZNSt3__112__hash_tableIxNS_4hashIxEENS_8equal_toIxEENS_9allocatorIxEEE8__rehashEm
-__GLOBAL__sub_I_is_in.cc
-__ZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextE
-__ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE7__cloneEv
-__ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE7__cloneEPNS0_6__baseISA_EE
-__ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEclEOxSC_
-__ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE6targetERKSt9type_info
-__ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE11target_typeEv
-__ZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExx
-__ZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextE
-__ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE7__cloneEv
-__ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE7__cloneEPNS0_6__baseISA_EE
-__ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEclEOxSC_
-__ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE6targetERKSt9type_info
-__ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE11target_typeEv
-__ZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExx
-__ZZNK3$_2clEPKN10tensorflow9KernelDefEENUlPNS0_20OpKernelConstructionEE_8__invokeES5_
-__ZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextE
-__ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE7__cloneEv
-__ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE7__cloneEPNS0_6__baseISA_EE
-__ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEclEOxSC_
-__ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE6targetERKSt9type_info
-__ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE11target_typeEv
-__ZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExx
-__GLOBAL__sub_I_split_ragged_block.cc
-__ZN10tensorflow11register_op19OpDefBuilderWrapper10SetShapeFnENSt3__18functionIFNS_6StatusEPNS_15shape_inference16InferenceContextEEEE
-__ZN10tensorflow8internal17MakeCheckOpStringIiiEEPNSt3__112basic_stringIcNS2_11char_traitsIcEENS2_9allocatorIcEEEERKT_RKT0_PKc
-__ZN10tensorflow11register_op19OpDefBuilderWrapperC2EPKc
-__ZN10tensorflow12OpDefBuilderD2Ev
-__ZNSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED1Ev
-__ZNSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED0Ev
-__ZNKSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEv
-__ZNKSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEPNS0_6__baseISA_EE
-__ZNSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7destroyEv
-__ZNSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE18destroy_deallocateEv
-__ZNSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEclEOS9_
-__ZNKSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE6targetERKSt9type_info
-__ZNKSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE11target_typeEv
-__ZNSt3__1lsIN10tensorflow8internal15LogMessageFatalExEENS_9enable_ifIXaantsr19is_lvalue_referenceIT_EE5valuesr10is_base_ofINS_8ios_baseES5_EE5valueEOS5_E4typeES7_RKT0_
-__ZNSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED1Ev
-__ZNSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED0Ev
-__ZNKSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEv
-__ZNKSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEPNS0_6__baseISA_EE
-__ZNSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7destroyEv
-__ZNSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE18destroy_deallocateEv
-__ZNSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEclEOS9_
-__ZNKSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE6targetERKSt9type_info
-__ZNKSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE11target_typeEv
-__ZN10tensorflow15shape_inference16InferenceContext3DimENS0_11ShapeHandleEx
-__ZN10tensorflow15shape_inference16InferenceContext12DimKnownRankENS0_11ShapeHandleEx
-__ZNSt3__1lsIN10tensorflow8internal15LogMessageFatalEA43_cEENS_9enable_ifIXaantsr19is_lvalue_referenceIT_EE5valuesr10is_base_ofINS_8ios_baseES6_EE5valueEOS6_E4typeES8_RKT0_
-__ZNSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED1Ev
-__ZNSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED0Ev
-__ZNKSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEv
-__ZNKSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEPNS0_6__baseISA_EE
-__ZNSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7destroyEv
-__ZNSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE18destroy_deallocateEv
-__ZNSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEclEOS9_
-__ZNKSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE6targetERKSt9type_info
-__ZNKSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE11target_typeEv
-__ZNSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED1Ev
-__ZNSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED0Ev
-__ZNKSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEv
-__ZNKSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEPNS0_6__baseISA_EE
-__ZNSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7destroyEv
-__ZNSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE18destroy_deallocateEv
-__ZNSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEclEOS9_
-__ZNKSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE6targetERKSt9type_info
-__ZNKSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE11target_typeEv
-__ZNSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED1Ev
-__ZNSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED0Ev
-__ZNKSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEv
-__ZNKSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEPNS0_6__baseISA_EE
-__ZNSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7destroyEv
-__ZNSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE18destroy_deallocateEv
-__ZNSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEclEOS9_
-__ZNKSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE6targetERKSt9type_info
-__ZNKSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE11target_typeEv
-__ZNSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED1Ev
-__ZNSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED0Ev
-__ZNKSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEv
-__ZNKSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEPNS0_6__baseISA_EE
-__ZNSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7destroyEv
-__ZNSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE18destroy_deallocateEv
-__ZNSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEclEOS9_
-__ZNKSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE6targetERKSt9type_info
-__ZNKSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE11target_typeEv
-__GLOBAL__sub_I_reco_ops.cc
-__ZN10tensorflow6StatusC1ENS_5error4CodeEN4absl14lts_2020_09_2311string_viewE.cold.1
-__ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS3_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKSA_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSI_EEEEKNS3_ILln1EKNS4_INS5_ISI_Li2ELi1ElEELi16ES7_EEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE0EE3runERSV_RKSW_.cold.1
-__ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS3_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKSA_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSI_EEEEKNS3_ILln1EKNS4_INS5_ISI_Li2ELi1ElEELi16ES7_EEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE0EE3runERSV_RKSW_.cold.2
-__ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS3_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKSA_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSI_EEEEKNS3_ILln1EKNS4_INS5_ISI_Li2ELi1ElEELi16ES7_EEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE0EE3runERSV_RKSW_.cold.3
-__ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS3_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKSA_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSI_EEEEKNS3_ILln1EKNS4_INS5_ISI_Li2ELi1ElEELi16ES7_EEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE0EE3runERSV_RKSW_.cold.4
-__ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS3_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKSA_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSI_EEEEKNS3_ILln1EKNS4_INS5_ISI_Li2ELi1ElEELi16ES7_EEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE0EE3runERSV_RKSW_.cold.5
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERS9_RKSA_.cold.1
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERS9_RKSA_.cold.2
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERS9_RKSA_.cold.3
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_.cold.1
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_.cold.2
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_.cold.3
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_.cold.1
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_.cold.2
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_.cold.3
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f.cold.1
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f.cold.2
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f.cold.3
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f.cold.4
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f.cold.5
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f.cold.1
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f.cold.2
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f.cold.3
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f.cold.4
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f.cold.5
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE8coeffRefEl.cold.1
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE8coeffRefEl.cold.2
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE8coeffRefEl.cold.3
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE8coeffRefEl.cold.4
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE8coeffRefEl.cold.5
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.1
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.2
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.3
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.4
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.5
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.6
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.1
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.2
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.3
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.4
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.5
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5coeffEl.cold.1
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5coeffEl.cold.2
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5coeffEl.cold.3
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5coeffEl.cold.4
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5coeffEl.cold.5
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.1
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.2
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.3
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.4
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.5
-__ZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextE.cold.1
-__ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKS9_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSH_EEEEKNS3_ILln1EKNS3_ILln1EKNS4_INS5_ISH_Li3ELi1ElEELi16ES7_EEEEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE1EE3runERSW_RKSX_.cold.1
-__ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKS9_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSH_EEEEKNS3_ILln1EKNS3_ILln1EKNS4_INS5_ISH_Li3ELi1ElEELi16ES7_EEEEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE1EE3runERSW_RKSX_.cold.2
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_.cold.1
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_.cold.2
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_.cold.3
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERSC_RKSD_.cold.1
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERSC_RKSD_.cold.2
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERSC_RKSD_.cold.3
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_.cold.1
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_.cold.2
-__ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_.cold.3
-__ZN5Eigen8internal17TensorBlockMapperILi1ELi1ElE25InitializeBlockDimensionsEv.cold.1
-__ZN5Eigen8internal17TensorBlockMapperILi1ELi1ElE25InitializeBlockDimensionsEv.cold.2
-__ZN5Eigen8internal17TensorBlockMapperILi1ELi1ElE25InitializeBlockDimensionsEv.cold.3
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE10writeBlockINS_8internal22TensorCwiseBinaryBlockINSB_13scalar_sum_opIffEENSB_23TensorMaterializedBlockIfLi1ELi1ElEENSB_21TensorCwiseUnaryBlockINSB_10bind1st_opINSB_17scalar_product_opIKfSK_EEEESG_EEEEEEvRKNSB_21TensorBlockDescriptorILi1ElEERKT_.cold.1
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE10writeBlockINS_8internal22TensorCwiseBinaryBlockINSB_13scalar_sum_opIffEENSB_23TensorMaterializedBlockIfLi1ELi1ElEENSB_21TensorCwiseUnaryBlockINSB_10bind1st_opINSB_17scalar_product_opIKfSK_EEEESG_EEEEEEvRKNSB_21TensorBlockDescriptorILi1ElEERKT_.cold.2
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE10writeBlockINS_8internal22TensorCwiseBinaryBlockINSB_13scalar_sum_opIffEENSB_23TensorMaterializedBlockIfLi1ELi1ElEENSB_21TensorCwiseUnaryBlockINSB_10bind1st_opINSB_17scalar_product_opIKfSK_EEEESG_EEEEEEvRKNSB_21TensorBlockDescriptorILi1ElEERKT_.cold.3
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE10writeBlockINS_8internal22TensorCwiseBinaryBlockINSB_13scalar_sum_opIffEENSB_23TensorMaterializedBlockIfLi1ELi1ElEENSB_21TensorCwiseUnaryBlockINSB_10bind1st_opINSB_17scalar_product_opIKfSK_EEEESG_EEEEEEvRKNSB_21TensorBlockDescriptorILi1ElEERKT_.cold.4
-__ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE10writeBlockINS_8internal22TensorCwiseBinaryBlockINSB_13scalar_sum_opIffEENSB_23TensorMaterializedBlockIfLi1ELi1ElEENSB_21TensorCwiseUnaryBlockINSB_10bind1st_opINSB_17scalar_product_opIKfSK_EEEESG_EEEEEEvRKNSB_21TensorBlockDescriptorILi1ElEERKT_.cold.5
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSB_27TensorBlockScratchAllocatorIS9_EEb.cold.1
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSB_27TensorBlockScratchAllocatorIS9_EEb.cold.2
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSB_27TensorBlockScratchAllocatorIS9_EEb.cold.3
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSB_27TensorBlockScratchAllocatorIS9_EEb.cold.4
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSB_27TensorBlockScratchAllocatorIS9_EEb.cold.5
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSB_27TensorBlockScratchAllocatorIS9_EEb.cold.6
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSB_27TensorBlockScratchAllocatorIS9_EEb.cold.7
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSB_27TensorBlockScratchAllocatorIS9_EEb.cold.8
-__ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_9TensorMapIKNS_6TensorIfLi2ELi1ElEELi0ENS_11MakePointerEEElE3RunERKNS8_6TargetERKS7_.cold.1
-__ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_9TensorMapIKNS_6TensorIfLi2ELi1ElEELi0ENS_11MakePointerEEElE3RunERKNS8_6TargetERKS7_.cold.2
-__ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_9TensorMapIKNS_6TensorIfLi2ELi1ElEELi0ENS_11MakePointerEEElE3RunERKNS8_6TargetERKS7_.cold.3
-__ZN5Eigen8internal23TensorMaterializedBlockIfLi2ELi1ElE11materializeINS_6DSizesIlLi2EEENS0_27TensorBlockScratchAllocatorINS_13DefaultDeviceEEEEES2_PKfRKT_RNS0_21TensorBlockDescriptorILi2ElEERT0_.cold.1
-__ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEE8allocateEm.cold.1
-__ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEE8allocateEm.cold.2
-__ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEE8allocateEm.cold.3
-__ZN5Eigen8internal13TensorBlockIOIflLi2ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi2EEE.cold.1
-__ZN5Eigen8internal13TensorBlockIOIflLi2ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi2EEE.cold.2
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSF_27TensorBlockScratchAllocatorISD_EEb.cold.1
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSF_27TensorBlockScratchAllocatorISD_EEb.cold.2
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSF_27TensorBlockScratchAllocatorISD_EEb.cold.3
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSF_27TensorBlockScratchAllocatorISD_EEb.cold.4
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSF_27TensorBlockScratchAllocatorISD_EEb.cold.5
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSF_27TensorBlockScratchAllocatorISD_EEb.cold.6
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSF_27TensorBlockScratchAllocatorISD_EEb.cold.7
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi2ElEERNSD_27TensorBlockScratchAllocatorISB_EEb.cold.1
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi2ElEERNSD_27TensorBlockScratchAllocatorISB_EEb.cold.2
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi2ElEERNSD_27TensorBlockScratchAllocatorISB_EEb.cold.3
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi2ElEERNSD_27TensorBlockScratchAllocatorISB_EEb.cold.4
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi2ElEERNSD_27TensorBlockScratchAllocatorISB_EEb.cold.5
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi2ElEERNSD_27TensorBlockScratchAllocatorISB_EEb.cold.6
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi2ElEERNSD_27TensorBlockScratchAllocatorISB_EEb.cold.7
-__ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi2ElEERNSD_27TensorBlockScratchAllocatorISB_EEb.cold.8
-__ZN5Eigen8internal21TensorBlockAssignmentIfLi3ENS_9TensorMapIKNS_6TensorIfLi3ELi1ElEELi0ENS_11MakePointerEEElE3RunERKNS8_6TargetERKS7_.cold.1
-__ZN5Eigen8internal21TensorBlockAssignmentIfLi3ENS_9TensorMapIKNS_6TensorIfLi3ELi1ElEELi0ENS_11MakePointerEEElE3RunERKNS8_6TargetERKS7_.cold.2
-__ZN5Eigen8internal21TensorBlockAssignmentIfLi3ENS_9TensorMapIKNS_6TensorIfLi3ELi1ElEELi0ENS_11MakePointerEEElE3RunERKNS8_6TargetERKS7_.cold.3
-__ZN5Eigen8internal23TensorMaterializedBlockIfLi3ELi1ElE11materializeINS_6DSizesIlLi3EEENS0_27TensorBlockScratchAllocatorINS_13DefaultDeviceEEEEES2_PKfRKT_RNS0_21TensorBlockDescriptorILi3ElEERT0_.cold.1
-__ZN5Eigen8internal13TensorBlockIOIflLi3ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi3EEE.cold.1
-__ZN5Eigen8internal13TensorBlockIOIflLi3ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi3EEE.cold.2
-__ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_17TensorReshapingOpIKNS_6DSizesIlLi2EEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKNS_9TensorMapIKNS_6TensorIfLi1ELi1ElEELi0ENS_11MakePointerEEEKNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSJ_EEEESF_EEEEEElE3RunERKNSR_6TargetERKSQ_.cold.1
-__ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_17TensorReshapingOpIKNS_6DSizesIlLi2EEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKNS_9TensorMapIKNS_6TensorIfLi1ELi1ElEELi0ENS_11MakePointerEEEKNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSJ_EEEESF_EEEEEElE3RunERKNSR_6TargetERKSQ_.cold.2
-__ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_17TensorReshapingOpIKNS_6DSizesIlLi2EEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKNS_9TensorMapIKNS_6TensorIfLi1ELi1ElEELi0ENS_11MakePointerEEEKNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSJ_EEEESF_EEEEEElE3RunERKNSR_6TargetERKSQ_.cold.3
-__ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_17TensorReshapingOpIKNS_6DSizesIlLi2EEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKNS_9TensorMapIKNS_6TensorIfLi1ELi1ElEELi0ENS_11MakePointerEEEKNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSJ_EEEESF_EEEEEElE3RunERKNSR_6TargetERKSQ_.cold.4
-__ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_17TensorReshapingOpIKNS_6DSizesIlLi2EEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKNS_9TensorMapIKNS_6TensorIfLi1ELi1ElEELi0ENS_11MakePointerEEEKNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSJ_EEEESF_EEEEEElE3RunERKNSR_6TargetERKSQ_.cold.5
-__ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_17TensorReshapingOpIKNS_6DSizesIlLi2EEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKNS_9TensorMapIKNS_6TensorIfLi1ELi1ElEELi0ENS_11MakePointerEEEKNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSJ_EEEESF_EEEEEElE3RunERKNSR_6TargetERKSQ_.cold.6
-__ZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextE.cold.1
-__ZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextE.cold.2
-__ZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextE.cold.3
-__ZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextE.cold.1
-__ZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextE.cold.1
-__ZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextE.cold.1
-__ZN10tensorflow11register_op19OpDefBuilderWrapper10SetShapeFnENSt3__18functionIFNS_6StatusEPNS_15shape_inference16InferenceContextEEEE.cold.1
-GCC_except_table2
-GCC_except_table5
-GCC_except_table9
-GCC_except_table10
-GCC_except_table11
-GCC_except_table12
-GCC_except_table13
-GCC_except_table26
-GCC_except_table27
-GCC_except_table28
-GCC_except_table29
-GCC_except_table34
-GCC_except_table35
-GCC_except_table36
-GCC_except_table37
-GCC_except_table38
-GCC_except_table39
-GCC_except_table49
-GCC_except_table61
-GCC_except_table64
-GCC_except_table65
-GCC_except_table66
-GCC_except_table67
-GCC_except_table71
-GCC_except_table74
-GCC_except_table89
-GCC_except_table44
-GCC_except_table46
-GCC_except_table48
-GCC_except_table14
-GCC_except_table21
-GCC_except_table24
-GCC_except_table25
-GCC_except_table45
-GCC_except_table58
-GCC_except_table59
-GCC_except_table62
-GCC_except_table73
-GCC_except_table3
-GCC_except_table4
-GCC_except_table6
-GCC_except_table16
-GCC_except_table31
-GCC_except_table55
-GCC_except_table85
-__ZTSNSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-__ZTS3$_0
-__ZTSNSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-__ZTS3$_1
-__ZTSNSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-__ZTS3$_2
-__ZTSNSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-__ZTS3$_3
-__ZTSNSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-__ZTS3$_4
-__ZTSNSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-__ZTS3$_5
-__ZTV16PoolingBySlotsOp
-__ZTVNSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEEE
-__ZTTNSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEEE
-__ZTCNSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEEE0_NS_14basic_iostreamIcS2_EE
-__ZTCNSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEEE0_NS_13basic_istreamIcS2_EE
-__ZTCNSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEEE16_NS_13basic_ostreamIcS2_EE
-__ZTVNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEEE
-__ZTVNSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-__ZTV20PoolingBySlotsGradOp
-__ZTV13GetSlotFidsOp
-__ZTVNSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-__ZTV14GroupBySlotsOp
-__ZTVNSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE
-__ZTV6IsInOpIiE
-__ZTV6IsInOpIxE
-__ZTV18SplitRaggedBlockOpIfE
-__ZTVNSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-__ZTV18SplitRaggedBlockOpIiE
-__ZTVNSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-__ZTV18SplitRaggedBlockOpIxE
-__ZTVNSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE
-__ZTVNSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-__ZTINSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-__ZTI3$_0
-__ZTVNSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-__ZTINSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-__ZTI3$_1
-__ZTVNSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-__ZTINSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-__ZTI3$_2
-__ZTVNSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-__ZTINSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-__ZTI3$_3
-__ZTVNSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-__ZTINSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-__ZTI3$_4
-__ZTVNSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-__ZTINSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE
-__ZTI3$_5
-__dyld_private
-__ZN5EigenL4lastE
-__ZN5EigenL6lastp1E
-__ZN5EigenL3allE
-__ZL17register_kernel_0
-__ZL17register_kernel_1
-__ZL17register_kernel_2
-__ZL12register_op0
-__ZL12register_op1
-__ZL12register_op2
-__ZL12register_op3
-__ZL12register_op4
-__ZL12register_op5
-__ZZZNK3$_0clEPN10tensorflow15shape_inference16InferenceContextEENKUliPKcE_clEiS5_E17vmodule_activated
-__ZGVZZNK3$_0clEPN10tensorflow15shape_inference16InferenceContextEENKUliPKcE_clEiS5_E17vmodule_activated
+segment_ids: int32
+unique_fids: int64
+absl::lts_2020_09_23::string_view::CheckLengthInternal(absl::lts_2020_09_23::string_view::size_type)::<lambda()>
+*UlPN10tensorflow15shape_inference16InferenceContextEE_
+*UlPN10tensorflow15shape_inference16InferenceContextEE0_
+*UlPN10tensorflow15shape_inference16InferenceContextEE1_
+*UlPN10tensorflow15shape_inference16InferenceContextEE2_
+*UlPN10tensorflow15shape_inference16InferenceContextEE3_
+*UlPN10tensorflow15shape_inference16InferenceContextEE4_
+*UlPN10tensorflow15shape_inference16InferenceContextEE5_
+GCC: (Ubuntu 7.5.0-3ubuntu1~18.04) 7.5.0
+_ZNSs4_Rep10_M_disposeERKSaIcE.part.7
+_ZZNKUlPKN10tensorflow9KernelDefEE_clES2_ENUlPNS_20OpKernelConstructionEE_4_FUNES5_
+_ZZNKUlPKN10tensorflow9KernelDefEE0_clES2_ENUlPNS_20OpKernelConstructionEE_4_FUNES5_
+_ZN5Eigen15TensorEvaluatorINS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE8coeffRefEl.isra.118.part.119
+_ZZN5Eigen15TensorEvaluatorINS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE8coeffRefElE19__PRETTY_FUNCTION__
+_ZNK5Eigen8internal21TensorBlockDescriptorILi1ElE17DestinationBuffer4dataIfEEPT_v.isra.186.part.187
+_ZZNK5Eigen8internal21TensorBlockDescriptorILi1ElE17DestinationBuffer4dataIfEEPT_vE19__PRETTY_FUNCTION__
+_ZNK5Eigen15TensorEvaluatorINS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE5coeffEl.isra.206.part.207
+_ZZNK5Eigen15TensorEvaluatorINS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE5coeffElE19__PRETTY_FUNCTION__
+_ZNK5Eigen15TensorEvaluatorIKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE5coeffEl.isra.208.part.209
+_ZZNK5Eigen15TensorEvaluatorIKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE5coeffElE19__PRETTY_FUNCTION__
+_ZNK5Eigen8internal21TensorBlockDescriptorILi2ElE17DestinationBuffer4dataIfEEPT_v.isra.264.part.265
+_ZZNK5Eigen8internal21TensorBlockDescriptorILi2ElE17DestinationBuffer4dataIfEEPT_vE19__PRETTY_FUNCTION__
+_ZNK5Eigen15TensorEvaluatorIKNS_9TensorMapIKNS_6TensorIfLi1ELi1ElEELi0ENS_11MakePointerEEENS_13DefaultDeviceEE5coeffEl.isra.286.part.287
+_ZZNK5Eigen15TensorEvaluatorIKNS_9TensorMapIKNS_6TensorIfLi1ELi1ElEELi0ENS_11MakePointerEEENS_13DefaultDeviceEE5coeffElE19__PRETTY_FUNCTION__
+_ZNK5Eigen8internal21TensorBlockDescriptorILi3ElE17DestinationBuffer4dataIfEEPT_v.isra.301.part.302
+_ZZNK5Eigen8internal21TensorBlockDescriptorILi3ElE17DestinationBuffer4dataIfEEPT_vE19__PRETTY_FUNCTION__
+_ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE23getResourceRequirementsEv.isra.224
+_ZZZN4absl14lts_2020_09_2311string_view19CheckLengthInternalEmENKUlvE_clEvE19__PRETTY_FUNCTION__
+_ZZZNK4absl14lts_2020_09_234SpanIKlEixEmENKUlvE_clEvE19__PRETTY_FUNCTION__
+_ZZN5Eigen8internal11DimensionIdILln1EEC4ElE19__PRETTY_FUNCTION__
+_ZZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC4ERS8_RKS9_E19__PRETTY_FUNCTION__
+_ZZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC4ERSA_RKSB_E19__PRETTY_FUNCTION__
+_ZZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC4ERS8_RKS9_E19__PRETTY_FUNCTION__
+_ZZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC4ERS9_RKSA_E19__PRETTY_FUNCTION__
+_ZZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv8_flE19__PRETTY_FUNCTION__
+_ZZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv8_fE19__PRETTY_FUNCTION__
+_ZZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE8srcCoeffElE19__PRETTY_FUNCTION__
+_ZZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE6packetILi0EEEDv8_flE19__PRETTY_FUNCTION__
+_ZZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv8_fE19__PRETTY_FUNCTION__
+_ZZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE8srcCoeffElE19__PRETTY_FUNCTION__
+_ZZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv8_flE19__PRETTY_FUNCTION__
+_ZZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE8srcCoeffElE19__PRETTY_FUNCTION__
+_ZZN5Eigen15TensorEvaluatorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS2_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_19TensorCwiseBinaryOpINS_8internal13scalar_sum_opIffEEKS9_KNS_18TensorCwiseUnaryOpINSB_10bind1st_opINSB_17scalar_product_opIKfSI_EEEEKNS2_ILln1EKNS3_INS4_ISI_Li2ELi1ElEELi16ES6_EEEEEEEEEENS_13DefaultDeviceEE20evalSubExprsIfNeededEPfE19__PRETTY_FUNCTION__
+_ZZN5Eigen15TensorEvaluatorIKNS_19TensorCwiseBinaryOpINS_8internal13scalar_sum_opIffEEKNS_16TensorChippingOpILln1ENS5_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_18TensorCwiseUnaryOpINS2_10bind1st_opINS2_17scalar_product_opIKfSH_EEEEKNS5_ILln1EKNS6_INS7_ISH_Li2ELi1ElEELi16ES9_EEEEEEEENS_13DefaultDeviceEEC4ERSS_RKST_E19__PRETTY_FUNCTION__
+_ZZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC4ERSA_RKSB_E19__PRETTY_FUNCTION__
+_ZZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC4ERSC_RKSD_E19__PRETTY_FUNCTION__
+_ZZN5Eigen8internal13TensorBlockIOIflLi2ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi2EEEE19__PRETTY_FUNCTION__
+_ZZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEE8allocateEmE19__PRETTY_FUNCTION__
+_ZZN5Eigen8internal13TensorBlockIOIflLi3ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi3EEEE19__PRETTY_FUNCTION__
+_ZZNK5Eigen15TensorEvaluatorIKNS_9TensorMapIKNS_6TensorIfLi3ELi1ElEELi0ENS_11MakePointerEEENS_13DefaultDeviceEE5coeffElE19__PRETTY_FUNCTION__
+_ZZNK5Eigen15TensorEvaluatorIKNS_9TensorMapIKNS_6TensorIfLi2ELi1ElEELi0ENS_11MakePointerEEENS_13DefaultDeviceEE5coeffElE19__PRETTY_FUNCTION__
+_ZZNK5Eigen15TensorEvaluatorINS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi2ElEERNS8_27TensorBlockScratchAllocatorIS6_EEbE19__PRETTY_FUNCTION__
+_ZZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE10writeBlockINS_8internal22TensorCwiseBinaryBlockINSB_13scalar_sum_opIffEENSB_23TensorMaterializedBlockIfLi1ELi1ElEENSB_21TensorCwiseUnaryBlockINSB_10bind1st_opINSB_17scalar_product_opIKfSK_EEEESG_EEEEEEvRKNSB_21TensorBlockDescriptorILi1ElEERKT_E19__PRETTY_FUNCTION__
+_ZZNK5Eigen15TensorEvaluatorIKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi3ElEERNSA_27TensorBlockScratchAllocatorIS8_EEbE19__PRETTY_FUNCTION__
+_ZZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE8srcCoeffElE19__PRETTY_FUNCTION__
+_ZZN5Eigen15TensorEvaluatorIKNS_19TensorCwiseBinaryOpINS_8internal13scalar_sum_opIffEEKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEEKNS_18TensorCwiseUnaryOpINS2_10bind1st_opINS2_17scalar_product_opIKfSG_EEEEKNS5_ILln1EKNS5_ILln1EKNS6_INS7_ISG_Li3ELi1ElEELi16ES9_EEEEEEEEEENS_13DefaultDeviceEEC4ERST_RKSU_E19__PRETTY_FUNCTION__
+_ZZN5Eigen15TensorEvaluatorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEEKNS_19TensorCwiseBinaryOpINS_8internal13scalar_sum_opIffEEKS8_KNS_18TensorCwiseUnaryOpINSA_10bind1st_opINSA_17scalar_product_opIKfSH_EEEEKNS2_ILln1EKNS2_ILln1EKNS3_INS4_ISH_Li3ELi1ElEELi16ES6_EEEEEEEEEEEENS_13DefaultDeviceEE20evalSubExprsIfNeededEPfE19__PRETTY_FUNCTION__
+_ZZN5Eigen8internal21TensorBlockAssignmentIfLi3ENS_9TensorMapIKNS_6TensorIfLi3ELi1ElEELi0ENS_11MakePointerEEElE3RunERKNS8_6TargetERKS7_E19__PRETTY_FUNCTION__
+_ZZN5Eigen15TensorEvaluatorIKNS_17TensorReshapingOpIKNS_6DSizesIlLi2EEEKNS_19TensorCwiseBinaryOpINS_8internal13scalar_sum_opIffEEKNS_9TensorMapIKNS_6TensorIfLi1ELi1ElEELi0ENS_11MakePointerEEEKNS_18TensorCwiseUnaryOpINS6_10bind1st_opINS6_17scalar_product_opIKfSJ_EEEESF_EEEEEENS_13DefaultDeviceEEC4ERSR_RKSS_E19__PRETTY_FUNCTION__
+_ZZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE8srcCoeffElE19__PRETTY_FUNCTION__
+_ZZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE8srcCoeffElE19__PRETTY_FUNCTION__
+_ZZN5Eigen8internal17TensorBlockMapperILi1ELi1ElE25InitializeBlockDimensionsEvE19__PRETTY_FUNCTION__
+_GLOBAL__sub_I_feature_pooling.cc
+_ZStL8__ioinit
+_ZZN5Eigen15TensorEvaluatorINS_9TensorMapINS_6TensorIiLi2ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE8coeffRefElE19__PRETTY_FUNCTION__
+_ZZN5Eigen15TensorEvaluatorINS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE8coeffRefElE19__PRETTY_FUNCTION__
+_GLOBAL__sub_I_get_slot_fids.cc
+_ZZNKUlPKN10tensorflow9KernelDefEE1_clES2_ENUlPNS_20OpKernelConstructionEE_4_FUNES5_
+_GLOBAL__sub_I_split_ragged_block.cc
+_GLOBAL__sub_I_feature_vec_to_sparse.cc
+_ZZN5Eigen15TensorEvaluatorINS_9TensorMapINS_6TensorIiLi1ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE8coeffRefElE19__PRETTY_FUNCTION__
+_ZZN5Eigen15TensorEvaluatorINS_9TensorMapINS_6TensorIfLi1ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE8coeffRefElE19__PRETTY_FUNCTION__
+_GLOBAL__sub_I_group_by_slots.cc
+_ZZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_E9copy_fromERKSF_mE19__PRETTY_FUNCTION__
+_ZZNK6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_E12test_deletedERKNS_30dense_hashtable_const_iteratorIS3_lS6_SD_SE_S9_SB_EEE19__PRETTY_FUNCTION__
+_ZZNK6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_E10test_emptyEmE19__PRETTY_FUNCTION__
+_ZZNK6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_E10test_emptyERKNS_30dense_hashtable_const_iteratorIS3_lS6_SD_SE_S9_SB_EEE19__PRETTY_FUNCTION__
+_ZZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_E13clear_to_sizeEmE19__PRETTY_FUNCTION__
+_ZZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_EC4ERKSF_mE19__PRETTY_FUNCTION__
+_GLOBAL__sub_I_parse_feature_vec.cc
+_ZZNK6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_E13find_positionERS2_E19__PRETTY_FUNCTION__
+_ZZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_E15insert_noresizeERKS3_E19__PRETTY_FUNCTION__
+_ZZNK6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_E12test_deletedEmE19__PRETTY_FUNCTION__
+_ZZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_E12maybe_shrinkEvE19__PRETTY_FUNCTION__
+_ZZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_E13set_empty_keyERKS3_E19__PRETTY_FUNCTION__
+_GLOBAL__sub_I_is_in.cc
+_ZNSt14_Function_base13_Base_managerIUlPN10tensorflow15shape_inference16InferenceContextEE_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation
+_ZTIUlPN10tensorflow15shape_inference16InferenceContextEE_
+_ZNSt14_Function_base13_Base_managerIUlPN10tensorflow15shape_inference16InferenceContextEE0_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation
+_ZTIUlPN10tensorflow15shape_inference16InferenceContextEE0_
+_ZNSt14_Function_base13_Base_managerIUlPN10tensorflow15shape_inference16InferenceContextEE1_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation
+_ZTIUlPN10tensorflow15shape_inference16InferenceContextEE1_
+_ZNSt14_Function_base13_Base_managerIUlPN10tensorflow15shape_inference16InferenceContextEE2_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation
+_ZTIUlPN10tensorflow15shape_inference16InferenceContextEE2_
+_ZNSt14_Function_base13_Base_managerIUlPN10tensorflow15shape_inference16InferenceContextEE3_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation
+_ZTIUlPN10tensorflow15shape_inference16InferenceContextEE3_
+_ZNSt14_Function_base13_Base_managerIUlPN10tensorflow15shape_inference16InferenceContextEE4_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation
+_ZTIUlPN10tensorflow15shape_inference16InferenceContextEE4_
+_ZNSt14_Function_base13_Base_managerIUlPN10tensorflow15shape_inference16InferenceContextEE5_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation
+_ZTIUlPN10tensorflow15shape_inference16InferenceContextEE5_
+_ZNSs4_Rep10_M_disposeERKSaIcE.part.12
+_ZNSt17_Function_handlerIFN10tensorflow6StatusEPNS0_15shape_inference16InferenceContextEEUlS4_E2_E9_M_invokeERKSt9_Any_dataOS4_
+_ZNSt17_Function_handlerIFN10tensorflow6StatusEPNS0_15shape_inference16InferenceContextEEUlS4_E0_E9_M_invokeERKSt9_Any_dataOS4_
+_ZN10tensorflow15shape_inference19DimensionOrConstantC2El.part.112
+_ZN10tensorflow15shape_inference9DimensionC2El.part.113
+_ZNSt17_Function_handlerIFN10tensorflow6StatusEPNS0_15shape_inference16InferenceContextEEUlS4_E1_E9_M_invokeERKSt9_Any_dataOS4_
+_ZN10tensorflow15shape_inference19DimensionOrConstantC2ENS0_15DimensionHandleE.part.115
+_ZNSt17_Function_handlerIFN10tensorflow6StatusEPNS0_15shape_inference16InferenceContextEEUlS4_E3_E9_M_invokeERKSt9_Any_dataOS4_
+_ZNSt17_Function_handlerIFN10tensorflow6StatusEPNS0_15shape_inference16InferenceContextEEUlS4_E5_E9_M_invokeERKSt9_Any_dataOS4_
+_ZNSt17_Function_handlerIFN10tensorflow6StatusEPNS0_15shape_inference16InferenceContextEEUlS4_E4_E9_M_invokeERKSt9_Any_dataOS4_
+_ZNSt17_Function_handlerIFN10tensorflow6StatusEPNS0_15shape_inference16InferenceContextEEUlS4_E_E9_M_invokeERKSt9_Any_dataOS4_
+_Z41__static_initialization_and_destruction_0ii.constprop.120
+_GLOBAL__sub_I_reco_ops.cc
+_ZTSUlPN10tensorflow15shape_inference16InferenceContextEE_
+_ZTSUlPN10tensorflow15shape_inference16InferenceContextEE0_
+_ZTSUlPN10tensorflow15shape_inference16InferenceContextEE1_
+_ZTSUlPN10tensorflow15shape_inference16InferenceContextEE2_
+_ZTSUlPN10tensorflow15shape_inference16InferenceContextEE3_
+_ZTSUlPN10tensorflow15shape_inference16InferenceContextEE4_
+_ZTSUlPN10tensorflow15shape_inference16InferenceContextEE5_
+crtstuff.c
+deregister_tm_clones
+__do_global_dtors_aux
+completed.7698
+__do_global_dtors_aux_fini_array_entry
+frame_dummy
+__frame_dummy_init_array_entry
+__FRAME_END__
+__TMC_END__
+_GLOBAL_OFFSET_TABLE_
+_DYNAMIC
+__GNU_EH_FRAME_HDR
+__dso_handle
+DW.ref.__gxx_personality_v0
+_ZN10tensorflow5OpDefD1Ev
+_ZTS18SplitRaggedBlockOpIlE
+_ZNSt17_Function_handlerIFvllEZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_E9_M_invokeERKSt9_Any_dataOlSA_
+_ZN18SplitRaggedBlockOpIfED0Ev
+_ZN22FeatureVecToSegmentsOpD0Ev
+_ZNSt17_Function_handlerIFvllEZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_E9_M_invokeERKSt9_Any_dataOlSA_
+_ZN10tensorflow12OpDefBuilder10SetShapeFnESt8functionIFNS_6StatusEPNS_15shape_inference16InferenceContextEEE
+_ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
+_ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEE8allocateEm
+_ZN10tensorflow15shape_inference19DimensionOrConstantC1El
+_ZNSt12length_errorC1EPKc
+_ZTSZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_
+_ZNK10tensorflow15TensorShapeBaseINS_11TensorShapeEE8dim_sizeEi
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERSC_RKSD_
+_ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm2EEEvN4absl14lts_2020_09_234SpanIKlEEPSt5arrayIlXT_EE
+_ZSt19__throw_logic_errorPKc@@GLIBCXX_3.4
+_ZGVZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
+_ZN20PoolingBySlotsGradOpD0Ev
+_ZN10tensorflow15OpKernelContext10CtxFailureEPKciRKNS_6StatusE
+__cxa_begin_catch@@CXXABI_1.3
+_ZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEll
+memcpy@@GLIBC_2.14
+_ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
+_ZSt17__throw_bad_allocv@@GLIBCXX_3.4
+_ZN6IsInOpIiED1Ev
+_ZNSt9bad_allocD1Ev@@GLIBCXX_3.4
+_ZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextE
+_ZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEll
+_ZGVZZN17ParseFeatureVecOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZTV18SplitRaggedBlockOpIiE
+_ZZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated
+_ZNSt18basic_stringstreamIcSt11char_traitsIcESaIcEED1Ev@@GLIBCXX_3.4
+_ITM_deregisterTMCloneTable
+_ZN6IsInOpIlED1Ev
+_ZN17ParseFeatureVecOpD2Ev
+_ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
+_ZGVZZN22FeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKS9_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSH_EEEEKNS3_ILln1EKNS3_ILln1EKNS4_INS5_ISH_Li3ELi1ElEELi16ES7_EEEEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE1EE3runERSW_RKSX_
+_ZN5Eigen8internal19throw_std_bad_allocEv
+_ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
+_ZTS17ParseFeatureVecOp
+_ZN10tensorflow22CheckNotInComputeAsyncEPNS_15OpKernelContextEPKc
+_ZTI6IsInOpIlE
+_ZN10tensorflow4core10RefCountedD0Ev
+_ZN10tensorflow15shape_inference19DimensionOrConstantC1ENS0_15DimensionHandleE
+_Znwm@@GLIBCXX_3.4
+memmove@@GLIBC_2.2.5
+_ZN10tensorflow11register_op19OpDefBuilderWrapperclEv
+__assert_fail@@GLIBC_2.2.5
+_ZTS16PoolingBySlotsOp
+_ZN10tensorflow8internal10LogMessageC1EPKcii
+_ZN30UnsortedFeatureVecToSegmentsOpD1Ev
+_ZTI30UnsortedFeatureVecToSegmentsOp
+_ZTI6IsInOpIiE
+_ZN10tensorflow12OpDefBuilder4AttrESs
+free@@GLIBC_2.2.5
+_ZNK10tensorflow6Tensor9CheckTypeENS_8DataTypeE
+_ZTV14GroupBySlotsOp
+__cxa_finalize@@GLIBC_2.2.5
+_ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev
+_ZTVSt15basic_stringbufIcSt11char_traitsIcESaIcEE@@GLIBCXX_3.4
+_ZN10tensorflow6StatusC1ENS_5error4CodeEN4absl14lts_2020_09_2311string_viewEOSt6vectorINS_10StackFrameESaIS7_EE
+_ZNK10tensorflow11TensorShape10IsSameSizeERKS0_
+_ZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEll
+_ZN10tensorflow8internal17MakeCheckOpStringIliEEPSsRKT_RKT0_PKc
+_ZN18SplitRaggedBlockOpIlED2Ev
+_ZN10tensorflow8internal10LogMessage16VmoduleActivatedEPKci
+_ZTSZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_
+_ZN10tensorflow15shape_inference16InferenceContext10ReplaceDimENS0_11ShapeHandleElNS0_15DimensionHandleEPS2_
+_ZNSs4_Rep20_S_empty_rep_storageE@@GLIBCXX_3.4
+_ZTIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_
+_ZN13GetSlotFidsOpD0Ev
+_ZN10tensorflow15shape_inference19DimensionOrConstantC2El
+_ZGVZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated
+_ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
+_ZN5Eigen8internal21queryCacheSizes_intelERiS1_S1_i
+__bss_start
+_ZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZNK10tensorflow15OpKernelContext5inputEi
+_ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE1_clEiS5_E17vmodule_activated
+_ZNSt6vectorIN5Eigen8internal27TensorBlockScratchAllocatorINS0_13DefaultDeviceEE10AllocationESaIS5_EE17_M_realloc_insertIJRKS5_EEEvN9__gnu_cxx17__normal_iteratorIPS5_S7_EEDpOT_
+_ZN30UnsortedFeatureVecToSegmentsOpD2Ev
+__stack_chk_fail@@GLIBC_2.4
+_ZN10tensorflow6thread10ThreadPool11ParallelForEllRKSt8functionIFvllEE
+_ZTV13GetSlotFidsOp
+_ZN10tensorflow14kernel_factory17OpKernelRegistrarC1EPKNS_9KernelDefEN4absl14lts_2020_09_2311string_viewEPFPNS_8OpKernelEPNS_20OpKernelConstructionEE
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERS9_RKSA_
+_ZTSZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_
+memset@@GLIBC_2.2.5
+_ZN10tensorflow6errors15InvalidArgumentIJPKcEEENS_6StatusEDpT_
+_ZNSolsEi@@GLIBCXX_3.4
+_ZN6IsInOpIlED2Ev
+_ZZNK4absl14lts_2020_09_234SpanIKlEixEmENUlvE_4_FUNEv
+_ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE_clEiS5_E17vmodule_activated
+_ZZN5Eigen8internal20manage_caching_sizesENS_6ActionEPlS2_S2_E12m_cacheSizes
+_ZN10tensorflow11register_op19OpDefBuilderWrapper10SetShapeFnESt8functionIFNS_6StatusEPNS_15shape_inference16InferenceContextEEE
+_ZN30UnsortedFeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextE
+_ZTISt12length_error@@GLIBCXX_3.4
+_ZN10tensorflow11register_op19OpDefBuilderWrapper5InputESs
+__cxa_guard_acquire@@CXXABI_1.3
+_ZTVN10__cxxabiv117__class_type_infoE@@CXXABI_1.3
+_ZNSt9basic_iosIcSt11char_traitsIcEE4initEPSt15basic_streambufIcS1_E@@GLIBCXX_3.4
+_ZN18SplitRaggedBlockOpIlED0Ev
+_ZNSo9_M_insertIlEERSoT_@@GLIBCXX_3.4.9
+_ZN16PoolingBySlotsOpD0Ev
+_ZZZN30UnsortedFeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEED2Ev
+_ZN20PoolingBySlotsGradOpD2Ev
+_ZTS13GetSlotFidsOp
+_ZN6IsInOpIlE7ComputeEPN10tensorflow15OpKernelContextE
+__cxa_allocate_exception@@CXXABI_1.3
+__pthread_key_create
+__gmon_start__
+strlen@@GLIBC_2.2.5
+_ZN10tensorflow8internal10LogMessageD1Ev
+_ZN10tensorflow16KernelDefBuilderC2EPKc
+_ZNK10tensorflow6Tensor4dataEv
+_ZTVSt9bad_alloc@@GLIBCXX_3.4
+_ZTS22FeatureVecToSegmentsOp
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_
+_ZTV17ParseFeatureVecOp
+__cxa_guard_abort@@CXXABI_1.3
+_ZZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated
+_ZTI17ParseFeatureVecOp
+_ZGVZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated
+_ZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextE
+_ZN6IsInOpIiE7ComputeEPN10tensorflow15OpKernelContextE
+_ZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_EC1ERKSF_m
+_ZGVZZN30UnsortedFeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZZZN7FidIter7advanceEvENKUliPKcE_clEiS1_E17vmodule_activated
+_ZTI22FeatureVecToSegmentsOp
+_ZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextE
+_ZGVZZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZNSo9_M_insertImEERSoT_@@GLIBCXX_3.4.9
+_ZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_EC2ERKSF_m
+_ZTV30UnsortedFeatureVecToSegmentsOp
+_ZN16PoolingBySlotsOpD2Ev
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_
+_ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERS8_RKS9_
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC1ERS9_RKSA_
+_ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEED1Ev
+_ZNSt6vectorIPN10tensorflow15shape_inference9DimensionESaIS3_EE17_M_realloc_insertIJS3_EEEvN9__gnu_cxx17__normal_iteratorIPS3_S5_EEDpOT_
+_ZTI16PoolingBySlotsOp
+_ZdlPv@@GLIBCXX_3.4
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_
+_ZN10tensorflow15TensorShapeBaseINS_11TensorShapeEEC1EN4absl14lts_2020_09_234SpanIKlEE
+_ZTISt9bad_alloc@@GLIBCXX_3.4
+_ZN10tensorflow8internal21CheckOpMessageBuilderD1Ev
+_ZTIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_
+_ZN6IsInOpIlED0Ev
+_ZNSt12length_errorD1Ev@@GLIBCXX_3.4
+__cxa_guard_release@@CXXABI_1.3
+_ZN10tensorflow16KernelDefBuilderD2Ev
+_ZNSt14_Function_base13_Base_managerIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E10_M_managerERSt9_Any_dataRKS8_St18_Manager_operation
+_ZN10tensorflow8internal15LogMessageFatalC1EPKci
+_ZTS14GroupBySlotsOp
+_ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEED2Ev
+_ZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS4_E17vmodule_activated
+_ZGVZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated
+_ZTS18SplitRaggedBlockOpIfE
+_ZNSt6vectorIN10tensorflow10StackFrameESaIS1_EED2Ev
+_ZN17ParseFeatureVecOpD1Ev
+_ZN10tensorflow12OpDefBuilder5InputESs
+_ZN14GroupBySlotsOpD2Ev
+__gxx_personality_v0@@CXXABI_1.3
+_ZNSs4swapERSs@@GLIBCXX_3.4
+_ZN10tensorflow12OpDefBuilderC1ESs
+_ZN10tensorflow16KernelDefBuilder5BuildEv
+_ZTSN10tensorflow4core10RefCountedE
+_ZTVN10tensorflow4core10RefCountedE
+_ZN10tensorflow14TensorShapeRep19DestructorOutOfLineEv
+_ZSt20__throw_length_errorPKc@@GLIBCXX_3.4
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERSA_RKSB_
+_ZTI18SplitRaggedBlockOpIlE
+_ZN10tensorflow4core10RefCountedD1Ev
+__cxa_throw@@CXXABI_1.3
+_ZN16PoolingBySlotsOpD1Ev
+_ZN6IsInOpIiED0Ev
+_ZN18SplitRaggedBlockOpIlED1Ev
+_ZTI18SplitRaggedBlockOpIfE
+_ZTV16PoolingBySlotsOp
+_ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
+_ZGVZN5Eigen8internal20manage_caching_sizesENS_6ActionEPlS2_S2_E12m_cacheSizes
+_ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS3_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKSA_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSI_EEEEKNS3_ILln1EKNS4_INS5_ISI_Li2ELi1ElEELi16ES7_EEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE0EE3runERSV_RKSW_
+_ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE0_clEiS5_E17vmodule_activated
+_ZTIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_
+_ZZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated
+_ZTIN10tensorflow8OpKernelE
+_Unwind_Resume@@GCC_3.0
+_ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
+_ZNSt8ios_base4InitD1Ev@@GLIBCXX_3.4
+_ZZZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZN18SplitRaggedBlockOpIiED0Ev
+_ZTV20PoolingBySlotsGradOp
+_ZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE0_clEll
+_ZNSt14_Function_base13_Base_managerIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation
+_ZTIN10tensorflow4core10RefCountedE
+_ZN10tensorflow14kernel_factory17OpKernelRegistrar12InitInternalEPKNS_9KernelDefEN4absl14lts_2020_09_2311string_viewESt10unique_ptrINS0_15OpKernelFactoryESt14default_deleteIS9_EE
+_ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE0_clEiS5_E17vmodule_activated
+_ZN13GetSlotFidsOpD1Ev
+_ZN14GroupBySlotsOpD1Ev
+_ZNSt17_Function_handlerIFvllEZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E9_M_invokeERKSt9_Any_dataOlSB_
+_ZNSs4_Rep9_S_createEmmRKSaIcE@@GLIBCXX_3.4
+_ZZN4absl14lts_2020_09_2311string_view19CheckLengthInternalEmENKUlvE_clEv
+_ZNSt14_Function_base13_Base_managerIZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E10_M_managerERSt9_Any_dataRKS8_St18_Manager_operation
+_ZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
+_ZNSt8ios_baseD2Ev@@GLIBCXX_3.4
+_ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE1_clEiS5_E17vmodule_activated
+_ZTSZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_
+_ZZZN22FeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC1ERSC_RKSD_
+_ZN10tensorflow14kernel_factory17OpKernelRegistrarC2EPKNS_9KernelDefEN4absl14lts_2020_09_2311string_viewEPFPNS_8OpKernelEPNS_20OpKernelConstructionEE
+_ZGVZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS4_E17vmodule_activated
+_ZZN4absl14lts_2020_09_2311string_view19CheckLengthInternalEmENUlvE_4_FUNEv
+_ZSt24__throw_out_of_range_fmtPKcz
+_ZNSo9_M_insertIdEERSoT_@@GLIBCXX_3.4.9
+_ZN10tensorflow15shape_inference19DimensionOrConstantC2ENS0_15DimensionHandleE
+_ZNK10tensorflow10DeviceBase29tensorflow_cpu_worker_threadsEv
+__cxa_end_catch@@CXXABI_1.3
+_ZN18SplitRaggedBlockOpIfED2Ev
+_ZGVZZN7FidIter7advanceEvENKUliPKcE_clEiS1_E17vmodule_activated
+_ZNSt6localeC1Ev@@GLIBCXX_3.4
+_ZN13GetSlotFidsOpD2Ev
+_ZN18SplitRaggedBlockOpIfED1Ev
+_ZNSt14_Function_base13_Base_managerIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation
+_ZN17ParseFeatureVecOp7ComputeEPN10tensorflow15OpKernelContextE
+_ZNSs6assignERKSs@@GLIBCXX_3.4
+_ZNSt6vectorIN10tensorflow10StackFrameESaIS1_EED1Ev
+__cxa_rethrow@@CXXABI_1.3
+_ZNSt14_Function_base13_Base_managerIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E10_M_managerERSt9_Any_dataRKS8_St18_Manager_operation
+_ZTI14GroupBySlotsOp
+_ZZNK4absl14lts_2020_09_234SpanIKlEixEmENKUlvE_clEv
+_ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE21_M_insert_unique_nodeEmmPNS1_10_Hash_nodeIiLb0EEE
+_ZGVZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZTV18SplitRaggedBlockOpIlE
+_ZTVN10__cxxabiv120__si_class_type_infoE@@CXXABI_1.3
+_ZTV22FeatureVecToSegmentsOp
+_ZN10tensorflow8internal21CheckOpMessageBuilder7ForVar2Ev
+_ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
+_ZN10tensorflow12OpDefBuilder6OutputESs
+_ZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextE
+_ZNSt17_Function_handlerIFvllEZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E9_M_invokeERKSt9_Any_dataOlSB_
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERSA_RKSB_
+_ZN14GroupBySlotsOpD0Ev
+_ZTIZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_
+_ZN10tensorflow8OpKernel11IsExpensiveEv
+__cxa_atexit@@GLIBC_2.2.5
+_ZNSt10unique_ptrIN10tensorflow6Status5StateESt14default_deleteIS2_EED1Ev
+_ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
+_ZTS20PoolingBySlotsGradOp
+_ZN10tensorflow11register_op19OpDefBuilderWrapper6OutputESs
+__cxa_free_exception@@CXXABI_1.3
+_ZNSt17_Function_handlerIFvllEZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E9_M_invokeERKSt9_Any_dataOlSB_
+_ZN10tensorflow8OpKernel7AsAsyncEv
+_ZN10tensorflow11register_op19OpDefBuilderWrapperC2EPKc
+_ZTVSt15basic_streambufIcSt11char_traitsIcEE@@GLIBCXX_3.4
+_ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE21_M_insert_unique_nodeEmmPNS1_10_Hash_nodeIlLb0EEE
+malloc@@GLIBC_2.2.5
+_ZGVZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
+_ZN10tensorflow16KernelDefBuilder6DeviceEPKc
+_ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
+_ZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextE
+_ZN18SplitRaggedBlockOpIiED2Ev
+_ZTIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_
+_ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm1EEEvN4absl14lts_2020_09_234SpanIKlEEPSt5arrayIlXT_EE
+_ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE9_M_rehashEmRKm
+_ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev
+_ZNKSt8__detail20_Prime_rehash_policy11_M_next_bktEm
+_ZN10tensorflow11register_op19OpDefBuilderWrapperC1EPKc
+_ZN10tensorflow7strings6StrCatERKNS0_8AlphaNumE
+_ZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
+_ZN10tensorflow15shape_inference9DimensionC2El
+_ZTS6IsInOpIlE
+_ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE9_M_rehashEmRKm
+_ZTVSt9basic_iosIcSt11char_traitsIcEE@@GLIBCXX_3.4
+_ZNSs4_Rep10_M_destroyERKSaIcE@@GLIBCXX_3.4
+_ZSt16__ostream_insertIcSt11char_traitsIcEERSt13basic_ostreamIT_T0_ES6_PKS3_l@@GLIBCXX_3.4.9
+_ZNSt8ios_baseC2Ev@@GLIBCXX_3.4
+_ZN10tensorflow8internal21CheckOpMessageBuilder9NewStringEv
+_ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE_clEiS5_E17vmodule_activated
+_ZNSt6localeD1Ev@@GLIBCXX_3.4
+_ZN10tensorflow8internal17MakeCheckOpStringImmEEPSsRKT_RKT0_PKc
+_ZNSt8ios_base4InitC1Ev@@GLIBCXX_3.4
+_ZNK10tensorflow6Tensor30CheckIsAlignedAndSingleElementEv
+_ITM_registerTMCloneTable
+_ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated
+_ZN10tensorflow15shape_inference16InferenceContext8WithRankENS0_11ShapeHandleElPS2_
+_ZNK10tensorflow8OpKernel12const_tensorEv
+_ZN22FeatureVecToSegmentsOpD2Ev
+_ZN20PoolingBySlotsGradOpD1Ev
+_ZN10tensorflow15OpKernelContext15allocate_outputEiRKNS_11TensorShapeEPPNS_6TensorE
+_ZN10tensorflow8OpKernelC2EPNS_20OpKernelConstructionE
+_ZTSZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_
+_ZTVSt18basic_stringstreamIcSt11char_traitsIcESaIcEE@@GLIBCXX_3.4
+_ZTI20PoolingBySlotsGradOp
+_ZGVZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZTVN10tensorflow14kernel_factory17OpKernelRegistrar18PtrOpKernelFactoryE
+_ZN10tensorflow8internal17MakeCheckOpStringIiiEEPSsRKT_RKT0_PKc
+_ZN10tensorflow4core10RefCountedD2Ev
+_ZZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE0_clEllENKUliPKcE_clEiS5_E17vmodule_activated
+_ZNSt6vectorIlSaIlEE17_M_realloc_insertIJRKlEEEvN9__gnu_cxx17__normal_iteratorIPlS1_EEDpOT_
+_ZN10tensorflow8internal21CheckOpMessageBuilderC1EPKc
+_ZN17ParseFeatureVecOpD0Ev
+_ZNSt17_Function_handlerIFvllEZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_E9_M_invokeERKSt9_Any_dataOlSA_
+_ZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEll
+_ZTV6IsInOpIlE
+_ZTTSt18basic_stringstreamIcSt11char_traitsIcESaIcEE@@GLIBCXX_3.4
+_ZN10tensorflow8internal15LogMessageFatalD1Ev
+_ZN10tensorflow8OpKernelD2Ev
+_ZTI13GetSlotFidsOp
+_ZTV6IsInOpIiE
+_ZTIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_
+_ZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
+_ZN6IsInOpIiED2Ev
+_ZTS18SplitRaggedBlockOpIiE
+_ZNSt9basic_iosIcSt11char_traitsIcEE5clearESt12_Ios_Iostate@@GLIBCXX_3.4
+_ZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextE
+_ZN5Eigen8internal13TensorBlockIOIflLi3ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi3EEE
+_ZN10tensorflow12OpDefBuilderD1Ev
+_ZZZN17ParseFeatureVecOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZN22FeatureVecToSegmentsOpD1Ev
+_ZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextE
+_ZNK10tensorflow6Tensor21CheckTypeAndIsAlignedENS_8DataTypeE
+_ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm3EEEvN4absl14lts_2020_09_234SpanIKlEEPSt5arrayIlXT_EE
+_ZTI18SplitRaggedBlockOpIiE
+_ZGVZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated
+_ZTV18SplitRaggedBlockOpIfE
+_ZTSZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_
+_ZN10tensorflow15shape_inference9DimensionC1El
+_ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERS8_RKS9_
+_ZN10tensorflow15shape_inference16InferenceContext9MakeShapeESt16initializer_listINS0_19DimensionOrConstantEE
+_ZN5Eigen8internal13TensorBlockIOIflLi2ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi2EEE
+_ZN22FeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextE
+_ZN10tensorflow10DEVICE_CPUE
+_ZNKSt8__detail20_Prime_rehash_policy14_M_need_rehashEmmm
+_ZGVZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE0_clEllENKUliPKcE_clEiS5_E17vmodule_activated
+_ZTS6IsInOpIiE
+_ZN30UnsortedFeatureVecToSegmentsOpD0Ev
+_ZN18SplitRaggedBlockOpIiED1Ev
+_ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated
+_ZN10tensorflow16KernelDefBuilder14TypeConstraintEPKcNS_8DataTypeE
+_ZNSsC1EPKcRKSaIcE@@GLIBCXX_3.4
+_ZTS30UnsortedFeatureVecToSegmentsOp
+_ZN10tensorflow15OpKernelContext21CtxFailureWithWarningEPKciRKNS_6StatusE
+_ZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated
+_ZNSt14_Function_base13_Base_managerIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation
+_ZNSt10unique_ptrIN10tensorflow6Status5StateESt14default_deleteIS2_EED2Ev
+_ZN10tensorflow8internal17MakeCheckOpStringIllEEPSsRKT_RKT0_PKc
+_ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEED2Ev
+_ZN10tensorflow12OpDefBuilderD2Ev
+.shstrtab
+.note.gnu.build-id
+.gnu.hash
+.gnu.version
+.gnu.version_r
+.rela.dyn
+.rela.plt
+.plt.got
+.eh_frame_hdr
+.eh_frame
+.gcc_except_table
+.init_array
+.fini_array
+.data.rel.ro
+.dynamic
+.got.plt
+.comment
```

### llvm-readobj --file-headers {}

```diff
@@ -1,21 +1,30 @@
 
-Format: Mach-O 64-bit x86-64
+Format: elf64-x86-64
 Arch: x86_64
 AddressSize: 64bit
-MachHeader {
-  Magic: Magic64 (0xFEEDFACF)
-  CpuType: X86-64 (0x1000007)
-  CpuSubType: CPU_SUBTYPE_X86_64_ALL (0x3)
-  FileType: DynamicLibrary (0x6)
-  NumOfLoadCommands: 16
-  SizeOfLoadCommands: 1824
-  Flags [ (0x118085)
-    MH_BINDS_TO_WEAK (0x10000)
-    MH_DYLDLINK (0x4)
-    MH_NOUNDEFS (0x1)
-    MH_NO_REEXPORTED_DYLIBS (0x100000)
-    MH_TWOLEVEL (0x80)
-    MH_WEAK_DEFINES (0x8000)
+LoadName: <Not found>
+ElfHeader {
+  Ident {
+    Magic: (7F 45 4C 46)
+    Class: 64-bit (0x2)
+    DataEncoding: LittleEndian (0x1)
+    FileVersion: 1
+    OS/ABI: GNU/Linux (0x3)
+    ABIVersion: 0
+    Unused: (00 00 00 00 00 00 00)
+  }
+  Type: SharedObject (0x3)
+  Machine: EM_X86_64 (0x3E)
+  Version: 1
+  Entry: 0xBD60
+  ProgramHeaderOffset: 0x40
+  SectionHeaderOffset: 0x6E798
+  Flags [ (0x0)
   ]
-  Reserved: 0x0
+  HeaderSize: 64
+  ProgramHeaderEntrySize: 56
+  ProgramHeaderCount: 7
+  SectionHeaderEntrySize: 64
+  SectionHeaderCount: 30
+  StringTableSectionIndex: 29
 }
```

### llvm-readobj --needed-libs {}

```diff
@@ -1,10 +1,11 @@
 
-Format: Mach-O 64-bit x86-64
+Format: elf64-x86-64
 Arch: x86_64
 AddressSize: 64bit
+LoadName: <Not found>
 NeededLibraries [
-  /usr/lib/libSystem.B.dylib
-  /usr/lib/libc++.1.dylib
-  @rpath/libtensorflow_framework.2.dylib
-  tensorflow_hs_addon/python/ops/_reco_ops.so
+  libc.so.6
+  libgcc_s.so.1
+  libstdc++.so.6
+  libtensorflow_framework.so.2
 ]
```

### llvm-readobj --symbols {}

```diff
@@ -1,7574 +1,4948 @@
 
-Format: Mach-O 64-bit x86-64
+Format: elf64-x86-64
 Arch: x86_64
 AddressSize: 64bit
+LoadName: <Not found>
 Symbols [
   Symbol {
-    Name: __ZNSt3__1lsIN10tensorflow8internal15LogMessageFatalENS_12basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEEEEENS_9enable_ifIXaantsr19is_lvalue_referenceIT_EE5valuesr10is_base_ofINS_8ios_baseESB_EE5valueEOSB_E4typeESD_RKT0_ (14569)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1080
-  }
-  Symbol {
-    Name: ___clang_call_terminate (14795)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x10B0
-  }
-  Symbol {
-    Name: __ZZNK3$_0clEPKN10tensorflow9KernelDefEENUlPNS0_20OpKernelConstructionEE_8__invokeES5_ (14819)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x10C0
-  }
-  Symbol {
-    Name: __ZN20PoolingBySlotsGradOpD1Ev (14906)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1110
-  }
-  Symbol {
-    Name: __ZN13GetSlotFidsOpD1Ev (14937)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1110
-  }
-  Symbol {
-    Name: __ZN14GroupBySlotsOpD1Ev (14961)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1110
-  }
-  Symbol {
-    Name: __ZN6IsInOpIiED1Ev (14986)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1110
-  }
-  Symbol {
-    Name: __ZN6IsInOpIxED1Ev (15005)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1110
-  }
-  Symbol {
-    Name: __ZN18SplitRaggedBlockOpIfED1Ev (15024)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1110
-  }
-  Symbol {
-    Name: __ZN18SplitRaggedBlockOpIiED1Ev (15056)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1110
-  }
-  Symbol {
-    Name: __ZN18SplitRaggedBlockOpIxED1Ev (15088)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1110
-  }
-  Symbol {
-    Name: __ZN16PoolingBySlotsOpD1Ev (15120)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1110
-  }
-  Symbol {
-    Name: __ZN20PoolingBySlotsGradOpD0Ev (15147)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1120
-  }
-  Symbol {
-    Name: __ZN13GetSlotFidsOpD0Ev (15178)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1120
-  }
-  Symbol {
-    Name: __ZN14GroupBySlotsOpD0Ev (15202)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1120
-  }
-  Symbol {
-    Name: __ZN6IsInOpIiED0Ev (15227)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1120
-  }
-  Symbol {
-    Name: __ZN6IsInOpIxED0Ev (15246)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1120
-  }
-  Symbol {
-    Name: __ZN18SplitRaggedBlockOpIfED0Ev (15265)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1120
-  }
-  Symbol {
-    Name: __ZN18SplitRaggedBlockOpIiED0Ev (15297)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1120
-  }
-  Symbol {
-    Name: __ZN18SplitRaggedBlockOpIxED0Ev (15329)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1120
-  }
-  Symbol {
-    Name: __ZN16PoolingBySlotsOpD0Ev (15361)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1120
-  }
-  Symbol {
-    Name: __ZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextE (15388)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1140
-  }
-  Symbol {
-    Name: __ZNK10tensorflow8OpKernel12const_tensorEv (15452)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1C30
-  }
-  Symbol {
-    Name: __ZN10tensorflow8OpKernel7AsAsyncEv (15495)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C30
-  }
-  Symbol {
-    Name: __ZN10tensorflow8OpKernel11IsExpensiveEv (15531)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C40
-  }
-  Symbol {
-    Name: __ZN10tensorflow6errors15InvalidArgumentIJPKcEEENS_6StatusEDpT_ (15572)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C50
-  }
-  Symbol {
-    Name: __ZNK10tensorflow6Tensor6shapedIiLm2EEENS_6TTypesIT_XT0_ElE11ConstTensorEN4absl14lts_2020_09_234SpanIKxEE (15636)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1DE0
-  }
-  Symbol {
-    Name: __ZNK10tensorflow6Tensor6shapedIfLm2EEENS_6TTypesIT_XT0_ElE11ConstTensorEN4absl14lts_2020_09_234SpanIKxEE (15742)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1EB0
-  }
-  Symbol {
-    Name: __ZN10tensorflow6errors8internal16PrepareForStrCatIPKcEENSt3__19enable_ifIXntsr3std14is_convertibleIT_NS_7strings8AlphaNumEEE5valueENS5_12basic_stringIcNS5_11char_traitsIcEENS5_9allocatorIcEEEEE4typeERKS7_ (15848)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F80
-  }
-  Symbol {
-    Name: __ZN10tensorflow6StatusC1ENS_5error4CodeEN4absl14lts_2020_09_2311string_viewE (16054)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x2170
-  }
-  Symbol {
-    Name: __ZNSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEED1Ev (16132)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x2230
-  }
-  Symbol {
-    Name: __ZNSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEED0Ev (16207)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x22C0
-  }
-  Symbol {
-    Name: __ZThn16_NSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEED1Ev (16282)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x2350
-  }
-  Symbol {
-    Name: __ZThn16_NSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEED0Ev (16363)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x23D0
-  }
-  Symbol {
-    Name: __ZTv0_n24_NSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEED1Ev (16444)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x2460
-  }
-  Symbol {
-    Name: __ZTv0_n24_NSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEED0Ev (16527)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x2500
-  }
-  Symbol {
-    Name: __ZNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEED1Ev (16610)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x25A0
-  }
-  Symbol {
-    Name: __ZNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEED0Ev (16682)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x25E0
-  }
-  Symbol {
-    Name: __ZNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEE7seekoffExNS_8ios_base7seekdirEj (16754)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x2620
-  }
-  Symbol {
-    Name: __ZNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEE7seekposENS_4fposI11__mbstate_tEEj (16854)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x2760
-  }
-  Symbol {
-    Name: __ZNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEE9underflowEv (16956)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x2790
-  }
-  Symbol {
-    Name: __ZNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEE9pbackfailEi (17036)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x27E0
-  }
-  Symbol {
-    Name: __ZNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEE8overflowEi (17116)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x2840
-  }
-  Symbol {
-    Name: __ZNSt3__124__put_character_sequenceIcNS_11char_traitsIcEEEERNS_13basic_ostreamIT_T0_EES7_PKS4_m (17195)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x29B0
-  }
-  Symbol {
-    Name: __ZNSt3__116__pad_and_outputIcNS_11char_traitsIcEEEENS_19ostreambuf_iteratorIT_T0_EES6_PKS4_S8_S8_RNS_8ios_baseES4_ (17292)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x2B10
-  }
-  Symbol {
-    Name: __ZNSt3__1L20__throw_length_errorEPKc (17408)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x2C80
-  }
-  Symbol {
-    Name: __ZNSt12length_errorC1EPKc (17446)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x2CD0
-  }
-  Symbol {
-    Name: __ZNKSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEE3strEv (17473)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x2D00
-  }
-  Symbol {
-    Name: __ZN10tensorflow6Status5StateD2Ev (17548)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x30D0
-  }
-  Symbol {
-    Name: __ZNSt3__1lsIN10tensorflow8internal15LogMessageFatalEA27_cEENS_9enable_ifIXaantsr19is_lvalue_referenceIT_EE5valuesr10is_base_ofINS_8ios_baseES6_EE5valueEOS6_E4typeES8_RKT0_ (17582)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x31D0
-  }
-  Symbol {
-    Name: __ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm2EEEvN4absl14lts_2020_09_234SpanIKxEEPNSt3__15arrayIlXT_EEE (17755)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x31F0
-  }
-  Symbol {
-    Name: __ZN10tensorflow8internal17MakeCheckOpStringImmEEPNSt3__112basic_stringIcNS2_11char_traitsIcEENS2_9allocatorIcEEEERKT_RKT0_PKc (17878)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x3350
-  }
-  Symbol {
-    Name: __ZN10tensorflow8internal17MakeCheckOpStringIxxEEPNSt3__112basic_stringIcNS2_11char_traitsIcEENS2_9allocatorIcEEEERKT_RKT0_PKc (18005)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x33D0
-  }
-  Symbol {
-    Name: __ZNK10tensorflow6Tensor6shapedIiLm1EEENS_6TTypesIT_XT0_ElE11ConstTensorEN4absl14lts_2020_09_234SpanIKxEE (18132)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x3450
-  }
-  Symbol {
-    Name: __ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm1EEEvN4absl14lts_2020_09_234SpanIKxEEPNSt3__15arrayIlXT_EEE (18238)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x3500
-  }
-  Symbol {
-    Name: __ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm3EEEvN4absl14lts_2020_09_234SpanIKxEEPNSt3__15arrayIlXT_EEE (18361)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x3640
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE7destroyEv (18484)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37C0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEED1Ev (18618)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37C0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE7destroyEv (18743)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37C0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEED1Ev (18874)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37C0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE7destroyEv (19000)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37C0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEED1Ev (19132)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37C0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE7destroyEv (19265)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37C0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEED1Ev (19404)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37C0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE7destroyEv (19537)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37C0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEED1Ev (19676)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37C0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE7destroyEv (19809)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37C0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEED1Ev (19948)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x37C0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE18destroy_deallocateEv (20076)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37D0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEED0Ev (20222)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37D0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE18destroy_deallocateEv (20347)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37D0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEED0Ev (20490)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37D0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE18destroy_deallocateEv (20616)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37D0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEED0Ev (20760)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37D0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE18destroy_deallocateEv (20893)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37D0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEED0Ev (21044)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37D0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE18destroy_deallocateEv (21177)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37D0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEED0Ev (21328)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37D0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE18destroy_deallocateEv (21461)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x37D0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEED0Ev (21612)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x37D0
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE7__cloneEv (21740)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x37E0
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE7__cloneEPNS0_6__baseIS9_EE (21875)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x3830
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEclEOxSB_ (22027)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x3870
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE6targetERKSt9type_info (22159)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x3890
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE11target_typeEv (22306)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x38B0
-  }
-  Symbol {
-    Name: __ZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExx (22446)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x38C0
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS3_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKSA_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSI_EEEEKNS3_ILln1EKNS4_INS5_ISI_Li2ELi1ElEELi16ES7_EEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE0EE3runERSV_RKSW_ (22525)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x3BC0
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERS9_RKSA_ (22931)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x3F70
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_ (23095)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x40E0
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_ (23247)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x4280
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f (23401)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x43E0
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f (23581)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x4680
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE8coeffRefEl (23749)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x4840
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl (23911)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x4940
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl (24084)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x4BE0
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5coeffEl (24245)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x4D50
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl (24406)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x4E50
-  }
-  Symbol {
-    Name: __ZZNK3$_1clEPKN10tensorflow9KernelDefEENUlPNS0_20OpKernelConstructionEE_8__invokeES5_ (24569)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x4FC0
-  }
-  Symbol {
-    Name: __ZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextE (24656)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x5010
-  }
-  Symbol {
-    Name: __ZNK10tensorflow6Tensor6shapedIfLm3EEENS_6TTypesIT_XT0_ElE11ConstTensorEN4absl14lts_2020_09_234SpanIKxEE (24724)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x5980
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKS9_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSH_EEEEKNS3_ILln1EKNS3_ILln1EKNS4_INS5_ISH_Li3ELi1ElEELi16ES7_EEEEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE1EE3runERSW_RKSX_ (24830)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x5A50
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEEKNS_19TensorCwiseBinaryOpINS_8internal13scalar_sum_opIffEEKS8_KNS_18TensorCwiseUnaryOpINSA_10bind1st_opINSA_17scalar_product_opIKfSH_EEEEKNS2_ILln1EKNS2_ILln1EKNS3_INS4_ISH_Li3ELi1ElEELi16ES6_EEEEEEEEEEEENS_13DefaultDeviceEE23getResourceRequirementsEv (25237)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x5DC0
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_ (25629)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x5F20
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERSC_RKSD_ (25781)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x6080
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_ (25948)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x61F0
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_19TensorCwiseBinaryOpINS_8internal13scalar_sum_opIffEEKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEEKNS_18TensorCwiseUnaryOpINS2_10bind1st_opINS2_17scalar_product_opIKfSG_EEEEKNS5_ILln1EKNS5_ILln1EKNS6_INS7_ISG_Li3ELi1ElEELi16ES9_EEEEEEEEEENS_13DefaultDeviceEE23getResourceRequirementsEv (26102)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x6390
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal15queryCacheSizesERiS1_S1_ (26468)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x6510
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal27queryCacheSizes_intel_codesERiS1_S1_ (26514)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x67A0
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE23getResourceRequirementsEv (26572)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x6E80
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal17TensorBlockMapperILi1ELi1ElE25InitializeBlockDimensionsEv (26755)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x7070
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE10writeBlockINS_8internal22TensorCwiseBinaryBlockINSB_13scalar_sum_opIffEENSB_23TensorMaterializedBlockIfLi1ELi1ElEENSB_21TensorCwiseUnaryBlockINSB_10bind1st_opINSB_17scalar_product_opIKfSK_EEEESG_EEEEEEvRKNSB_21TensorBlockDescriptorILi1ElEERKT_ (26834)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x7160
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSB_27TensorBlockScratchAllocatorIS9_EEb (27218)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x7290
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_9TensorMapIKNS_6TensorIfLi2ELi1ElEELi0ENS_11MakePointerEEElE3RunERKNS8_6TargetERKS7_ (27451)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x7640
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal23TensorMaterializedBlockIfLi2ELi1ElE11materializeINS_6DSizesIlLi2EEENS0_27TensorBlockScratchAllocatorINS_13DefaultDeviceEEEEES2_PKfRKT_RNS0_21TensorBlockDescriptorILi2ElEERT0_ (27587)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x7FB0
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEE8allocateEm (27783)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x8170
-  }
-  Symbol {
-    Name: __ZNSt3__16vectorIN5Eigen8internal27TensorBlockScratchAllocatorINS1_13DefaultDeviceEE10AllocationENS_9allocatorIS6_EEE21__push_back_slow_pathIRKS6_EEvOT_ (27864)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x8370
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal13TensorBlockIOIflLi2ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi2EEE (28018)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x8490
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSF_27TensorBlockScratchAllocatorISD_EEb (28113)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0xA670
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi2ElEERNSD_27TensorBlockScratchAllocatorISB_EEb (28361)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0xA9F0
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal21TensorBlockAssignmentIfLi3ENS_9TensorMapIKNS_6TensorIfLi3ELi1ElEELi0ENS_11MakePointerEEElE3RunERKNS8_6TargetERKS7_ (28596)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0xAEC0
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal23TensorMaterializedBlockIfLi3ELi1ElE11materializeINS_6DSizesIlLi3EEENS0_27TensorBlockScratchAllocatorINS_13DefaultDeviceEEEEES2_PKfRKT_RNS0_21TensorBlockDescriptorILi3ElEERT0_ (28732)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0xB9C0
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal13TensorBlockIOIflLi3ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi3EEE (28928)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0xBC30
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_17TensorReshapingOpIKNS_6DSizesIlLi2EEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKNS_9TensorMapIKNS_6TensorIfLi1ELi1ElEELi0ENS_11MakePointerEEEKNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSJ_EEEESF_EEEEEElE3RunERKNSR_6TargetERKSQ_ (29023)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
+    Name:  (0)
+    Value: 0x0
+    Size: 0
+    Binding: Local (0x0)
+    Type: None (0x0)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: .note.gnu.build-id (0)
+    Value: 0x1C8
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .note.gnu.build-id (0x1)
+  }
+  Symbol {
+    Name: .gnu.hash (0)
+    Value: 0x1F0
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .gnu.hash (0x2)
+  }
+  Symbol {
+    Name: .dynsym (0)
+    Value: 0x9E0
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .dynsym (0x3)
+  }
+  Symbol {
+    Name: .dynstr (0)
+    Value: 0x2B58
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .dynstr (0x4)
+  }
+  Symbol {
+    Name: .gnu.version (0)
+    Value: 0x89C8
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .gnu.version (0x5)
+  }
+  Symbol {
+    Name: .gnu.version_r (0)
+    Value: 0x8C98
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .gnu.version_r (0x6)
+  }
+  Symbol {
+    Name: .rela.dyn (0)
+    Value: 0x8D38
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .rela.dyn (0x7)
+  }
+  Symbol {
+    Name: .rela.plt (0)
+    Value: 0xA718
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .rela.plt (0x8)
+  }
+  Symbol {
+    Name: .init (0)
+    Value: 0xB450
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .init (0x9)
+  }
+  Symbol {
+    Name: .plt (0)
+    Value: 0xB470
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .plt (0xA)
+  }
+  Symbol {
+    Name: .plt.got (0)
+    Value: 0xBD50
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .plt.got (0xB)
+  }
+  Symbol {
+    Name: .text (0)
+    Value: 0xBD60
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: .fini (0)
+    Value: 0x520C0
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .fini (0xD)
+  }
+  Symbol {
+    Name: .rodata (0)
+    Value: 0x520E0
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: .eh_frame_hdr (0)
+    Value: 0x5CCFC
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .eh_frame_hdr (0xF)
+  }
+  Symbol {
+    Name: .eh_frame (0)
+    Value: 0x5D1E8
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .eh_frame (0x10)
+  }
+  Symbol {
+    Name: .gcc_except_table (0)
+    Value: 0x5EE94
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .gcc_except_table (0x11)
+  }
+  Symbol {
+    Name: .init_array (0)
+    Value: 0x260518
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .init_array (0x12)
+  }
+  Symbol {
+    Name: .fini_array (0)
+    Value: 0x260560
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .fini_array (0x13)
+  }
+  Symbol {
+    Name: .data.rel.ro (0)
+    Value: 0x260568
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: .dynamic (0)
+    Value: 0x260AE8
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .dynamic (0x15)
+  }
+  Symbol {
+    Name: .got (0)
+    Value: 0x260CD8
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .got (0x16)
+  }
+  Symbol {
+    Name: .got.plt (0)
+    Value: 0x261000
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .got.plt (0x17)
+  }
+  Symbol {
+    Name: .data (0)
+    Value: 0x261480
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .data (0x18)
+  }
+  Symbol {
+    Name: .bss (0)
+    Value: 0x261490
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: .comment (0)
+    Value: 0x0
+    Size: 0
+    Binding: Local (0x0)
+    Type: Section (0x3)
+    Other: 0
+    Section: .comment (0x1A)
+  }
+  Symbol {
+    Name: feature_pooling.cc (9107)
+    Value: 0x0
+    Size: 0
+    Binding: Local (0x0)
+    Type: File (0x4)
+    Other: 0
+    Section: Absolute (0xFFF1)
+  }
+  Symbol {
+    Name: _ZNSs4_Rep10_M_disposeERKSaIcE.part.7 (1)
+    Value: 0xBD60
+    Size: 39
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZNKUlPKN10tensorflow9KernelDefEE_clES2_ENUlPNS_20OpKernelConstructionEE_4_FUNES5_ (39)
+    Value: 0xDDC0
+    Size: 79
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZNKUlPKN10tensorflow9KernelDefEE0_clES2_ENUlPNS_20OpKernelConstructionEE_4_FUNES5_ (123)
+    Value: 0xDE10
+    Size: 79
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorINS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE8coeffRefEl.isra.118.part.119 (208)
+    Value: 0xDE60
+    Size: 35
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZN5Eigen15TensorEvaluatorINS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE8coeffRefElE19__PRETTY_FUNCTION__ (346)
+    Value: 0x59080
+    Size: 408
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZNK5Eigen8internal21TensorBlockDescriptorILi1ElE17DestinationBuffer4dataIfEEPT_v.isra.186.part.187 (489)
+    Value: 0xBD88
+    Size: 35
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZNK5Eigen8internal21TensorBlockDescriptorILi1ElE17DestinationBuffer4dataIfEEPT_vE19__PRETTY_FUNCTION__ (589)
+    Value: 0x554C0
+    Size: 161
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZNK5Eigen15TensorEvaluatorINS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE5coeffEl.isra.206.part.207 (694)
+    Value: 0xDE90
+    Size: 35
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZNK5Eigen15TensorEvaluatorINS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE5coeffElE19__PRETTY_FUNCTION__ (830)
+    Value: 0x57280
+    Size: 410
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZNK5Eigen15TensorEvaluatorIKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE5coeffEl.isra.208.part.209 (971)
+    Value: 0xBDAC
+    Size: 35
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZNK5Eigen15TensorEvaluatorIKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE5coeffElE19__PRETTY_FUNCTION__ (1109)
+    Value: 0x57B00
+    Size: 452
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZNK5Eigen8internal21TensorBlockDescriptorILi2ElE17DestinationBuffer4dataIfEEPT_v.isra.264.part.265 (1252)
+    Value: 0xBDD0
+    Size: 35
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZNK5Eigen8internal21TensorBlockDescriptorILi2ElE17DestinationBuffer4dataIfEEPT_vE19__PRETTY_FUNCTION__ (1352)
+    Value: 0x551E0
+    Size: 161
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZNK5Eigen15TensorEvaluatorIKNS_9TensorMapIKNS_6TensorIfLi1ELi1ElEELi0ENS_11MakePointerEEENS_13DefaultDeviceEE5coeffEl.isra.286.part.287 (1457)
+    Value: 0xBDF4
+    Size: 35
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZNK5Eigen15TensorEvaluatorIKNS_9TensorMapIKNS_6TensorIfLi1ELi1ElEELi0ENS_11MakePointerEEENS_13DefaultDeviceEE5coeffElE19__PRETTY_FUNCTION__ (1594)
+    Value: 0x53500
+    Size: 445
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZNK5Eigen8internal21TensorBlockDescriptorILi3ElE17DestinationBuffer4dataIfEEPT_v.isra.301.part.302 (1736)
+    Value: 0xBE18
+    Size: 35
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZNK5Eigen8internal21TensorBlockDescriptorILi3ElE17DestinationBuffer4dataIfEEPT_vE19__PRETTY_FUNCTION__ (1836)
+    Value: 0x54DA0
+    Size: 161
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE23getResourceRequirementsEv.isra.224 (1941)
+    Value: 0xE010
+    Size: 2568
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZN4absl14lts_2020_09_2311string_view19CheckLengthInternalEmENKUlvE_clEvE19__PRETTY_FUNCTION__ (2117)
+    Value: 0x592A0
+    Size: 113
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZZNK4absl14lts_2020_09_234SpanIKlEixEmENKUlvE_clEvE19__PRETTY_FUNCTION__ (2214)
+    Value: 0x59220
+    Size: 128
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen8internal11DimensionIdILln1EEC4ElE19__PRETTY_FUNCTION__ (2289)
+    Value: 0x58E80
+    Size: 65
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC4ERS8_RKS9_E19__PRETTY_FUNCTION__ (2355)
+    Value: 0x565A0
+    Size: 473
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC4ERSA_RKSB_E19__PRETTY_FUNCTION__ (2529)
+    Value: 0x58380
+    Size: 497
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC4ERS8_RKS9_E19__PRETTY_FUNCTION__ (2705)
+    Value: 0x58A80
+    Size: 473
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC4ERS9_RKSA_E19__PRETTY_FUNCTION__ (2879)
+    Value: 0x58C60
+    Size: 533
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv8_flE19__PRETTY_FUNCTION__ (3065)
+    Value: 0x57CE0
+    Size: 666
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv8_fE19__PRETTY_FUNCTION__ (3250)
+    Value: 0x56920
+    Size: 564
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE8srcCoeffElE19__PRETTY_FUNCTION__ (3440)
+    Value: 0x57420
+    Size: 510
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE6packetILi0EEEDv8_flE19__PRETTY_FUNCTION__ (3614)
+    Value: 0x57620
+    Size: 684
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv8_fE19__PRETTY_FUNCTION__ (3809)
+    Value: 0x56B60
+    Size: 594
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE8srcCoeffElE19__PRETTY_FUNCTION__ (4011)
+    Value: 0x578E0
+    Size: 522
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv8_flE19__PRETTY_FUNCTION__ (4187)
+    Value: 0x56FE0
+    Size: 654
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE8srcCoeffElE19__PRETTY_FUNCTION__ (4370)
+    Value: 0x56DC0
+    Size: 540
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen15TensorEvaluatorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS2_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_19TensorCwiseBinaryOpINS_8internal13scalar_sum_opIffEEKS9_KNS_18TensorCwiseUnaryOpINSB_10bind1st_opINSB_17scalar_product_opIKfSI_EEEEKNS2_ILln1EKNS3_INS4_ISI_Li2ELi1ElEELi16ES6_EEEEEEEEEENS_13DefaultDeviceEE20evalSubExprsIfNeededEPfE19__PRETTY_FUNCTION__ (4556)
+    Value: 0x57F80
+    Size: 1021
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen15TensorEvaluatorIKNS_19TensorCwiseBinaryOpINS_8internal13scalar_sum_opIffEEKNS_16TensorChippingOpILln1ENS5_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_18TensorCwiseUnaryOpINS2_10bind1st_opINS2_17scalar_product_opIKfSH_EEEEKNS5_ILln1EKNS6_INS7_ISH_Li2ELi1ElEELi16ES9_EEEEEEEENS_13DefaultDeviceEEC4ERSS_RKST_E19__PRETTY_FUNCTION__ (4966)
+    Value: 0x58580
+    Size: 1261
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC4ERSA_RKSB_E19__PRETTY_FUNCTION__ (5337)
+    Value: 0x55C60
+    Size: 497
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC4ERSC_RKSD_E19__PRETTY_FUNCTION__ (5513)
+    Value: 0x55E60
+    Size: 569
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen8internal13TensorBlockIOIflLi2ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi2EEEE19__PRETTY_FUNCTION__ (5702)
+    Value: 0x53EC0
+    Size: 456
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEE8allocateEmE19__PRETTY_FUNCTION__ (5819)
+    Value: 0x54D00
+    Size: 152
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen8internal13TensorBlockIOIflLi3ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi3EEEE19__PRETTY_FUNCTION__ (5922)
+    Value: 0x54B20
+    Size: 456
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZNK5Eigen15TensorEvaluatorIKNS_9TensorMapIKNS_6TensorIfLi3ELi1ElEELi0ENS_11MakePointerEEENS_13DefaultDeviceEE5coeffElE19__PRETTY_FUNCTION__ (6039)
+    Value: 0x547C0
+    Size: 445
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZNK5Eigen15TensorEvaluatorIKNS_9TensorMapIKNS_6TensorIfLi2ELi1ElEELi0ENS_11MakePointerEEENS_13DefaultDeviceEE5coeffElE19__PRETTY_FUNCTION__ (6181)
+    Value: 0x54600
+    Size: 445
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZNK5Eigen15TensorEvaluatorINS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi2ElEERNS8_27TensorBlockScratchAllocatorIS6_EEbE19__PRETTY_FUNCTION__ (6323)
+    Value: 0x540A0
+    Size: 838
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE10writeBlockINS_8internal22TensorCwiseBinaryBlockINSB_13scalar_sum_opIffEENSB_23TensorMaterializedBlockIfLi1ELi1ElEENSB_21TensorCwiseUnaryBlockINSB_10bind1st_opINSB_17scalar_product_opIKfSK_EEEESG_EEEEEEvRKNSB_21TensorBlockDescriptorILi1ElEERKT_E19__PRETTY_FUNCTION__ (6548)
+    Value: 0x53B60
+    Size: 858
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZNK5Eigen15TensorEvaluatorIKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi3ElEERNSA_27TensorBlockScratchAllocatorIS8_EEbE19__PRETTY_FUNCTION__ (6954)
+    Value: 0x54E60
+    Size: 886
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE8srcCoeffElE19__PRETTY_FUNCTION__ (7181)
+    Value: 0x54400
+    Size: 510
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen15TensorEvaluatorIKNS_19TensorCwiseBinaryOpINS_8internal13scalar_sum_opIffEEKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEEKNS_18TensorCwiseUnaryOpINS2_10bind1st_opINS2_17scalar_product_opIKfSG_EEEEKNS5_ILln1EKNS5_ILln1EKNS6_INS7_ISG_Li3ELi1ElEELi16ES9_EEEEEEEEEENS_13DefaultDeviceEEC4ERST_RKSU_E19__PRETTY_FUNCTION__ (7355)
+    Value: 0x560A0
+    Size: 1273
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen15TensorEvaluatorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEEKNS_19TensorCwiseBinaryOpINS_8internal13scalar_sum_opIffEEKS8_KNS_18TensorCwiseUnaryOpINSA_10bind1st_opINSA_17scalar_product_opIKfSH_EEEEKNS2_ILln1EKNS2_ILln1EKNS3_INS4_ISH_Li3ELi1ElEELi16ES6_EEEEEEEEEEEENS_13DefaultDeviceEE20evalSubExprsIfNeededEPfE19__PRETTY_FUNCTION__ (7727)
+    Value: 0x55860
+    Size: 997
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen8internal21TensorBlockAssignmentIfLi3ENS_9TensorMapIKNS_6TensorIfLi3ELi1ElEELi0ENS_11MakePointerEEElE3RunERKNS8_6TargetERKS7_E19__PRETTY_FUNCTION__ (8138)
+    Value: 0x54980
+    Size: 389
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen15TensorEvaluatorIKNS_17TensorReshapingOpIKNS_6DSizesIlLi2EEEKNS_19TensorCwiseBinaryOpINS_8internal13scalar_sum_opIffEEKNS_9TensorMapIKNS_6TensorIfLi1ELi1ElEELi0ENS_11MakePointerEEEKNS_18TensorCwiseUnaryOpINS6_10bind1st_opINS6_17scalar_product_opIKfSJ_EEEESF_EEEEEENS_13DefaultDeviceEEC4ERSR_RKSS_E19__PRETTY_FUNCTION__ (8296)
+    Value: 0x536C0
+    Size: 1169
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE8srcCoeffElE19__PRETTY_FUNCTION__ (8626)
+    Value: 0x55580
+    Size: 558
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE8srcCoeffElE19__PRETTY_FUNCTION__ (8815)
+    Value: 0x552A0
+    Size: 522
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen8internal17TensorBlockMapperILi1ELi1ElE25InitializeBlockDimensionsEvE19__PRETTY_FUNCTION__ (8991)
+    Value: 0x557C0
+    Size: 158
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _GLOBAL__sub_I_feature_pooling.cc (9092)
+    Value: 0xBE40
+    Size: 280
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZStL8__ioinit (9126)
+    Value: 0x261491
+    Size: 1
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZZN5Eigen15TensorEvaluatorINS_9TensorMapINS_6TensorIiLi2ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE8coeffRefElE19__PRETTY_FUNCTION__ (9141)
+    Value: 0x58EE0
+    Size: 404
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen15TensorEvaluatorINS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE8coeffRefElE19__PRETTY_FUNCTION__ (9284)
+    Value: 0x56780
+    Size: 408
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: get_slot_fids.cc (9442)
+    Value: 0x0
+    Size: 0
+    Binding: Local (0x0)
+    Type: File (0x4)
+    Other: 0
+    Section: Absolute (0xFFF1)
+  }
+  Symbol {
+    Name: _ZZNKUlPKN10tensorflow9KernelDefEE_clES2_ENUlPNS_20OpKernelConstructionEE_4_FUNES5_ (39)
+    Value: 0x258E0
+    Size: 79
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZN4absl14lts_2020_09_2311string_view19CheckLengthInternalEmENKUlvE_clEvE19__PRETTY_FUNCTION__ (2117)
+    Value: 0x597E0
+    Size: 113
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _GLOBAL__sub_I_get_slot_fids.cc (9427)
+    Value: 0xBF60
+    Size: 283
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZStL8__ioinit (9126)
+    Value: 0x2614E8
+    Size: 1
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZZZNK4absl14lts_2020_09_234SpanIKlEixEmENKUlvE_clEvE19__PRETTY_FUNCTION__ (2214)
+    Value: 0x59760
+    Size: 128
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen15TensorEvaluatorINS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE8coeffRefElE19__PRETTY_FUNCTION__ (9284)
+    Value: 0x59420
+    Size: 408
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen15TensorEvaluatorINS_9TensorMapINS_6TensorIiLi2ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE8coeffRefElE19__PRETTY_FUNCTION__ (9141)
+    Value: 0x595C0
+    Size: 404
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: split_ragged_block.cc (9559)
+    Value: 0x0
+    Size: 0
+    Binding: Local (0x0)
+    Type: File (0x4)
+    Other: 0
+    Section: Absolute (0xFFF1)
+  }
+  Symbol {
+    Name: _ZZNKUlPKN10tensorflow9KernelDefEE_clES2_ENUlPNS_20OpKernelConstructionEE_4_FUNES5_ (39)
+    Value: 0x29630
+    Size: 79
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZNKUlPKN10tensorflow9KernelDefEE0_clES2_ENUlPNS_20OpKernelConstructionEE_4_FUNES5_ (123)
+    Value: 0x29680
+    Size: 79
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZNKUlPKN10tensorflow9KernelDefEE1_clES2_ENUlPNS_20OpKernelConstructionEE_4_FUNES5_ (9459)
+    Value: 0x296D0
+    Size: 79
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZN4absl14lts_2020_09_2311string_view19CheckLengthInternalEmENKUlvE_clEvE19__PRETTY_FUNCTION__ (2117)
+    Value: 0x59A60
+    Size: 113
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _GLOBAL__sub_I_split_ragged_block.cc (9544)
+    Value: 0xC080
+    Size: 414
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZStL8__ioinit (9126)
+    Value: 0x2614E9
+    Size: 1
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZZZNK4absl14lts_2020_09_234SpanIKlEixEmENKUlvE_clEvE19__PRETTY_FUNCTION__ (2214)
+    Value: 0x599E0
+    Size: 128
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: feature_vec_to_sparse.cc (9596)
+    Value: 0x0
+    Size: 0
+    Binding: Local (0x0)
+    Type: File (0x4)
+    Other: 0
+    Section: Absolute (0xFFF1)
+  }
+  Symbol {
+    Name: _ZZNKUlPKN10tensorflow9KernelDefEE_clES2_ENUlPNS_20OpKernelConstructionEE_4_FUNES5_ (39)
+    Value: 0x32AE0
+    Size: 79
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZNKUlPKN10tensorflow9KernelDefEE0_clES2_ENUlPNS_20OpKernelConstructionEE_4_FUNES5_ (123)
+    Value: 0x32B30
+    Size: 79
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZN4absl14lts_2020_09_2311string_view19CheckLengthInternalEmENKUlvE_clEvE19__PRETTY_FUNCTION__ (2117)
+    Value: 0x5A0E0
+    Size: 113
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZZNK4absl14lts_2020_09_234SpanIKlEixEmENKUlvE_clEvE19__PRETTY_FUNCTION__ (2214)
+    Value: 0x5A060
+    Size: 128
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _GLOBAL__sub_I_feature_vec_to_sparse.cc (9581)
+    Value: 0xC220
+    Size: 280
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZStL8__ioinit (9126)
+    Value: 0x2615A9
+    Size: 1
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZZN5Eigen15TensorEvaluatorINS_9TensorMapINS_6TensorIiLi1ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE8coeffRefElE19__PRETTY_FUNCTION__ (9621)
+    Value: 0x59EC0
+    Size: 404
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN5Eigen15TensorEvaluatorINS_9TensorMapINS_6TensorIfLi1ELi1ElEELi16ENS_11MakePointerEEENS_13DefaultDeviceEE8coeffRefElE19__PRETTY_FUNCTION__ (9764)
+    Value: 0x59D20
+    Size: 408
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: group_by_slots.cc (9922)
+    Value: 0x0
+    Size: 0
+    Binding: Local (0x0)
+    Type: File (0x4)
+    Other: 0
+    Section: Absolute (0xFFF1)
+  }
+  Symbol {
+    Name: _ZZNKUlPKN10tensorflow9KernelDefEE_clES2_ENUlPNS_20OpKernelConstructionEE_4_FUNES5_ (39)
+    Value: 0x3DC20
+    Size: 79
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZN4absl14lts_2020_09_2311string_view19CheckLengthInternalEmENKUlvE_clEvE19__PRETTY_FUNCTION__ (2117)
+    Value: 0x5A340
+    Size: 113
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZZNK4absl14lts_2020_09_234SpanIKlEixEmENKUlvE_clEvE19__PRETTY_FUNCTION__ (2214)
+    Value: 0x5A2C0
+    Size: 128
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _GLOBAL__sub_I_group_by_slots.cc (9907)
+    Value: 0xC340
+    Size: 283
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZStL8__ioinit (9126)
+    Value: 0x2615C9
+    Size: 1
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: parse_feature_vec.cc (11295)
+    Value: 0x0
+    Size: 0
+    Binding: Local (0x0)
+    Type: File (0x4)
+    Other: 0
+    Section: Absolute (0xFFF1)
+  }
+  Symbol {
+    Name: _ZZNKUlPKN10tensorflow9KernelDefEE_clES2_ENUlPNS_20OpKernelConstructionEE_4_FUNES5_ (39)
+    Value: 0x444C0
+    Size: 79
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZN4absl14lts_2020_09_2311string_view19CheckLengthInternalEmENKUlvE_clEvE19__PRETTY_FUNCTION__ (2117)
+    Value: 0x5C5A0
+    Size: 113
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZZNK4absl14lts_2020_09_234SpanIKlEixEmENKUlvE_clEvE19__PRETTY_FUNCTION__ (2214)
+    Value: 0x5C620
+    Size: 128
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_E9copy_fromERKSF_mE19__PRETTY_FUNCTION__ (9940)
+    Value: 0x5B340
+    Size: 727
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZNK6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_E12test_deletedERKNS_30dense_hashtable_const_iteratorIS3_lS6_SD_SE_S9_SB_EEE19__PRETTY_FUNCTION__ (10146)
+    Value: 0x5A9E0
+    Size: 862
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZNK6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_E10test_emptyEmE19__PRETTY_FUNCTION__ (10410)
+    Value: 0x5BD60
+    Size: 644
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZNK6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_E10test_emptyERKNS_30dense_hashtable_const_iteratorIS3_lS6_SD_SE_S9_SB_EEE19__PRETTY_FUNCTION__ (10614)
+    Value: 0x5AD40
+    Size: 860
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_E13clear_to_sizeEmE19__PRETTY_FUNCTION__ (10876)
+    Value: 0x5B0A0
+    Size: 641
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_EC4ERKSF_mE19__PRETTY_FUNCTION__ (11082)
+    Value: 0x5B620
+    Size: 728
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _GLOBAL__sub_I_parse_feature_vec.cc (11280)
+    Value: 0xC460
+    Size: 283
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZStL8__ioinit (9126)
+    Value: 0x261629
+    Size: 1
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZZNK6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_E13find_positionERS2_E19__PRETTY_FUNCTION__ (11316)
+    Value: 0x5C000
+    Size: 732
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_E15insert_noresizeERKS3_E19__PRETTY_FUNCTION__ (11526)
+    Value: 0x5A6E0
+    Size: 749
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZNK6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_E12test_deletedEmE19__PRETTY_FUNCTION__ (11738)
+    Value: 0x5BAC0
+    Size: 646
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_E12maybe_shrinkEvE19__PRETTY_FUNCTION__ (11944)
+    Value: 0x5B900
+    Size: 434
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_E13set_empty_keyERKS3_E19__PRETTY_FUNCTION__ (12149)
+    Value: 0x5C2E0
+    Size: 673
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: is_in.cc (12374)
+    Value: 0x0
+    Size: 0
+    Binding: Local (0x0)
+    Type: File (0x4)
+    Other: 0
+    Section: Absolute (0xFFF1)
+  }
+  Symbol {
+    Name: _ZZNKUlPKN10tensorflow9KernelDefEE_clES2_ENUlPNS_20OpKernelConstructionEE_4_FUNES5_ (39)
+    Value: 0x4B7C0
+    Size: 79
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZNKUlPKN10tensorflow9KernelDefEE0_clES2_ENUlPNS_20OpKernelConstructionEE_4_FUNES5_ (123)
+    Value: 0x4B810
+    Size: 79
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _GLOBAL__sub_I_is_in.cc (12359)
+    Value: 0xC580
+    Size: 320
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZStL8__ioinit (9126)
+    Value: 0x261639
+    Size: 1
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZZZNK4absl14lts_2020_09_234SpanIKlEixEmENKUlvE_clEvE19__PRETTY_FUNCTION__ (2214)
+    Value: 0x5C720
+    Size: 128
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: reco_ops.cc (15052)
+    Value: 0x0
+    Size: 0
+    Binding: Local (0x0)
+    Type: File (0x4)
+    Other: 0
+    Section: Absolute (0xFFF1)
+  }
+  Symbol {
+    Name: _ZNSt14_Function_base13_Base_managerIUlPN10tensorflow15shape_inference16InferenceContextEE_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation (12383)
+    Value: 0x4DAB0
+    Size: 29
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTIUlPN10tensorflow15shape_inference16InferenceContextEE_ (12529)
+    Value: 0x260A78
+    Size: 16
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZNSt14_Function_base13_Base_managerIUlPN10tensorflow15shape_inference16InferenceContextEE0_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation (12588)
+    Value: 0x4DAD0
+    Size: 29
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTIUlPN10tensorflow15shape_inference16InferenceContextEE0_ (12735)
+    Value: 0x260A88
+    Size: 16
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZNSt14_Function_base13_Base_managerIUlPN10tensorflow15shape_inference16InferenceContextEE1_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation (12795)
+    Value: 0x4DAF0
+    Size: 29
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTIUlPN10tensorflow15shape_inference16InferenceContextEE1_ (12942)
+    Value: 0x260A98
+    Size: 16
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZNSt14_Function_base13_Base_managerIUlPN10tensorflow15shape_inference16InferenceContextEE2_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation (13002)
+    Value: 0x4DB10
+    Size: 29
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTIUlPN10tensorflow15shape_inference16InferenceContextEE2_ (13149)
+    Value: 0x260AA8
+    Size: 16
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZNSt14_Function_base13_Base_managerIUlPN10tensorflow15shape_inference16InferenceContextEE3_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation (13209)
+    Value: 0x4DB30
+    Size: 29
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTIUlPN10tensorflow15shape_inference16InferenceContextEE3_ (13356)
+    Value: 0x260AB8
+    Size: 16
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZNSt14_Function_base13_Base_managerIUlPN10tensorflow15shape_inference16InferenceContextEE4_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation (13416)
+    Value: 0x4DB50
+    Size: 29
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTIUlPN10tensorflow15shape_inference16InferenceContextEE4_ (13563)
+    Value: 0x260AC8
+    Size: 16
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZNSt14_Function_base13_Base_managerIUlPN10tensorflow15shape_inference16InferenceContextEE5_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation (13623)
+    Value: 0x4DB70
+    Size: 29
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTIUlPN10tensorflow15shape_inference16InferenceContextEE5_ (13770)
+    Value: 0x260AD8
+    Size: 16
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZNSs4_Rep10_M_disposeERKSaIcE.part.12 (13830)
+    Value: 0x4DB90
+    Size: 40
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt17_Function_handlerIFN10tensorflow6StatusEPNS0_15shape_inference16InferenceContextEEUlS4_E2_E9_M_invokeERKSt9_Any_dataOS4_ (13869)
+    Value: 0x4DBC0
+    Size: 173
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt17_Function_handlerIFN10tensorflow6StatusEPNS0_15shape_inference16InferenceContextEEUlS4_E0_E9_M_invokeERKSt9_Any_dataOS4_ (13997)
+    Value: 0x4DC70
+    Size: 405
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZN4absl14lts_2020_09_2311string_view19CheckLengthInternalEmENKUlvE_clEvE19__PRETTY_FUNCTION__ (2117)
+    Value: 0x5CAC0
+    Size: 113
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15shape_inference19DimensionOrConstantC2El.part.112 (14125)
+    Value: 0x4F7C0
+    Size: 124
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15shape_inference9DimensionC2El.part.113 (14192)
+    Value: 0x4F870
+    Size: 124
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt17_Function_handlerIFN10tensorflow6StatusEPNS0_15shape_inference16InferenceContextEEUlS4_E1_E9_M_invokeERKSt9_Any_dataOS4_ (14248)
+    Value: 0x4DE10
+    Size: 575
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15shape_inference19DimensionOrConstantC2ENS0_15DimensionHandleE.part.115 (14376)
+    Value: 0x4F910
+    Size: 109
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt17_Function_handlerIFN10tensorflow6StatusEPNS0_15shape_inference16InferenceContextEEUlS4_E3_E9_M_invokeERKSt9_Any_dataOS4_ (14464)
+    Value: 0x4E050
+    Size: 1160
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt17_Function_handlerIFN10tensorflow6StatusEPNS0_15shape_inference16InferenceContextEEUlS4_E5_E9_M_invokeERKSt9_Any_dataOS4_ (14592)
+    Value: 0x4E4E0
+    Size: 1131
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt17_Function_handlerIFN10tensorflow6StatusEPNS0_15shape_inference16InferenceContextEEUlS4_E4_E9_M_invokeERKSt9_Any_dataOS4_ (14720)
+    Value: 0x4E950
+    Size: 1160
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt17_Function_handlerIFN10tensorflow6StatusEPNS0_15shape_inference16InferenceContextEEUlS4_E_E9_M_invokeERKSt9_Any_dataOS4_ (14848)
+    Value: 0x4EDE0
+    Size: 1236
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _Z41__static_initialization_and_destruction_0ii.constprop.120 (14975)
+    Value: 0xC6C0
+    Size: 5637
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZStL8__ioinit (9126)
+    Value: 0x26163A
+    Size: 1
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _GLOBAL__sub_I_reco_ops.cc (15037)
     Value: 0xDCD0
+    Size: 5
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTSUlPN10tensorflow15shape_inference16InferenceContextEE_ (15064)
+    Value: 0x5CB40
+    Size: 56
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZTSUlPN10tensorflow15shape_inference16InferenceContextEE0_ (15123)
+    Value: 0x5CB80
+    Size: 57
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZTSUlPN10tensorflow15shape_inference16InferenceContextEE1_ (15183)
+    Value: 0x5CBC0
+    Size: 57
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZTSUlPN10tensorflow15shape_inference16InferenceContextEE2_ (15243)
+    Value: 0x5CC00
+    Size: 57
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZTSUlPN10tensorflow15shape_inference16InferenceContextEE3_ (15303)
+    Value: 0x5CC40
+    Size: 57
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZTSUlPN10tensorflow15shape_inference16InferenceContextEE4_ (15363)
+    Value: 0x5CC80
+    Size: 57
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZTSUlPN10tensorflow15shape_inference16InferenceContextEE5_ (15423)
+    Value: 0x5CCC0
+    Size: 57
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: crtstuff.c (15483)
+    Value: 0x0
+    Size: 0
+    Binding: Local (0x0)
+    Type: File (0x4)
+    Other: 0
+    Section: Absolute (0xFFF1)
+  }
+  Symbol {
+    Name: deregister_tm_clones (15494)
+    Value: 0xDCE0
+    Size: 0
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: register_tm_clones (15496)
+    Value: 0xDD20
+    Size: 0
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: __do_global_dtors_aux (15515)
+    Value: 0xDD70
+    Size: 0
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: completed.7698 (15537)
+    Value: 0x261490
+    Size: 1
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: __do_global_dtors_aux_fini_array_entry (15552)
+    Value: 0x260560
+    Size: 0
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .fini_array (0x13)
+  }
+  Symbol {
+    Name: frame_dummy (15591)
+    Value: 0xDDB0
+    Size: 0
+    Binding: Local (0x0)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: __frame_dummy_init_array_entry (15603)
+    Value: 0x260518
+    Size: 0
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .init_array (0x12)
+  }
+  Symbol {
+    Name: crtstuff.c (15483)
+    Value: 0x0
+    Size: 0
+    Binding: Local (0x0)
+    Type: File (0x4)
+    Other: 0
+    Section: Absolute (0xFFF1)
+  }
+  Symbol {
+    Name: __FRAME_END__ (15634)
+    Value: 0x5EE90
+    Size: 0
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .eh_frame (0x10)
+  }
+  Symbol {
+    Name:  (0)
+    Value: 0x0
+    Size: 0
+    Binding: Local (0x0)
+    Type: File (0x4)
+    Other: 0
+    Section: Absolute (0xFFF1)
+  }
+  Symbol {
+    Name: __TMC_END__ (15648)
+    Value: 0x261490
+    Size: 0
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data (0x18)
+  }
+  Symbol {
+    Name: _GLOBAL_OFFSET_TABLE_ (15660)
+    Value: 0x261000
+    Size: 0
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .got.plt (0x17)
+  }
+  Symbol {
+    Name: _DYNAMIC (15682)
+    Value: 0x260AE8
+    Size: 0
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .dynamic (0x15)
+  }
+  Symbol {
+    Name: __GNU_EH_FRAME_HDR (15691)
+    Value: 0x5CCFC
+    Size: 0
+    Binding: Local (0x0)
+    Type: None (0x0)
+    Other: 0
+    Section: .eh_frame_hdr (0xF)
+  }
+  Symbol {
+    Name: __dso_handle (15710)
+    Value: 0x261480
+    Size: 0
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data (0x18)
+  }
+  Symbol {
+    Name: DW.ref.__gxx_personality_v0 (15723)
+    Value: 0x261488
+    Size: 8
+    Binding: Local (0x0)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data (0x18)
+  }
+  Symbol {
+    Name: _ZN10tensorflow5OpDefD1Ev (15751)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTS18SplitRaggedBlockOpIlE (15777)
+    Value: 0x59C30
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZNSt17_Function_handlerIFvllEZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_E9_M_invokeERKSt9_Any_dataOlSA_ (15805)
+    Value: 0x444B0
+    Size: 14
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIfED0Ev (15934)
+    Value: 0x29740
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN22FeatureVecToSegmentsOpD0Ev (15965)
+    Value: 0x32BA0
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt17_Function_handlerIFvllEZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_E9_M_invokeERKSt9_Any_dataOlSA_ (15997)
+    Value: 0x21F60
+    Size: 14
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow12OpDefBuilder10SetShapeFnESt8functionIFNS_6StatusEPNS_15shape_inference16InferenceContextEEE (16128)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated (16237)
+    Value: 0x261568
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEE8allocateEm (16345)
+    Value: 0x17C10
+    Size: 596
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15shape_inference19DimensionOrConstantC1El (16425)
+    Value: 0x4F840
+    Size: 36
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt12length_errorC1EPKc (16483)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTSZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_ (16509)
+    Value: 0x59380
+    Size: 70
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow15TensorShapeBaseINS_11TensorShapeEE8dim_sizeEi (16583)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERSC_RKSD_ (16647)
+    Value: 0x15F50
+    Size: 230
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm2EEEvN4absl14lts_2020_09_234SpanIKlEEPSt5arrayIlXT_EE (16813)
+    Value: 0x1DD40
+    Size: 373
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZSt19__throw_logic_errorPKc@@GLIBCXX_3.4 (16929)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZGVZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated (16971)
+    Value: 0x261580
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN20PoolingBySlotsGradOpD0Ev (17082)
+    Value: 0xDF50
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15OpKernelContext10CtxFailureEPKciRKNS_6StatusE (17112)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: __cxa_begin_catch@@CXXABI_1.3 (17175)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEll (17205)
+    Value: 0x320B0
+    Size: 2588
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: memcpy@@GLIBC_2.14 (17289)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated (17308)
+    Value: 0x261518
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZSt17__throw_bad_allocv@@GLIBCXX_3.4 (17417)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN6IsInOpIiED1Ev (17455)
+    Value: 0x4B860
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt9bad_allocD1Ev@@GLIBCXX_3.4 (17473)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextE (17506)
+    Value: 0x29990
+    Size: 8805
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEll (17574)
+    Value: 0x41DC0
+    Size: 9957
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN17ParseFeatureVecOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (17651)
+    Value: 0x261630
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTV18SplitRaggedBlockOpIiE (17757)
+    Value: 0x260798
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated (17785)
+    Value: 0x2614F8
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZNSt18basic_stringstreamIcSt11char_traitsIcESaIcEED1Ev@@GLIBCXX_3.4 (17909)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ITM_deregisterTMCloneTable (17978)
+    Value: 0x0
+    Size: 0
+    Binding: Weak (0x2)
+    Type: None (0x0)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN6IsInOpIlED1Ev (18006)
+    Value: 0x4B8A0
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN17ParseFeatureVecOpD2Ev (18024)
+    Value: 0x44510
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated (18051)
+    Value: 0x261520
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZGVZZN22FeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (18161)
+    Value: 0x2615C0
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
   }
   Symbol {
-    Name: __GLOBAL__sub_I_feature_pooling.cc (29336)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0xE770
-  }
-  Symbol {
-    Name: __ZNSt3__1lsIN10tensorflow8internal15LogMessageFatalENS_12basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEEEEENS_9enable_ifIXaantsr19is_lvalue_referenceIT_EE5valuesr10is_base_ofINS_8ios_baseESB_EE5valueEOSB_E4typeESD_RKT0_ (14569)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0xE8E0
-  }
-  Symbol {
-    Name: __ZZNK3$_0clEPKN10tensorflow9KernelDefEENUlPNS0_20OpKernelConstructionEE_8__invokeES5_ (14819)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0xE910
-  }
-  Symbol {
-    Name: __ZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextE (29371)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0xE960
-  }
-  Symbol {
-    Name: __ZNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEE7seekposENS_4fposI11__mbstate_tEEj (16854)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0xF270
-  }
-  Symbol {
-    Name: __ZNSt3__1lsIN10tensorflow8internal15LogMessageFatalEA27_cEENS_9enable_ifIXaantsr19is_lvalue_referenceIT_EE5valuesr10is_base_ofINS_8ios_baseES6_EE5valueEOS6_E4typeES8_RKT0_ (17582)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0xF2A0
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE7__cloneEv (29432)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0xF2C0
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE7__cloneEPNS0_6__baseIS9_EE (29564)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0xF300
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEclEOxSB_ (29713)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0xF330
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE6targetERKSt9type_info (29842)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0xF420
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE11target_typeEv (29986)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0xF440
-  }
-  Symbol {
-    Name: __GLOBAL__sub_I_get_slot_fids.cc (30123)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0xF450
-  }
-  Symbol {
-    Name: __ZNSt3__1lsIN10tensorflow8internal15LogMessageFatalENS_12basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEEEEENS_9enable_ifIXaantsr19is_lvalue_referenceIT_EE5valuesr10is_base_ofINS_8ios_baseESB_EE5valueEOSB_E4typeESD_RKT0_ (14569)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0xF530
-  }
-  Symbol {
-    Name: __ZZNK3$_0clEPKN10tensorflow9KernelDefEENUlPNS0_20OpKernelConstructionEE_8__invokeES5_ (14819)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0xF560
-  }
-  Symbol {
-    Name: __ZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextE (30156)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0xF5B0
-  }
-  Symbol {
-    Name: __ZNK10tensorflow6Tensor6shapedIxLm2EEENS_6TTypesIT_XT0_ElE11ConstTensorEN4absl14lts_2020_09_234SpanIKxEE (30218)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x10180
-  }
-  Symbol {
-    Name: __ZNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEE7seekposENS_4fposI11__mbstate_tEEj (16854)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x10250
-  }
-  Symbol {
-    Name: __ZNSt3__1lsIN10tensorflow8internal15LogMessageFatalEA27_cEENS_9enable_ifIXaantsr19is_lvalue_referenceIT_EE5valuesr10is_base_ofINS_8ios_baseES6_EE5valueEOS6_E4typeES8_RKT0_ (17582)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x10280
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE7__cloneEv (30324)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x102A0
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE7__cloneEPNS0_6__baseIS9_EE (30457)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x102F0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEclEOxSB_ (30607)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x10330
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE6targetERKSt9type_info (30737)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x10350
+    Name: _ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKS9_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSH_EEEEKNS3_ILln1EKNS3_ILln1EKNS4_INS5_ISH_Li3ELi1ElEELi16ES7_EEEEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE1EE3runERSW_RKSX_ (18272)
+    Value: 0x19EC0
+    Size: 15630
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen8internal19throw_std_bad_allocEv (18678)
+    Value: 0xEA20
+    Size: 50
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated (18720)
+    Value: 0x261560
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTS17ParseFeatureVecOp (18830)
+    Value: 0x5C6A0
+    Size: 20
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZN10tensorflow22CheckNotInComputeAsyncEPNS_15OpKernelContextEPKc (18854)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTI6IsInOpIlE (18920)
+    Value: 0x2609D0
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN10tensorflow4core10RefCountedD0Ev (18935)
+    Value: 0x1DC90
+    Size: 18
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
   }
   Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEE11target_typeEv (30882)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x10370
-  }
-  Symbol {
-    Name: __ZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExx (31020)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x10380
-  }
-  Symbol {
-    Name: __ZN14GroupBySlotsOp12process_slotEiR7FidIteriRiS2_RN5Eigen9TensorMapINS3_6TensorIxLi2ELi1ElEELi16ENS3_11MakePointerEEERNS4_INS5_IfLi2ELi1ElEELi16ES7_EE (31097)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x10910
-  }
-  Symbol {
-    Name: __ZN7FidIter7advanceEv (31250)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x10A20
-  }
-  Symbol {
-    Name: __GLOBAL__sub_I_group_by_slots.cc (31273)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x10C30
-  }
-  Symbol {
-    Name: __ZNSt3__1lsIN10tensorflow8internal15LogMessageFatalENS_12basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEEEEENS_9enable_ifIXaantsr19is_lvalue_referenceIT_EE5valuesr10is_base_ofINS_8ios_baseESB_EE5valueEOSB_E4typeESD_RKT0_ (14569)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x10D10
-  }
-  Symbol {
-    Name: __ZZNK3$_0clEPKN10tensorflow9KernelDefEENUlPNS0_20OpKernelConstructionEE_8__invokeES5_ (14819)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x10D40
-  }
-  Symbol {
-    Name: __ZN6IsInOpIiE7ComputeEPN10tensorflow15OpKernelContextE (31307)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x10D90
-  }
-  Symbol {
-    Name: __ZNSt3__1lsIN10tensorflow8internal15LogMessageFatalEA27_cEENS_9enable_ifIXaantsr19is_lvalue_referenceIT_EE5valuesr10is_base_ofINS_8ios_baseES6_EE5valueEOS6_E4typeES8_RKT0_ (17582)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x11590
-  }
-  Symbol {
-    Name: __ZNSt3__1L20__throw_length_errorEPKc (17408)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x115B0
-  }
-  Symbol {
-    Name: __ZNSt12length_errorC1EPKc (17446)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x11600
-  }
-  Symbol {
-    Name: __ZNSt3__112__hash_tableIiNS_4hashIiEENS_8equal_toIiEENS_9allocatorIiEEE6rehashEm (31363)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x11630
-  }
-  Symbol {
-    Name: __ZNSt3__112__hash_tableIiNS_4hashIiEENS_8equal_toIiEENS_9allocatorIiEEE8__rehashEm (31445)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
+    Name: _ZN10tensorflow15shape_inference19DimensionOrConstantC1ENS0_15DimensionHandleE (18972)
+    Value: 0x4F980
+    Size: 25
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _fini (19051)
+    Value: 0x520C0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: .fini (0xD)
+  }
+  Symbol {
+    Name: _Znwm@@GLIBCXX_3.4 (19057)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: memmove@@GLIBC_2.2.5 (19076)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow11register_op19OpDefBuilderWrapperclEv (19097)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: __assert_fail@@GLIBC_2.2.5 (19151)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTS16PoolingBySlotsOp (19178)
+    Value: 0x59340
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal10LogMessageC1EPKcii (19201)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN30UnsortedFeatureVecToSegmentsOpD1Ev (19246)
+    Value: 0x32BC0
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTI30UnsortedFeatureVecToSegmentsOp (19286)
+    Value: 0x260840
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZTI6IsInOpIiE (19323)
+    Value: 0x2609B8
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN10tensorflow12OpDefBuilder4AttrESs (19338)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: free@@GLIBC_2.2.5 (19376)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow6Tensor9CheckTypeENS_8DataTypeE (19394)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTV14GroupBySlotsOp (19442)
+    Value: 0x260910
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: __cxa_finalize@@GLIBC_2.2.5 (19463)
+    Value: 0x0
+    Size: 0
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev (19491)
+    Value: 0x4B8E0
+    Size: 119
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTVSt15basic_stringbufIcSt11char_traitsIcESaIcEE@@GLIBCXX_3.4 (19686)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow6StatusC1ENS_5error4CodeEN4absl14lts_2020_09_2311string_viewEOSt6vectorINS_10StackFrameESaIS7_EE (19749)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow11TensorShape10IsSameSizeERKS0_ (19861)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEll (19909)
+    Value: 0x2F120
+    Size: 3331
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal17MakeCheckOpStringIliEEPSsRKT_RKT0_PKc (19993)
     Value: 0x11760
+    Size: 150
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
   }
   Symbol {
-    Name: __ZZNK3$_1clEPKN10tensorflow9KernelDefEENUlPNS0_20OpKernelConstructionEE_8__invokeES5_ (24569)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x119C0
-  }
-  Symbol {
-    Name: __ZN6IsInOpIxE7ComputeEPN10tensorflow15OpKernelContextE (31529)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x11A10
-  }
-  Symbol {
-    Name: __ZNK10tensorflow6Tensor6shapedIxLm1EEENS_6TTypesIT_XT0_ElE11ConstTensorEN4absl14lts_2020_09_234SpanIKxEE (31585)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x12250
-  }
-  Symbol {
-    Name: __ZNSt3__112__hash_tableIxNS_4hashIxEENS_8equal_toIxEENS_9allocatorIxEEE6rehashEm (31691)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x12300
-  }
-  Symbol {
-    Name: __ZNSt3__112__hash_tableIxNS_4hashIxEENS_8equal_toIxEENS_9allocatorIxEEE8__rehashEm (31773)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x12430
-  }
-  Symbol {
-    Name: __GLOBAL__sub_I_is_in.cc (31857)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x12690
-  }
-  Symbol {
-    Name: __ZNSt3__1lsIN10tensorflow8internal15LogMessageFatalENS_12basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEEEEENS_9enable_ifIXaantsr19is_lvalue_referenceIT_EE5valuesr10is_base_ofINS_8ios_baseESB_EE5valueEOSB_E4typeESD_RKT0_ (14569)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x12820
-  }
-  Symbol {
-    Name: __ZZNK3$_0clEPKN10tensorflow9KernelDefEENUlPNS0_20OpKernelConstructionEE_8__invokeES5_ (14819)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x12850
-  }
-  Symbol {
-    Name: __ZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextE (31882)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x128A0
-  }
-  Symbol {
-    Name: __ZNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEE7seekposENS_4fposI11__mbstate_tEEj (16854)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x132B0
-  }
-  Symbol {
-    Name: __ZNSt3__1lsIN10tensorflow8internal15LogMessageFatalEA27_cEENS_9enable_ifIXaantsr19is_lvalue_referenceIT_EE5valuesr10is_base_ofINS_8ios_baseES6_EE5valueEOS6_E4typeES8_RKT0_ (17582)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x132E0
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE7__cloneEv (31951)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x13300
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE7__cloneEPNS0_6__baseISA_EE (32091)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x13340
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEclEOxSC_ (32248)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x13370
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE6targetERKSt9type_info (32385)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x13390
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE11target_typeEv (32537)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x133B0
-  }
-  Symbol {
-    Name: __ZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExx (32682)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x133C0
-  }
-  Symbol {
-    Name: __ZZNK3$_1clEPKN10tensorflow9KernelDefEENUlPNS0_20OpKernelConstructionEE_8__invokeES5_ (24569)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x13EA0
-  }
-  Symbol {
-    Name: __ZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextE (32766)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x13EF0
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE7__cloneEv (32835)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x14910
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE7__cloneEPNS0_6__baseISA_EE (32975)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x14950
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEclEOxSC_ (33132)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x14980
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE6targetERKSt9type_info (33269)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x149A0
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE11target_typeEv (33421)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x149C0
-  }
-  Symbol {
-    Name: __ZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExx (33566)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x149D0
-  }
-  Symbol {
-    Name: __ZZNK3$_2clEPKN10tensorflow9KernelDefEENUlPNS0_20OpKernelConstructionEE_8__invokeES5_ (33650)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x14FA0
-  }
-  Symbol {
-    Name: __ZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextE (33737)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x14FF0
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE7__cloneEv (33806)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x15A20
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE7__cloneEPNS0_6__baseISA_EE (33946)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x15A60
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEclEOxSC_ (34103)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x15A90
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE6targetERKSt9type_info (34240)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x15AB0
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEE11target_typeEv (34392)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x15AD0
-  }
-  Symbol {
-    Name: __ZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExx (34537)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x15AE0
-  }
-  Symbol {
-    Name: __GLOBAL__sub_I_split_ragged_block.cc (34621)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x16640
-  }
-  Symbol {
-    Name: __ZNSt3__1lsIN10tensorflow8internal15LogMessageFatalENS_12basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEEEEENS_9enable_ifIXaantsr19is_lvalue_referenceIT_EE5valuesr10is_base_ofINS_8ios_baseESB_EE5valueEOSB_E4typeESD_RKT0_ (14569)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x16870
-  }
-  Symbol {
-    Name: __ZN10tensorflow11register_op19OpDefBuilderWrapper10SetShapeFnENSt3__18functionIFNS_6StatusEPNS_15shape_inference16InferenceContextEEEE (34659)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x168A0
-  }
-  Symbol {
-    Name: __ZN10tensorflow8internal17MakeCheckOpStringIiiEEPNSt3__112basic_stringIcNS2_11char_traitsIcEENS2_9allocatorIcEEEERKT_RKT0_PKc (34795)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x16980
-  }
-  Symbol {
-    Name: __ZN10tensorflow11register_op19OpDefBuilderWrapperC2EPKc (34922)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x16A00
-  }
-  Symbol {
-    Name: __ZN10tensorflow12OpDefBuilderD2Ev (34979)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x16AE0
-  }
-  Symbol {
-    Name: __ZNSt3__1L20__throw_length_errorEPKc (17408)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x16CE0
-  }
-  Symbol {
-    Name: __ZNSt12length_errorC1EPKc (17446)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x16D30
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED1Ev (35014)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x16D60
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED0Ev (35137)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x16D70
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEv (35260)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x16D80
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEPNS0_6__baseISA_EE (35390)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x16DA0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7destroyEv (35537)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x16DB0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE18destroy_deallocateEv (35666)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x16DC0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEclEOS9_ (35807)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x16DD0
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE6targetERKSt9type_info (35933)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17120
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE11target_typeEv (36075)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17140
-  }
-  Symbol {
-    Name: __ZNSt3__1lsIN10tensorflow8internal15LogMessageFatalExEENS_9enable_ifIXaantsr19is_lvalue_referenceIT_EE5valuesr10is_base_ofINS_8ios_baseES5_EE5valueEOS5_E4typeES7_RKT0_ (36210)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17150
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED1Ev (36379)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17160
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED0Ev (36502)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17170
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEv (36625)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17180
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEPNS0_6__baseISA_EE (36755)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x171A0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7destroyEv (36902)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x171B0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE18destroy_deallocateEv (37031)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x171C0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEclEOS9_ (37172)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x171D0
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE6targetERKSt9type_info (37298)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17670
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE11target_typeEv (37440)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17690
-  }
-  Symbol {
-    Name: __ZN10tensorflow15shape_inference16InferenceContext3DimENS0_11ShapeHandleEx (37575)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x176A0
-  }
-  Symbol {
-    Name: __ZN10tensorflow15shape_inference16InferenceContext12DimKnownRankENS0_11ShapeHandleEx (37651)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x17800
-  }
-  Symbol {
-    Name: __ZNSt3__1lsIN10tensorflow8internal15LogMessageFatalEA43_cEENS_9enable_ifIXaantsr19is_lvalue_referenceIT_EE5valuesr10is_base_ofINS_8ios_baseES6_EE5valueEOS6_E4typeES8_RKT0_ (37737)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x178C0
-  }
-  Symbol {
-    Name: __ZNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEE7seekposENS_4fposI11__mbstate_tEEj (16854)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x178E0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED1Ev (37910)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17910
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED0Ev (38033)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17920
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEv (38156)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17930
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEPNS0_6__baseISA_EE (38286)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17950
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7destroyEv (38433)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17960
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE18destroy_deallocateEv (38562)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17970
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEclEOS9_ (38703)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17980
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE6targetERKSt9type_info (38829)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17CF0
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE11target_typeEv (38971)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17D10
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED1Ev (39106)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17D20
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED0Ev (39229)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17D30
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEv (39352)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17D40
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEPNS0_6__baseISA_EE (39482)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17D60
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7destroyEv (39629)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17D70
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE18destroy_deallocateEv (39758)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17D80
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEclEOS9_ (39899)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17D90
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE6targetERKSt9type_info (40025)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17EF0
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE11target_typeEv (40167)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17F10
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED1Ev (40302)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17F20
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED0Ev (40425)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17F30
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEv (40548)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17F40
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEPNS0_6__baseISA_EE (40678)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17F60
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7destroyEv (40825)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17F70
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE18destroy_deallocateEv (40954)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17F80
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEclEOS9_ (41095)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x17F90
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE6targetERKSt9type_info (41221)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x18210
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE11target_typeEv (41363)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x18230
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED1Ev (41498)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x18240
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEED0Ev (41621)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x18250
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEv (41744)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x18260
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7__cloneEPNS0_6__baseISA_EE (41874)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x18280
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE7destroyEv (42021)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x18290
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE18destroy_deallocateEv (42150)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x182A0
-  }
-  Symbol {
-    Name: __ZNSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEclEOS9_ (42291)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x182B0
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE6targetERKSt9type_info (42417)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x18330
-  }
-  Symbol {
-    Name: __ZNKSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEE11target_typeEv (42559)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x18350
-  }
-  Symbol {
-    Name: __GLOBAL__sub_I_reco_ops.cc (42694)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x18360
-  }
-  Symbol {
-    Name: __ZN10tensorflow6StatusC1ENS_5error4CodeEN4absl14lts_2020_09_2311string_viewE.cold.1 (42722)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x196E0
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS3_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKSA_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSI_EEEEKNS3_ILln1EKNS4_INS5_ISI_Li2ELi1ElEELi16ES7_EEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE0EE3runERSV_RKSW_.cold.1 (42807)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19740
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS3_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKSA_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSI_EEEEKNS3_ILln1EKNS4_INS5_ISI_Li2ELi1ElEELi16ES7_EEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE0EE3runERSV_RKSW_.cold.2 (43220)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19770
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS3_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKSA_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSI_EEEEKNS3_ILln1EKNS4_INS5_ISI_Li2ELi1ElEELi16ES7_EEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE0EE3runERSV_RKSW_.cold.3 (43633)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x197A0
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS3_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKSA_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSI_EEEEKNS3_ILln1EKNS4_INS5_ISI_Li2ELi1ElEELi16ES7_EEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE0EE3runERSV_RKSW_.cold.4 (44046)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x197D0
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS3_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKSA_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSI_EEEEKNS3_ILln1EKNS4_INS5_ISI_Li2ELi1ElEELi16ES7_EEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE0EE3runERSV_RKSW_.cold.5 (44459)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19800
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERS9_RKSA_.cold.1 (44872)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19830
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERS9_RKSA_.cold.2 (45043)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19860
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERS9_RKSA_.cold.3 (45214)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19890
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_.cold.1 (45385)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x198C0
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_.cold.2 (45544)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x198F0
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_.cold.3 (45703)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19920
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_.cold.1 (45862)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19950
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_.cold.2 (46023)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19980
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_.cold.3 (46184)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x199B0
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f.cold.1 (46345)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x199E0
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f.cold.2 (46532)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19A10
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f.cold.3 (46719)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19A40
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f.cold.4 (46906)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19A70
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f.cold.5 (47093)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19AA0
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f.cold.1 (47280)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19AD0
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f.cold.2 (47455)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19B00
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f.cold.3 (47630)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19B30
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f.cold.4 (47805)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19B60
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE11writePacketILi0EEEvlRKDv4_f.cold.5 (47980)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19B90
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE8coeffRefEl.cold.1 (48155)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19BC0
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE8coeffRefEl.cold.2 (48324)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19BF0
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE8coeffRefEl.cold.3 (48493)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19C20
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE8coeffRefEl.cold.4 (48662)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19C50
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE8coeffRefEl.cold.5 (48831)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19C80
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.1 (49000)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19CB0
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.2 (49180)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19CE0
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.3 (49360)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19D10
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.4 (49540)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19D40
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.5 (49720)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19D70
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.6 (49900)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19DA0
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.1 (50080)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19DD0
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.2 (50248)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19E00
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.3 (50416)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19E30
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.4 (50584)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19E60
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.5 (50752)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19E90
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5coeffEl.cold.1 (50920)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19EC0
+    Name: _ZN18SplitRaggedBlockOpIlED2Ev (20057)
+    Value: 0x297A0
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal10LogMessage16VmoduleActivatedEPKci (20088)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
   }
   Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5coeffEl.cold.2 (51088)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19EF0
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5coeffEl.cold.3 (51256)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19F20
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5coeffEl.cold.4 (51424)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19F50
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5coeffEl.cold.5 (51592)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19F80
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.1 (51760)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19FB0
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.2 (51930)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x19FE0
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.3 (52100)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A010
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.4 (52270)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A040
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE6packetILi0EEEDv4_fl.cold.5 (52440)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A070
-  }
-  Symbol {
-    Name: __ZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextE.cold.1 (52610)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A0A0
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKS9_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSH_EEEEKNS3_ILln1EKNS3_ILln1EKNS4_INS5_ISH_Li3ELi1ElEELi16ES7_EEEEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE1EE3runERSW_RKSX_.cold.1 (52685)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A0D0
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKS9_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSH_EEEEKNS3_ILln1EKNS3_ILln1EKNS4_INS5_ISH_Li3ELi1ElEELi16ES7_EEEEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE1EE3runERSW_RKSX_.cold.2 (53099)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A100
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_.cold.1 (53513)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A130
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_.cold.2 (53672)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A160
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_.cold.3 (53831)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A190
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERSC_RKSD_.cold.1 (53990)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A1C0
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERSC_RKSD_.cold.2 (54164)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A1F0
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERSC_RKSD_.cold.3 (54338)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A220
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_.cold.1 (54512)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A250
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_.cold.2 (54673)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A280
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_.cold.3 (54834)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A2B0
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal17TensorBlockMapperILi1ELi1ElE25InitializeBlockDimensionsEv.cold.1 (54995)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A2E0
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal17TensorBlockMapperILi1ELi1ElE25InitializeBlockDimensionsEv.cold.2 (55081)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A310
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal17TensorBlockMapperILi1ELi1ElE25InitializeBlockDimensionsEv.cold.3 (55167)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A340
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE10writeBlockINS_8internal22TensorCwiseBinaryBlockINSB_13scalar_sum_opIffEENSB_23TensorMaterializedBlockIfLi1ELi1ElEENSB_21TensorCwiseUnaryBlockINSB_10bind1st_opINSB_17scalar_product_opIKfSK_EEEESG_EEEEEEvRKNSB_21TensorBlockDescriptorILi1ElEERKT_.cold.1 (55253)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A370
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE10writeBlockINS_8internal22TensorCwiseBinaryBlockINSB_13scalar_sum_opIffEENSB_23TensorMaterializedBlockIfLi1ELi1ElEENSB_21TensorCwiseUnaryBlockINSB_10bind1st_opINSB_17scalar_product_opIKfSK_EEEESG_EEEEEEvRKNSB_21TensorBlockDescriptorILi1ElEERKT_.cold.2 (55644)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A3A0
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE10writeBlockINS_8internal22TensorCwiseBinaryBlockINSB_13scalar_sum_opIffEENSB_23TensorMaterializedBlockIfLi1ELi1ElEENSB_21TensorCwiseUnaryBlockINSB_10bind1st_opINSB_17scalar_product_opIKfSK_EEEESG_EEEEEEvRKNSB_21TensorBlockDescriptorILi1ElEERKT_.cold.3 (56035)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A3D0
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE10writeBlockINS_8internal22TensorCwiseBinaryBlockINSB_13scalar_sum_opIffEENSB_23TensorMaterializedBlockIfLi1ELi1ElEENSB_21TensorCwiseUnaryBlockINSB_10bind1st_opINSB_17scalar_product_opIKfSK_EEEESG_EEEEEEvRKNSB_21TensorBlockDescriptorILi1ElEERKT_.cold.4 (56426)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A400
-  }
-  Symbol {
-    Name: __ZN5Eigen15TensorEvaluatorINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE10writeBlockINS_8internal22TensorCwiseBinaryBlockINSB_13scalar_sum_opIffEENSB_23TensorMaterializedBlockIfLi1ELi1ElEENSB_21TensorCwiseUnaryBlockINSB_10bind1st_opINSB_17scalar_product_opIKfSK_EEEESG_EEEEEEvRKNSB_21TensorBlockDescriptorILi1ElEERKT_.cold.5 (56817)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A430
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSB_27TensorBlockScratchAllocatorIS9_EEb.cold.1 (57208)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A460
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSB_27TensorBlockScratchAllocatorIS9_EEb.cold.2 (57448)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A490
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSB_27TensorBlockScratchAllocatorIS9_EEb.cold.3 (57688)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A4C0
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSB_27TensorBlockScratchAllocatorIS9_EEb.cold.4 (57928)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A4F0
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSB_27TensorBlockScratchAllocatorIS9_EEb.cold.5 (58168)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A520
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSB_27TensorBlockScratchAllocatorIS9_EEb.cold.6 (58408)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A550
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSB_27TensorBlockScratchAllocatorIS9_EEb.cold.7 (58648)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A580
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSB_27TensorBlockScratchAllocatorIS9_EEb.cold.8 (58888)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A5B0
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_9TensorMapIKNS_6TensorIfLi2ELi1ElEELi0ENS_11MakePointerEEElE3RunERKNS8_6TargetERKS7_.cold.1 (59128)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A5E0
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_9TensorMapIKNS_6TensorIfLi2ELi1ElEELi0ENS_11MakePointerEEElE3RunERKNS8_6TargetERKS7_.cold.2 (59271)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A610
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_9TensorMapIKNS_6TensorIfLi2ELi1ElEELi0ENS_11MakePointerEEElE3RunERKNS8_6TargetERKS7_.cold.3 (59414)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A640
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal23TensorMaterializedBlockIfLi2ELi1ElE11materializeINS_6DSizesIlLi2EEENS0_27TensorBlockScratchAllocatorINS_13DefaultDeviceEEEEES2_PKfRKT_RNS0_21TensorBlockDescriptorILi2ElEERT0_.cold.1 (59557)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A670
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEE8allocateEm.cold.1 (59760)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A6A0
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEE8allocateEm.cold.2 (59848)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A6D0
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEE8allocateEm.cold.3 (59936)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A700
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal13TensorBlockIOIflLi2ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi2EEE.cold.1 (60024)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A730
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal13TensorBlockIOIflLi2ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi2EEE.cold.2 (60126)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A760
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSF_27TensorBlockScratchAllocatorISD_EEb.cold.1 (60228)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A790
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSF_27TensorBlockScratchAllocatorISD_EEb.cold.2 (60483)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A7C0
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSF_27TensorBlockScratchAllocatorISD_EEb.cold.3 (60738)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A7F0
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSF_27TensorBlockScratchAllocatorISD_EEb.cold.4 (60993)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A820
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSF_27TensorBlockScratchAllocatorISD_EEb.cold.5 (61248)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A850
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSF_27TensorBlockScratchAllocatorISD_EEb.cold.6 (61503)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A880
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi1ElEERNSF_27TensorBlockScratchAllocatorISD_EEb.cold.7 (61758)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A8B0
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi2ElEERNSD_27TensorBlockScratchAllocatorISB_EEb.cold.1 (62013)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A8E0
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi2ElEERNSD_27TensorBlockScratchAllocatorISB_EEb.cold.2 (62255)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A910
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi2ElEERNSD_27TensorBlockScratchAllocatorISB_EEb.cold.3 (62497)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A940
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi2ElEERNSD_27TensorBlockScratchAllocatorISB_EEb.cold.4 (62739)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A970
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi2ElEERNSD_27TensorBlockScratchAllocatorISB_EEb.cold.5 (62981)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A9A0
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi2ElEERNSD_27TensorBlockScratchAllocatorISB_EEb.cold.6 (63223)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1A9D0
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi2ElEERNSD_27TensorBlockScratchAllocatorISB_EEb.cold.7 (63465)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1AA00
-  }
-  Symbol {
-    Name: __ZNK5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEE5blockERNS_8internal21TensorBlockDescriptorILi2ElEERNSD_27TensorBlockScratchAllocatorISB_EEb.cold.8 (63707)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1AA30
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal21TensorBlockAssignmentIfLi3ENS_9TensorMapIKNS_6TensorIfLi3ELi1ElEELi0ENS_11MakePointerEEElE3RunERKNS8_6TargetERKS7_.cold.1 (63949)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1AA60
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal21TensorBlockAssignmentIfLi3ENS_9TensorMapIKNS_6TensorIfLi3ELi1ElEELi0ENS_11MakePointerEEElE3RunERKNS8_6TargetERKS7_.cold.2 (64092)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1AA90
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal21TensorBlockAssignmentIfLi3ENS_9TensorMapIKNS_6TensorIfLi3ELi1ElEELi0ENS_11MakePointerEEElE3RunERKNS8_6TargetERKS7_.cold.3 (64235)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1AAC0
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal23TensorMaterializedBlockIfLi3ELi1ElE11materializeINS_6DSizesIlLi3EEENS0_27TensorBlockScratchAllocatorINS_13DefaultDeviceEEEEES2_PKfRKT_RNS0_21TensorBlockDescriptorILi3ElEERT0_.cold.1 (64378)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1AAF0
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal13TensorBlockIOIflLi3ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi3EEE.cold.1 (64581)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1AB20
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal13TensorBlockIOIflLi3ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi3EEE.cold.2 (64683)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1AB50
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_17TensorReshapingOpIKNS_6DSizesIlLi2EEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKNS_9TensorMapIKNS_6TensorIfLi1ELi1ElEELi0ENS_11MakePointerEEEKNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSJ_EEEESF_EEEEEElE3RunERKNSR_6TargetERKSQ_.cold.1 (64785)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1AB80
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_17TensorReshapingOpIKNS_6DSizesIlLi2EEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKNS_9TensorMapIKNS_6TensorIfLi1ELi1ElEELi0ENS_11MakePointerEEEKNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSJ_EEEESF_EEEEEElE3RunERKNSR_6TargetERKSQ_.cold.2 (65105)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1ABB0
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_17TensorReshapingOpIKNS_6DSizesIlLi2EEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKNS_9TensorMapIKNS_6TensorIfLi1ELi1ElEELi0ENS_11MakePointerEEEKNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSJ_EEEESF_EEEEEElE3RunERKNSR_6TargetERKSQ_.cold.3 (65425)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1ABE0
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_17TensorReshapingOpIKNS_6DSizesIlLi2EEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKNS_9TensorMapIKNS_6TensorIfLi1ELi1ElEELi0ENS_11MakePointerEEEKNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSJ_EEEESF_EEEEEElE3RunERKNSR_6TargetERKSQ_.cold.4 (65745)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1AC10
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_17TensorReshapingOpIKNS_6DSizesIlLi2EEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKNS_9TensorMapIKNS_6TensorIfLi1ELi1ElEELi0ENS_11MakePointerEEEKNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSJ_EEEESF_EEEEEElE3RunERKNSR_6TargetERKSQ_.cold.5 (66065)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1AC40
-  }
-  Symbol {
-    Name: __ZN5Eigen8internal21TensorBlockAssignmentIfLi2ENS_17TensorReshapingOpIKNS_6DSizesIlLi2EEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKNS_9TensorMapIKNS_6TensorIfLi1ELi1ElEELi0ENS_11MakePointerEEEKNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSJ_EEEESF_EEEEEElE3RunERKNSR_6TargetERKSQ_.cold.6 (66385)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1AC70
-  }
-  Symbol {
-    Name: __ZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextE.cold.1 (66705)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1ACA0
-  }
-  Symbol {
-    Name: __ZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextE.cold.2 (66773)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1ACD0
-  }
-  Symbol {
-    Name: __ZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextE.cold.3 (66841)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1AD00
-  }
-  Symbol {
-    Name: __ZN10tensorflow6StatusC1ENS_5error4CodeEN4absl14lts_2020_09_2311string_viewE.cold.1 (42722)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1AD20
-  }
-  Symbol {
-    Name: __ZN10tensorflow6StatusC1ENS_5error4CodeEN4absl14lts_2020_09_2311string_viewE.cold.1 (42722)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1AD80
-  }
-  Symbol {
-    Name: __ZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextE.cold.1 (66909)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1ADE0
-  }
-  Symbol {
-    Name: __ZN10tensorflow6StatusC1ENS_5error4CodeEN4absl14lts_2020_09_2311string_viewE.cold.1 (42722)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1AE00
-  }
-  Symbol {
-    Name: __ZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextE.cold.1 (66985)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1AE60
-  }
-  Symbol {
-    Name: __ZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextE.cold.1 (67061)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1AE80
-  }
-  Symbol {
-    Name: __ZN10tensorflow11register_op19OpDefBuilderWrapper10SetShapeFnENSt3__18functionIFNS_6StatusEPNS_15shape_inference16InferenceContextEEEE.cold.1 (67137)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1AEA0
-  }
-  Symbol {
-    Name: __ZN10tensorflow6StatusC1ENS_5error4CodeEN4absl14lts_2020_09_2311string_viewE.cold.1 (42722)
-    Type: Section (0xE)
-    Section: __text (0x1)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1AEC0
-  }
-  Symbol {
-    Name: GCC_except_table2 (67280)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B468
-  }
-  Symbol {
-    Name: GCC_except_table5 (67298)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B478
-  }
-  Symbol {
-    Name: GCC_except_table9 (67316)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B51C
-  }
-  Symbol {
-    Name: GCC_except_table10 (67334)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B54C
-  }
-  Symbol {
-    Name: GCC_except_table11 (67353)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B55C
-  }
-  Symbol {
-    Name: GCC_except_table12 (67372)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B56C
-  }
-  Symbol {
-    Name: GCC_except_table13 (67391)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B588
-  }
-  Symbol {
-    Name: GCC_except_table26 (67410)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B598
-  }
-  Symbol {
-    Name: GCC_except_table27 (67429)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B5B0
-  }
-  Symbol {
-    Name: GCC_except_table28 (67448)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B5F4
-  }
-  Symbol {
-    Name: GCC_except_table29 (67467)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B608
-  }
-  Symbol {
-    Name: GCC_except_table34 (67486)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B618
-  }
-  Symbol {
-    Name: GCC_except_table35 (67505)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B644
-  }
-  Symbol {
-    Name: GCC_except_table36 (67524)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B654
-  }
-  Symbol {
-    Name: GCC_except_table37 (67543)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B664
-  }
-  Symbol {
-    Name: GCC_except_table38 (67562)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B674
-  }
-  Symbol {
-    Name: GCC_except_table39 (67581)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B6A0
-  }
-  Symbol {
-    Name: GCC_except_table49 (67600)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B6CC
-  }
-  Symbol {
-    Name: GCC_except_table61 (67619)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B6E8
-  }
-  Symbol {
-    Name: GCC_except_table64 (67638)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B6F8
-  }
-  Symbol {
-    Name: GCC_except_table65 (67657)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B770
-  }
-  Symbol {
-    Name: GCC_except_table66 (67676)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B780
-  }
-  Symbol {
-    Name: GCC_except_table67 (67695)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B798
-  }
-  Symbol {
-    Name: GCC_except_table71 (67714)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B7B0
-  }
-  Symbol {
-    Name: GCC_except_table74 (67733)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B7C8
-  }
-  Symbol {
-    Name: GCC_except_table89 (67752)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B7E0
-  }
-  Symbol {
-    Name: GCC_except_table2 (67280)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B808
-  }
-  Symbol {
-    Name: GCC_except_table5 (67298)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B818
-  }
-  Symbol {
-    Name: GCC_except_table44 (67771)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B88C
-  }
-  Symbol {
-    Name: GCC_except_table2 (67280)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B8A4
-  }
-  Symbol {
-    Name: GCC_except_table5 (67298)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B8B4
-  }
-  Symbol {
-    Name: GCC_except_table10 (67334)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B9AC
-  }
-  Symbol {
-    Name: GCC_except_table46 (67790)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1B9BC
-  }
-  Symbol {
-    Name: GCC_except_table48 (67809)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BA00
-  }
-  Symbol {
-    Name: GCC_except_table49 (67600)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BA1C
-  }
-  Symbol {
-    Name: GCC_except_table2 (67280)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BA34
-  }
-  Symbol {
-    Name: GCC_except_table5 (67298)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BA44
-  }
-  Symbol {
-    Name: GCC_except_table14 (67828)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BA8C
-  }
-  Symbol {
-    Name: GCC_except_table21 (67847)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BA9C
-  }
-  Symbol {
-    Name: GCC_except_table24 (67866)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BAAC
-  }
-  Symbol {
-    Name: GCC_except_table25 (67885)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BAF4
-  }
-  Symbol {
-    Name: GCC_except_table28 (67448)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BB04
-  }
-  Symbol {
-    Name: GCC_except_table2 (67280)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BB2C
-  }
-  Symbol {
-    Name: GCC_except_table5 (67298)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BB3C
-  }
-  Symbol {
-    Name: GCC_except_table44 (67771)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BBCC
-  }
-  Symbol {
-    Name: GCC_except_table45 (67904)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BBE8
-  }
-  Symbol {
-    Name: GCC_except_table48 (67809)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BBF8
-  }
-  Symbol {
-    Name: GCC_except_table58 (67923)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BC88
-  }
-  Symbol {
-    Name: GCC_except_table59 (67942)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BCA4
-  }
-  Symbol {
-    Name: GCC_except_table62 (67961)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BCB4
-  }
-  Symbol {
-    Name: GCC_except_table73 (67980)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BD44
-  }
-  Symbol {
-    Name: GCC_except_table74 (67733)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BD60
-  }
-  Symbol {
-    Name: GCC_except_table2 (67280)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BD9C
-  }
-  Symbol {
-    Name: GCC_except_table3 (67999)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BDB8
-  }
-  Symbol {
-    Name: GCC_except_table4 (68017)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BDC8
-  }
-  Symbol {
-    Name: GCC_except_table6 (68035)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BDDC
-  }
-  Symbol {
-    Name: GCC_except_table16 (68053)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BDEC
-  }
-  Symbol {
-    Name: GCC_except_table26 (67410)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BE0C
-  }
-  Symbol {
-    Name: GCC_except_table31 (68072)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BE38
-  }
-  Symbol {
-    Name: GCC_except_table55 (68091)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BE48
-  }
-  Symbol {
-    Name: GCC_except_table85 (68110)
-    Type: Section (0xE)
-    Section: __gcc_except_tab (0x4)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1BE70
-  }
-  Symbol {
-    Name: __ZTSNSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE (68129)
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1C640
-  }
-  Symbol {
-    Name: __ZTS3$_0 (68251)
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1C713
-  }
-  Symbol {
-    Name: __ZTSNSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE (68261)
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1C718
-  }
-  Symbol {
-    Name: __ZTS3$_1 (68383)
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1C78D
-  }
-  Symbol {
-    Name: __ZTSNSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE (68393)
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1C792
-  }
-  Symbol {
-    Name: __ZTS3$_2 (68515)
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1C807
-  }
-  Symbol {
-    Name: __ZTSNSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE (68525)
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1C80C
-  }
-  Symbol {
-    Name: __ZTS3$_3 (68647)
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1C881
-  }
-  Symbol {
-    Name: __ZTSNSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE (68657)
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1C886
-  }
-  Symbol {
-    Name: __ZTS3$_4 (68779)
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1C8FB
-  }
-  Symbol {
-    Name: __ZTSNSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE (68789)
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1C900
-  }
-  Symbol {
-    Name: __ZTS3$_5 (68911)
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1C975
-  }
-  Symbol {
-    Name: __ZTV16PoolingBySlotsOp (68921)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E2E0
-  }
-  Symbol {
-    Name: __ZTVNSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEEE (68945)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E340
-  }
-  Symbol {
-    Name: __ZTTNSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEEE (69019)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E3B8
-  }
-  Symbol {
-    Name: __ZTCNSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEEE0_NS_14basic_iostreamIcS2_EE (69093)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E408
-  }
-  Symbol {
-    Name: __ZTCNSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEEE0_NS_13basic_istreamIcS2_EE (69195)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E480
-  }
-  Symbol {
-    Name: __ZTCNSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEEE16_NS_13basic_ostreamIcS2_EE (69296)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E4D0
-  }
-  Symbol {
-    Name: __ZTVNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEEE (69398)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E538
-  }
-  Symbol {
-    Name: __ZTVNSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE (69469)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E5D0
-  }
-  Symbol {
-    Name: __ZTV20PoolingBySlotsGradOp (69596)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E660
-  }
-  Symbol {
-    Name: __ZTV13GetSlotFidsOp (69624)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E6C0
-  }
-  Symbol {
-    Name: __ZTVNSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE (69645)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E720
-  }
-  Symbol {
-    Name: __ZTV14GroupBySlotsOp (69769)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E7A0
-  }
-  Symbol {
-    Name: __ZTVNSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE (69791)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E800
-  }
-  Symbol {
-    Name: __ZTV6IsInOpIiE (69916)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E880
-  }
-  Symbol {
-    Name: __ZTV6IsInOpIxE (69932)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E8E0
-  }
-  Symbol {
-    Name: __ZTV18SplitRaggedBlockOpIfE (69948)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E940
-  }
-  Symbol {
-    Name: __ZTVNSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE (69977)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E9A0
-  }
-  Symbol {
-    Name: __ZTV18SplitRaggedBlockOpIiE (70109)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1EA20
-  }
-  Symbol {
-    Name: __ZTVNSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE (70138)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1EA80
-  }
-  Symbol {
-    Name: __ZTV18SplitRaggedBlockOpIxE (70270)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1EB00
-  }
-  Symbol {
-    Name: __ZTVNSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE (70299)
-    PrivateExtern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1EB60
-  }
-  Symbol {
-    Name: __ZTVNSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE (70431)
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1EBE0
-  }
-  Symbol {
-    Name: __ZTINSt3__110__function6__funcI3$_0NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE (70553)
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1EC48
-  }
-  Symbol {
-    Name: __ZTI3$_0 (70675)
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1EC60
-  }
-  Symbol {
-    Name: __ZTVNSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE (70685)
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1EC70
-  }
-  Symbol {
-    Name: __ZTINSt3__110__function6__funcI3$_1NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE (70807)
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1ECC8
-  }
-  Symbol {
-    Name: __ZTI3$_1 (70929)
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1ECE0
-  }
-  Symbol {
-    Name: __ZTVNSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE (70939)
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1ECF0
-  }
-  Symbol {
-    Name: __ZTINSt3__110__function6__funcI3$_2NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE (71061)
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1ED48
-  }
-  Symbol {
-    Name: __ZTI3$_2 (71183)
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1ED60
-  }
-  Symbol {
-    Name: __ZTVNSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE (71193)
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1ED70
-  }
-  Symbol {
-    Name: __ZTINSt3__110__function6__funcI3$_3NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE (71315)
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1EDC8
-  }
-  Symbol {
-    Name: __ZTI3$_3 (71437)
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1EDE0
-  }
-  Symbol {
-    Name: __ZTVNSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE (71447)
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1EDF0
-  }
-  Symbol {
-    Name: __ZTINSt3__110__function6__funcI3$_4NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE (71569)
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1EE48
-  }
-  Symbol {
-    Name: __ZTI3$_4 (71691)
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1EE60
-  }
-  Symbol {
-    Name: __ZTVNSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE (71701)
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1EE70
-  }
-  Symbol {
-    Name: __ZTINSt3__110__function6__funcI3$_5NS_9allocatorIS2_EEFN10tensorflow6StatusEPNS5_15shape_inference16InferenceContextEEEE (71823)
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1EEC8
-  }
-  Symbol {
-    Name: __ZTI3$_5 (71945)
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1EEE0
-  }
-  Symbol {
-    Name: __dyld_private (71955)
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F2B0
-  }
-  Symbol {
-    Name: __ZN5EigenL4lastE (71970)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F428
-  }
-  Symbol {
-    Name: __ZN5EigenL6lastp1E (71988)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F429
-  }
-  Symbol {
-    Name: __ZN5EigenL3allE (72008)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F42B
-  }
-  Symbol {
-    Name: __ZL17register_kernel_0 (72025)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F42C
-  }
-  Symbol {
-    Name: __ZL17register_kernel_1 (72049)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F42D
-  }
-  Symbol {
-    Name: __ZN5EigenL4lastE (71970)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F42E
-  }
-  Symbol {
-    Name: __ZN5EigenL6lastp1E (71988)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F42F
-  }
-  Symbol {
-    Name: __ZN5EigenL3allE (72008)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F431
-  }
-  Symbol {
-    Name: __ZL17register_kernel_0 (72025)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F432
-  }
-  Symbol {
-    Name: __ZN5EigenL4lastE (71970)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F433
-  }
-  Symbol {
-    Name: __ZN5EigenL6lastp1E (71988)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F434
-  }
-  Symbol {
-    Name: __ZN5EigenL3allE (72008)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F436
-  }
-  Symbol {
-    Name: __ZL17register_kernel_0 (72025)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F437
-  }
-  Symbol {
-    Name: __ZN5EigenL4lastE (71970)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F438
-  }
-  Symbol {
-    Name: __ZN5EigenL6lastp1E (71988)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F439
-  }
-  Symbol {
-    Name: __ZN5EigenL3allE (72008)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F43B
-  }
-  Symbol {
-    Name: __ZL17register_kernel_0 (72025)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F43C
-  }
-  Symbol {
-    Name: __ZL17register_kernel_1 (72049)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F43D
-  }
-  Symbol {
-    Name: __ZN5EigenL4lastE (71970)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F43E
-  }
-  Symbol {
-    Name: __ZN5EigenL6lastp1E (71988)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F43F
-  }
-  Symbol {
-    Name: __ZN5EigenL3allE (72008)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F441
-  }
-  Symbol {
-    Name: __ZL17register_kernel_0 (72025)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F442
-  }
-  Symbol {
-    Name: __ZL17register_kernel_1 (72049)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F443
-  }
-  Symbol {
-    Name: __ZL17register_kernel_2 (72073)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F444
-  }
-  Symbol {
-    Name: __ZN5EigenL4lastE (71970)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F448
-  }
-  Symbol {
-    Name: __ZN5EigenL6lastp1E (71988)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F449
-  }
-  Symbol {
-    Name: __ZN5EigenL3allE (72008)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F44B
-  }
-  Symbol {
-    Name: __ZL12register_op0 (72097)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F44C
-  }
-  Symbol {
-    Name: __ZL12register_op1 (72116)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F44D
-  }
-  Symbol {
-    Name: __ZL12register_op2 (72135)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F44E
-  }
-  Symbol {
-    Name: __ZL12register_op3 (72154)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F44F
-  }
-  Symbol {
-    Name: __ZL12register_op4 (72173)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F450
-  }
-  Symbol {
-    Name: __ZL12register_op5 (72192)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F451
-  }
-  Symbol {
-    Name: __ZZZNK3$_0clEPN10tensorflow15shape_inference16InferenceContextEENKUliPKcE_clEiS5_E17vmodule_activated (72211)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F452
-  }
-  Symbol {
-    Name: __ZGVZZNK3$_0clEPN10tensorflow15shape_inference16InferenceContextEENKUliPKcE_clEiS5_E17vmodule_activated (72314)
-    Type: Section (0xE)
-    Section: __bss (0xD)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x0)
-    ]
-    Value: 0x1F458
-  }
-  Symbol {
-    Name: __ZGVZN5Eigen8internal20manage_caching_sizesENS_6ActionEPlS2_S2_E12m_cacheSizes (2)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F300
-  }
-  Symbol {
-    Name: __ZGVZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS4_E17vmodule_activated (82)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F320
-  }
-  Symbol {
-    Name: __ZGVZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (187)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F310
-  }
-  Symbol {
-    Name: __ZGVZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (291)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F2C0
-  }
-  Symbol {
-    Name: __ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated (397)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F380
-  }
-  Symbol {
-    Name: __ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated (509)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F390
-  }
-  Symbol {
-    Name: __ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated (621)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F370
-  }
-  Symbol {
-    Name: __ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated (732)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F3C0
-  }
-  Symbol {
-    Name: __ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated (844)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F3D0
-  }
-  Symbol {
-    Name: __ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated (956)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F3B0
-  }
-  Symbol {
-    Name: __ZGVZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated (1067)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F400
-  }
-  Symbol {
-    Name: __ZGVZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated (1179)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F410
-  }
-  Symbol {
-    Name: __ZGVZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated (1291)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F3F0
-  }
-  Symbol {
-    Name: __ZGVZZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (1402)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F2E0
-  }
-  Symbol {
-    Name: __ZGVZZN7FidIter7advanceEvENKUliPKcE_clEiS1_E17vmodule_activated (1512)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F340
-  }
-  Symbol {
-    Name: __ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE0_clEiS5_E17vmodule_activated (1577)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F350
-  }
-  Symbol {
-    Name: __ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE1_clEiS5_E17vmodule_activated (1697)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F360
-  }
-  Symbol {
-    Name: __ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS5_E17vmodule_activated (1817)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F330
-  }
-  Symbol {
-    Name: __ZGVZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS5_E17vmodule_activated (1936)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F2D0
-  }
-  Symbol {
-    Name: __ZGVZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated (2057)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F3A0
-  }
-  Symbol {
-    Name: __ZGVZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated (2183)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F3E0
-  }
-  Symbol {
-    Name: __ZGVZZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated (2309)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F420
-  }
-  Symbol {
-    Name: __ZTI13GetSlotFidsOp (2435)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E708
-  }
-  Symbol {
-    Name: __ZTI14GroupBySlotsOp (2456)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E7E8
-  }
-  Symbol {
-    Name: __ZTI16PoolingBySlotsOp (2478)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E328
-  }
-  Symbol {
-    Name: __ZTI18SplitRaggedBlockOpIfE (2502)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E988
-  }
-  Symbol {
-    Name: __ZTI18SplitRaggedBlockOpIiE (2531)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1EA68
-  }
-  Symbol {
-    Name: __ZTI18SplitRaggedBlockOpIxE (2560)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1EB48
-  }
-  Symbol {
-    Name: __ZTI20PoolingBySlotsGradOp (2589)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E6A8
-  }
-  Symbol {
-    Name: __ZTI6IsInOpIiE (2617)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E8C8
-  }
-  Symbol {
-    Name: __ZTI6IsInOpIxE (2633)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E928
-  }
-  Symbol {
-    Name: __ZTINSt3__110__function6__baseIFN10tensorflow6StatusEPNS2_15shape_inference16InferenceContextEEEE (2649)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1EC38
-  }
-  Symbol {
-    Name: __ZTINSt3__110__function6__baseIFvxxEEE (2748)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E628
-  }
-  Symbol {
-    Name: __ZTINSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE (2788)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E778
-  }
-  Symbol {
-    Name: __ZTINSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE (2912)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E858
-  }
-  Symbol {
-    Name: __ZTINSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE (3037)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E638
-  }
-  Symbol {
-    Name: __ZTINSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE (3164)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E9F8
-  }
-  Symbol {
-    Name: __ZTINSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE (3296)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1EAD8
-  }
-  Symbol {
-    Name: __ZTINSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE (3428)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1EBB8
-  }
-  Symbol {
-    Name: __ZTINSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEEE (3560)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E5B8
-  }
-  Symbol {
-    Name: __ZTINSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEEE (3631)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E520
-  }
-  Symbol {
-    Name: __ZTIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_ (3705)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E790
-  }
-  Symbol {
-    Name: __ZTIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_ (3776)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E870
-  }
-  Symbol {
-    Name: __ZTIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_ (3848)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1E650
-  }
-  Symbol {
-    Name: __ZTIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_ (3922)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1EA10
-  }
-  Symbol {
-    Name: __ZTIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_ (4001)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1EAF0
-  }
-  Symbol {
-    Name: __ZTIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_ (4080)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0xA)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1EBD0
-  }
-  Symbol {
-    Name: __ZTS13GetSlotFidsOp (4159)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C1AB
-  }
-  Symbol {
-    Name: __ZTS14GroupBySlotsOp (4180)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C274
-  }
-  Symbol {
-    Name: __ZTS16PoolingBySlotsOp (4202)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C018
-  }
-  Symbol {
-    Name: __ZTS18SplitRaggedBlockOpIfE (4226)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C35A
-  }
-  Symbol {
-    Name: __ZTS18SplitRaggedBlockOpIiE (4255)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C43B
-  }
-  Symbol {
-    Name: __ZTS18SplitRaggedBlockOpIxE (4284)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C51C
-  }
-  Symbol {
-    Name: __ZTS20PoolingBySlotsGradOp (4313)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C194
-  }
-  Symbol {
-    Name: __ZTS6IsInOpIiE (4341)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C344
-  }
-  Symbol {
-    Name: __ZTS6IsInOpIxE (4357)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C34F
-  }
-  Symbol {
-    Name: __ZTSNSt3__110__function6__baseIFN10tensorflow6StatusEPNS2_15shape_inference16InferenceContextEEEE (4373)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C6B5
-  }
-  Symbol {
-    Name: __ZTSNSt3__110__function6__baseIFvxxEEE (4472)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C12C
-  }
-  Symbol {
-    Name: __ZTSNSt3__110__function6__funcIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE (4512)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C1BB
-  }
-  Symbol {
-    Name: __ZTSNSt3__110__function6__funcIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE (4636)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C285
-  }
-  Symbol {
-    Name: __ZTSNSt3__110__function6__funcIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS6_EEFvxxEEE (4761)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C0B2
-  }
-  Symbol {
-    Name: __ZTSNSt3__110__function6__funcIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE (4888)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C372
-  }
-  Symbol {
-    Name: __ZTSNSt3__110__function6__funcIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE (5020)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C453
-  }
-  Symbol {
-    Name: __ZTSNSt3__110__function6__funcIZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_NS_9allocatorIS7_EEFvxxEEE (5152)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C534
-  }
-  Symbol {
-    Name: __ZTSNSt3__115basic_stringbufIcNS_11char_traitsIcEENS_9allocatorIcEEEE (5284)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C070
-  }
-  Symbol {
-    Name: __ZTSNSt3__118basic_stringstreamIcNS_11char_traitsIcEENS_9allocatorIcEEEE (5355)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C02B
-  }
-  Symbol {
-    Name: __ZTSZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_ (5429)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C232
-  }
-  Symbol {
-    Name: __ZTSZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_ (5500)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C2FD
-  }
-  Symbol {
-    Name: __ZTSZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_ (5572)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C14F
-  }
-  Symbol {
-    Name: __ZTSZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_ (5646)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C3F1
-  }
-  Symbol {
-    Name: __ZTSZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_ (5725)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C4D2
-  }
-  Symbol {
-    Name: __ZTSZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEEUlxxE_ (5804)
-    Extern
-    Type: Section (0xE)
-    Section: __const (0x5)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1C5B3
-  }
-  Symbol {
-    Name: __ZZN5Eigen8internal20manage_caching_sizesENS_6ActionEPlS2_S2_E12m_cacheSizes (5883)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F2E8
-  }
-  Symbol {
-    Name: __ZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS4_E17vmodule_activated (5961)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F318
-  }
-  Symbol {
-    Name: __ZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (6064)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F308
-  }
-  Symbol {
-    Name: __ZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (6166)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F2B8
-  }
-  Symbol {
-    Name: __ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated (6270)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F378
-  }
-  Symbol {
-    Name: __ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated (6380)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F388
-  }
-  Symbol {
-    Name: __ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated (6490)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F368
-  }
-  Symbol {
-    Name: __ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated (6599)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F3B8
-  }
-  Symbol {
-    Name: __ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated (6709)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F3C8
-  }
-  Symbol {
-    Name: __ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated (6819)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F3A8
-  }
-  Symbol {
-    Name: __ZZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated (6928)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F3F8
-  }
-  Symbol {
-    Name: __ZZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated (7038)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F408
-  }
-  Symbol {
-    Name: __ZZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated (7148)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F3E8
-  }
-  Symbol {
-    Name: __ZZZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (7257)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F2D8
-  }
-  Symbol {
-    Name: __ZZZN7FidIter7advanceEvENKUliPKcE_clEiS1_E17vmodule_activated (7365)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F338
-  }
-  Symbol {
-    Name: __ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE0_clEiS5_E17vmodule_activated (7428)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F348
-  }
-  Symbol {
-    Name: __ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE1_clEiS5_E17vmodule_activated (7546)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F358
-  }
-  Symbol {
-    Name: __ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS5_E17vmodule_activated (7664)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F328
-  }
-  Symbol {
-    Name: __ZZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS5_E17vmodule_activated (7781)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F2C8
-  }
-  Symbol {
-    Name: __ZZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated (7900)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F398
-  }
-  Symbol {
-    Name: __ZZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated (8024)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F3D8
-  }
-  Symbol {
-    Name: __ZZZZN18SplitRaggedBlockOpIxE7ComputeEPN10tensorflow15OpKernelContextEENKUlxxE_clExxENKUliPKcE_clEiS6_E17vmodule_activated (8148)
-    Extern
-    Type: Section (0xE)
-    Section: __data (0xC)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x80)
-      WeakDef (0x80)
-    ]
-    Value: 0x1F418
-  }
-  Symbol {
-    Name: __Unwind_Resume (8272)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x300)
-      AltEntry (0x200)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow10DEVICE_CPUE (8288)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow11register_op19OpDefBuilderWrapperclEv (8318)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow12OpDefBuilder10SetShapeFnENSt3__18functionIFNS_6StatusEPNS_15shape_inference16InferenceContextEEEE (8373)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow12OpDefBuilder4AttrENSt3__112basic_stringIcNS1_11char_traitsIcEENS1_9allocatorIcEEEE (8489)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow12OpDefBuilder5InputENSt3__112basic_stringIcNS1_11char_traitsIcEENS1_9allocatorIcEEEE (8590)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow12OpDefBuilder6OutputENSt3__112basic_stringIcNS1_11char_traitsIcEENS1_9allocatorIcEEEE (8692)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow12OpDefBuilderC1ENSt3__112basic_stringIcNS1_11char_traitsIcEENS1_9allocatorIcEEEE (8795)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow14TensorShapeRep19DestructorOutOfLineEv (8893)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow14kernel_factory17OpKernelRegistrar12InitInternalEPKNS_9KernelDefEN4absl14lts_2020_09_2311string_viewENSt3__110unique_ptrINS0_15OpKernelFactoryENS8_14default_deleteISA_EEEE (8949)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow15OpKernelContext10CtxFailureEPKciRKNS_6StatusE (9138)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow15OpKernelContext15allocate_outputEiRKNS_11TensorShapeEPPNS_6TensorE (9202)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow15OpKernelContext21CtxFailureWithWarningEPKciRKNS_6StatusE (9287)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow15TensorShapeBaseINS_11TensorShapeEEC2EN4absl14lts_2020_09_234SpanIKxEE (9362)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x180)
-      SymbolResolver (0x100)
-      WeakDef (0x80)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow15shape_inference16InferenceContext10ReplaceDimENS0_11ShapeHandleExNS0_15DimensionHandleEPS2_ (9450)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow15shape_inference16InferenceContext8WithRankENS0_11ShapeHandleExPS2_ (9560)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow15shape_inference16InferenceContext9MakeShapeESt16initializer_listINS0_19DimensionOrConstantEE (9645)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow16KernelDefBuilder14TypeConstraintEPKcNS_8DataTypeE (9756)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow16KernelDefBuilder5BuildEv (9824)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow16KernelDefBuilder6DeviceEPKc (9867)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow16KernelDefBuilderC2EPKc (9913)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow16KernelDefBuilderD2Ev (9954)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow22CheckNotInComputeAsyncEPNS_15OpKernelContextEPKc (9993)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow5OpDefD1Ev (10060)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow6StatusC1ENS_5error4CodeEN4absl14lts_2020_09_2311string_viewEONSt3__16vectorINS_10StackFrameENS6_9allocatorIS8_EEEE (10087)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow6thread10ThreadPool11ParallelForExxRKNSt3__18functionIFvxxEEE (10219)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow7strings6StrCatERKNS0_8AlphaNumE (10297)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow8OpKernelC2EPNS_20OpKernelConstructionE (10346)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow8OpKernelD2Ev (10402)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow8internal10LogMessage16VmoduleActivatedEPKci (10432)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow8internal10LogMessageC1EPKcii (10493)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow8internal10LogMessageD1Ev (10539)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow8internal15LogMessageFatalC1EPKci (10581)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow8internal15LogMessageFatalD1Ev (10631)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow8internal21CheckOpMessageBuilder7ForVar2Ev (10678)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow8internal21CheckOpMessageBuilder9NewStringEv (10737)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow8internal21CheckOpMessageBuilderC1EPKc (10798)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZN10tensorflow8internal21CheckOpMessageBuilderD1Ev (10853)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNK10tensorflow11TensorShape10IsSameSizeERKS0_ (10906)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNK10tensorflow15OpKernelContext5inputEi (10955)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNK10tensorflow15TensorShapeBaseINS_11TensorShapeEE8dim_sizeEi (10998)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x180)
-      SymbolResolver (0x100)
-      WeakDef (0x80)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNK10tensorflow6Tensor21CheckTypeAndIsAlignedENS_8DataTypeE (11063)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNK10tensorflow6Tensor30CheckIsAlignedAndSingleElementEv (11125)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNK10tensorflow6Tensor9CheckTypeENS_8DataTypeE (11184)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb (11233)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNKSt3__120__vector_base_commonILb1EE20__throw_length_errorEv (11298)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNKSt3__120__vector_base_commonILb1EE20__throw_out_of_rangeEv (11362)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNKSt3__121__basic_string_commonILb1EE20__throw_length_errorEv (11426)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNKSt3__16locale9use_facetERNS0_2idE (11491)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNKSt3__18ios_base6getlocEv (11530)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt11logic_errorC2EPKc (11560)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt12length_errorD1Ev (11586)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__112__next_primeEm (11611)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEE6resizeEmc (11638)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__112basic_stringIcNS_11char_traitsIcEENS_9allocatorIcEEE9push_backEc (11713)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__113basic_istreamIcNS_11char_traitsIcEEED0Ev (11790)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__113basic_istreamIcNS_11char_traitsIcEEED1Ev (11843)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEE6sentryC1ERS3_ (11896)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEE6sentryD1Ev (11959)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEED0Ev (12019)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEED1Ev (12072)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEElsEf (12125)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEElsEi (12178)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEElsEm (12231)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__113basic_ostreamIcNS_11char_traitsIcEEElsEx (12284)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__114basic_iostreamIcNS_11char_traitsIcEEED0Ev (12337)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__114basic_iostreamIcNS_11char_traitsIcEEED1Ev (12391)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__114basic_iostreamIcNS_11char_traitsIcEEED2Ev (12445)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__115basic_streambufIcNS_11char_traitsIcEEE4syncEv (12499)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__115basic_streambufIcNS_11char_traitsIcEEE5imbueERKNS_6localeE (12557)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__115basic_streambufIcNS_11char_traitsIcEEE5uflowEv (12628)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__115basic_streambufIcNS_11char_traitsIcEEE6setbufEPcl (12687)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__115basic_streambufIcNS_11char_traitsIcEEE6xsgetnEPcl (12749)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__115basic_streambufIcNS_11char_traitsIcEEE6xsputnEPKcl (12811)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__115basic_streambufIcNS_11char_traitsIcEEE9showmanycEv (12874)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__115basic_streambufIcNS_11char_traitsIcEEEC2Ev (12937)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__115basic_streambufIcNS_11char_traitsIcEEED2Ev (12992)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__15ctypeIcE2idE (13047)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__16localeD1Ev (13071)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__18ios_base33__set_badbit_and_consider_rethrowEv (13093)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__18ios_base4initEPv (13150)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__18ios_base5clearEj (13178)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt3__19basic_iosIcNS_11char_traitsIcEEED2Ev (13206)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt9bad_allocC1Ev (13254)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZNSt9bad_allocD1Ev (13275)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZSt9terminatev (13296)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZTIN10tensorflow8OpKernelE (13313)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZTINSt3__113basic_istreamIcNS_11char_traitsIcEEEE (13342)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZTINSt3__113basic_ostreamIcNS_11char_traitsIcEEEE (13394)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZTINSt3__114basic_iostreamIcNS_11char_traitsIcEEEE (13446)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZTINSt3__115basic_streambufIcNS_11char_traitsIcEEEE (13499)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZTISt12length_error (13553)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x280)
-      AltEntry (0x200)
-      WeakDef (0x80)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZTISt9bad_alloc (13575)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZTVN10__cxxabiv117__class_type_infoE (13593)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZTVN10__cxxabiv120__si_class_type_infoE (13632)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZTVN10tensorflow14kernel_factory17OpKernelRegistrar18PtrOpKernelFactoryE (13674)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x100)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZTVSt12length_error (13749)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZThn16_NSt3__114basic_iostreamIcNS_11char_traitsIcEEED0Ev (13771)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZThn16_NSt3__114basic_iostreamIcNS_11char_traitsIcEEED1Ev (13831)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZTv0_n24_NSt3__113basic_istreamIcNS_11char_traitsIcEEED0Ev (13891)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZTv0_n24_NSt3__113basic_istreamIcNS_11char_traitsIcEEED1Ev (13952)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZTv0_n24_NSt3__113basic_ostreamIcNS_11char_traitsIcEEED0Ev (14013)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZTv0_n24_NSt3__113basic_ostreamIcNS_11char_traitsIcEEED1Ev (14074)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZTv0_n24_NSt3__114basic_iostreamIcNS_11char_traitsIcEEED0Ev (14135)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZTv0_n24_NSt3__114basic_iostreamIcNS_11char_traitsIcEEED1Ev (14197)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __ZdlPv (14259)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x280)
-      AltEntry (0x200)
-      WeakDef (0x80)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: __Znwm (14267)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x280)
-      AltEntry (0x200)
-      WeakDef (0x80)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: ___assert_rtn (14274)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x300)
-      AltEntry (0x200)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: ___bzero (14288)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x300)
-      AltEntry (0x200)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: ___cxa_allocate_exception (14297)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: ___cxa_begin_catch (14323)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: ___cxa_end_catch (14342)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: ___cxa_free_exception (14359)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: ___cxa_guard_abort (14381)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: ___cxa_guard_acquire (14400)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: ___cxa_guard_release (14421)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: ___cxa_throw (14442)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: ___gxx_personality_v0 (14455)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x200)
-      AltEntry (0x200)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: ___stack_chk_fail (14477)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x300)
-      AltEntry (0x200)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: ___stack_chk_guard (14495)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x300)
-      AltEntry (0x200)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: _free (14514)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x300)
-      AltEntry (0x200)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: _malloc (14520)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x300)
-      AltEntry (0x200)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: _memcpy (14528)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x300)
-      AltEntry (0x200)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: _memset (14536)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x300)
-      AltEntry (0x200)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: _strlen (14544)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x300)
-      AltEntry (0x200)
-      SymbolResolver (0x100)
-    ]
-    Value: 0x0
-  }
-  Symbol {
-    Name: dyld_stub_binder (14552)
-    Extern
-    Type: Undef (0x0)
-    Section:  (0x0)
-    RefType: UndefinedNonLazy (0x0)
-    Flags [ (0x300)
-      AltEntry (0x200)
-      SymbolResolver (0x100)
-    ]
+    Name: _ZTSZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ (20148)
+    Value: 0x59BA0
+    Size: 75
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15shape_inference16InferenceContext10ReplaceDimENS0_11ShapeHandleElNS0_15DimensionHandleEPS2_ (20227)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSs4_Rep20_S_empty_rep_storageE@@GLIBCXX_3.4 (20336)
     Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ (20383)
+    Value: 0x2606E8
+    Size: 16
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN13GetSlotFidsOpD0Ev (20462)
+    Value: 0x25D10
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15shape_inference19DimensionOrConstantC2El (20485)
+    Value: 0x4F840
+    Size: 36
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated (20543)
+    Value: 0x2614F0
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated (20669)
+    Value: 0x261550
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN5Eigen8internal21queryCacheSizes_intelERiS1_S1_i (20780)
+    Value: 0xEA60
+    Size: 1317
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: __bss_start (20832)
+    Value: 0x261490
+    Size: 0
+    Binding: Global (0x1)
+    Type: None (0x0)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (20844)
+    Value: 0x2614C0
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow15OpKernelContext5inputEi (20947)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE1_clEiS5_E17vmodule_activated (20989)
+    Value: 0x2615D0
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZNSt6vectorIN5Eigen8internal27TensorBlockScratchAllocatorINS0_13DefaultDeviceEE10AllocationESaIS5_EE17_M_realloc_insertIJRKS5_EEEvN9__gnu_cxx17__normal_iteratorIPS5_S7_EEDpOT_ (21109)
+    Value: 0x17AE0
+    Size: 302
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN30UnsortedFeatureVecToSegmentsOpD2Ev (21286)
+    Value: 0x32BC0
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: __stack_chk_fail@@GLIBC_2.4 (21326)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow6thread10ThreadPool11ParallelForEllRKSt8functionIFvllEE (21354)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTV13GetSlotFidsOp (21425)
+    Value: 0x260690
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN10tensorflow14kernel_factory17OpKernelRegistrarC1EPKNS_9KernelDefEN4absl14lts_2020_09_2311string_viewEPFPNS_8OpKernelEPNS_20OpKernelConstructionEE (21445)
+    Value: 0xEFD0
+    Size: 181
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERS9_RKSA_ (21595)
+    Value: 0x11CB0
+    Size: 230
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTSZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_ (21758)
+    Value: 0x59880
+    Size: 66
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: memset@@GLIBC_2.2.5 (21828)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow6errors15InvalidArgumentIJPKcEEENS_6StatusEDpT_ (21848)
+    Value: 0x10350
+    Size: 4969
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSolsEi@@GLIBCXX_3.4 (21911)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN6IsInOpIlED2Ev (21934)
+    Value: 0x4B8A0
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZNK4absl14lts_2020_09_234SpanIKlEixEmENUlvE_4_FUNEv (21952)
+    Value: 0x10340
+    Size: 11
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE_clEiS5_E17vmodule_activated (22006)
+    Value: 0x2615F0
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZZN5Eigen8internal20manage_caching_sizesENS_6ActionEPlS2_S2_E12m_cacheSizes (22125)
+    Value: 0x2614D0
+    Size: 24
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN10tensorflow11register_op19OpDefBuilderWrapper10SetShapeFnESt8functionIFNS_6StatusEPNS_15shape_inference16InferenceContextEEE (22202)
+    Value: 0x4F530
+    Size: 185
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN30UnsortedFeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextE (22331)
+    Value: 0x38BC0
+    Size: 20567
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTISt12length_error@@GLIBCXX_3.4 (22408)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow11register_op19OpDefBuilderWrapper5InputESs (22442)
+    Value: 0x4F390
+    Size: 203
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: __cxa_guard_acquire@@CXXABI_1.3 (22501)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTVN10__cxxabiv117__class_type_infoE@@CXXABI_1.3 (22533)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSt9basic_iosIcSt11char_traitsIcEE4initEPSt15basic_streambufIcS1_E@@GLIBCXX_3.4 (22583)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIlED0Ev (22665)
+    Value: 0x297C0
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSo9_M_insertIlEERSoT_@@GLIBCXX_3.4.9 (22696)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN16PoolingBySlotsOpD0Ev (22736)
+    Value: 0xDF10
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZN30UnsortedFeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (22762)
+    Value: 0x2615B8
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEED2Ev (22879)
+    Value: 0x4B960
+    Size: 119
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN20PoolingBySlotsGradOpD2Ev (23074)
+    Value: 0xDF30
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTS13GetSlotFidsOp (23104)
+    Value: 0x59860
+    Size: 16
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZN6IsInOpIlE7ComputeEPN10tensorflow15OpKernelContextE (23124)
+    Value: 0x4CC80
+    Size: 3625
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _end (23179)
+    Value: 0x261640
+    Size: 0
+    Binding: Global (0x1)
+    Type: None (0x0)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: __cxa_allocate_exception@@CXXABI_1.3 (23184)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: __pthread_key_create (23221)
+    Value: 0x0
+    Size: 0
+    Binding: Weak (0x2)
+    Type: None (0x0)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: __gmon_start__ (23242)
+    Value: 0x0
+    Size: 0
+    Binding: Weak (0x2)
+    Type: None (0x0)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: strlen@@GLIBC_2.2.5 (23257)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal10LogMessageD1Ev (23277)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow16KernelDefBuilderC2EPKc (23318)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow6Tensor4dataEv (23358)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTVSt9bad_alloc@@GLIBCXX_3.4 (23389)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTS22FeatureVecToSegmentsOp (23419)
+    Value: 0x5A160
+    Size: 25
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_ (23448)
+    Value: 0x15DB0
+    Size: 406
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTV17ParseFeatureVecOp (23601)
+    Value: 0x260970
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: __cxa_guard_abort@@CXXABI_1.3 (23625)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated (23655)
+    Value: 0x261578
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTI17ParseFeatureVecOp (23779)
+    Value: 0x260958
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZGVZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated (23803)
+    Value: 0x261570
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextE (23929)
+    Value: 0x2CEC0
+    Size: 8786
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN6IsInOpIiE7ComputeEPN10tensorflow15OpKernelContextE (23997)
+    Value: 0x4BE80
+    Size: 3577
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_EC1ERKSF_m (24052)
+    Value: 0x44680
+    Size: 4941
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN30UnsortedFeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (24227)
+    Value: 0x2615B0
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZZZN7FidIter7advanceEvENKUliPKcE_clEiS1_E17vmodule_activated (24346)
+    Value: 0x261628
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTI22FeatureVecToSegmentsOp (24408)
+    Value: 0x260828
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextE (24437)
+    Value: 0x3DD50
+    Size: 16489
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (24498)
+    Value: 0x261498
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZNSo9_M_insertImEERSoT_@@GLIBCXX_3.4.9 (24607)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_EC2ERKSF_m (24647)
+    Value: 0x44680
+    Size: 4941
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTV30UnsortedFeatureVecToSegmentsOp (24822)
+    Value: 0x2608A0
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN16PoolingBySlotsOpD2Ev (24859)
+    Value: 0xDEF0
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_ (24885)
+    Value: 0x11B10
+    Size: 406
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb (25036)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERS8_RKS9_ (25100)
+    Value: 0x11B10
+    Size: 406
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC1ERS9_RKSA_ (25251)
+    Value: 0x11CB0
+    Size: 230
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEED1Ev (25414)
+    Value: 0x118A0
+    Size: 135
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt6vectorIPN10tensorflow15shape_inference9DimensionESaIS3_EE17_M_realloc_insertIJS3_EEEvN9__gnu_cxx17__normal_iteratorIPS3_S5_EEDpOT_ (25487)
+    Value: 0x4F690
+    Size: 302
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTI16PoolingBySlotsOp (25624)
+    Value: 0x260578
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZdlPv@@GLIBCXX_3.4 (25647)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_ (25667)
+    Value: 0x11930
+    Size: 230
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15TensorShapeBaseINS_11TensorShapeEEC1EN4absl14lts_2020_09_234SpanIKlEE (25818)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTISt9bad_alloc@@GLIBCXX_3.4 (25905)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal21CheckOpMessageBuilderD1Ev (25935)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_ (25987)
+    Value: 0x260900
+    Size: 16
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN6IsInOpIlED0Ev (26059)
+    Value: 0x4B8C0
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt12length_errorD1Ev@@GLIBCXX_3.4 (26077)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: __cxa_guard_release@@CXXABI_1.3 (26114)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow16KernelDefBuilderD2Ev (26146)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSt14_Function_base13_Base_managerIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E10_M_managerERSt9_Any_dataRKS8_St18_Manager_operation (26184)
+    Value: 0x29870
+    Size: 129
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal15LogMessageFatalC1EPKci (26350)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTS14GroupBySlotsOp (26399)
+    Value: 0x5A3C0
+    Size: 17
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEED2Ev (26420)
+    Value: 0x4B8E0
+    Size: 119
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS4_E17vmodule_activated (26615)
+    Value: 0x261608
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZGVZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated (26717)
+    Value: 0x261530
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTS18SplitRaggedBlockOpIfE (26843)
+    Value: 0x59BF0
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZNSt6vectorIN10tensorflow10StackFrameESaIS1_EED2Ev (26871)
+    Value: 0xFA90
+    Size: 2161
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN17ParseFeatureVecOpD1Ev (26923)
+    Value: 0x44510
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow12OpDefBuilder5InputESs (26950)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN14GroupBySlotsOpD2Ev (26989)
+    Value: 0x3DC70
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: __gxx_personality_v0@@CXXABI_1.3 (27013)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSs4swapERSs@@GLIBCXX_3.4 (27046)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow12OpDefBuilderC1ESs (27074)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow16KernelDefBuilder5BuildEv (27109)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTSN10tensorflow4core10RefCountedE (27151)
+    Value: 0x59320
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZTVN10tensorflow4core10RefCountedE (27187)
+    Value: 0x2605B8
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN10tensorflow14TensorShapeRep19DestructorOutOfLineEv (27223)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZSt20__throw_length_errorPKc@@GLIBCXX_3.4 (27278)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERSA_RKSB_ (27321)
+    Value: 0x15DB0
+    Size: 406
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _edata (27474)
+    Value: 0x261490
+    Size: 0
+    Binding: Global (0x1)
+    Type: None (0x0)
+    Other: 0
+    Section: .data (0x18)
+  }
+  Symbol {
+    Name: _ZTI18SplitRaggedBlockOpIlE (27481)
+    Value: 0x260738
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN10tensorflow4core10RefCountedD1Ev (27509)
+    Value: 0x1DBD0
+    Size: 180
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: __cxa_throw@@CXXABI_1.3 (27546)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN16PoolingBySlotsOpD1Ev (27570)
+    Value: 0xDEF0
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN6IsInOpIiED0Ev (27596)
+    Value: 0x4B880
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIlED1Ev (27614)
+    Value: 0x297A0
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTI18SplitRaggedBlockOpIfE (27645)
+    Value: 0x260708
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZTV16PoolingBySlotsOp (27673)
+    Value: 0x2605D8
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated (27696)
+    Value: 0x261500
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZGVZN5Eigen8internal20manage_caching_sizesENS_6ActionEPlS2_S2_E12m_cacheSizes (27807)
+    Value: 0x2614C8
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS3_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKSA_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSI_EEEEKNS3_ILln1EKNS4_INS5_ISI_Li2ELi1ElEELi16ES7_EEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE0EE3runERSV_RKSW_ (27886)
+    Value: 0x11DA0
+    Size: 16397
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE0_clEiS5_E17vmodule_activated (28291)
+    Value: 0x2615E8
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_ (28409)
+    Value: 0x2605A8
+    Size: 16
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated (28483)
+    Value: 0x261538
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTIN10tensorflow8OpKernelE (28607)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _Unwind_Resume@@GCC_3.0 (28635)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated (28659)
+    Value: 0x261540
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZNSt8ios_base4InitD1Ev@@GLIBCXX_3.4 (28770)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZZZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (28807)
+    Value: 0x2614A0
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIiED0Ev (28914)
+    Value: 0x29780
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTV20PoolingBySlotsGradOp (28945)
+    Value: 0x260620
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE0_clEll (28972)
+    Value: 0x21C10
+    Size: 846
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt14_Function_base13_Base_managerIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation (29051)
+    Value: 0xDF70
+    Size: 153
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTIN10tensorflow4core10RefCountedE (29212)
+    Value: 0x260568
+    Size: 16
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN10tensorflow14kernel_factory17OpKernelRegistrar12InitInternalEPKNS_9KernelDefEN4absl14lts_2020_09_2311string_viewESt10unique_ptrINS0_15OpKernelFactoryESt14default_deleteIS9_EE (29248)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE0_clEiS5_E17vmodule_activated (29427)
+    Value: 0x2615E0
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN13GetSlotFidsOpD1Ev (29547)
+    Value: 0x25CF0
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN14GroupBySlotsOpD1Ev (29570)
+    Value: 0x3DC70
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt17_Function_handlerIFvllEZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E9_M_invokeERKSt9_Any_dataOlSB_ (29594)
+    Value: 0x2CEB0
+    Size: 14
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSs4_Rep9_S_createEmmRKSaIcE@@GLIBCXX_3.4 (29730)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZZN4absl14lts_2020_09_2311string_view19CheckLengthInternalEmENKUlvE_clEv (29774)
+    Value: 0xEF90
+    Size: 35
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt14_Function_base13_Base_managerIZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E10_M_managerERSt9_Any_dataRKS8_St18_Manager_operation (29848)
+    Value: 0x297E0
+    Size: 129
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated (30014)
+    Value: 0x261598
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZNSt8ios_baseD2Ev@@GLIBCXX_3.4 (30123)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE1_clEiS5_E17vmodule_activated (30155)
+    Value: 0x2615D8
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTSZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ (30273)
+    Value: 0x59AE0
+    Size: 75
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZZN22FeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (30352)
+    Value: 0x2615C8
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC1ERSC_RKSD_ (30461)
+    Value: 0x15F50
+    Size: 230
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow14kernel_factory17OpKernelRegistrarC2EPKNS_9KernelDefEN4absl14lts_2020_09_2311string_viewEPFPNS_8OpKernelEPNS_20OpKernelConstructionEE (30627)
+    Value: 0xEFD0
+    Size: 181
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS4_E17vmodule_activated (30777)
+    Value: 0x261600
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZZN4absl14lts_2020_09_2311string_view19CheckLengthInternalEmENUlvE_4_FUNEv (30881)
+    Value: 0xEFC0
+    Size: 11
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZSt24__throw_out_of_range_fmtPKcz (30957)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSo9_M_insertIdEERSoT_@@GLIBCXX_3.4.9 (30992)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15shape_inference19DimensionOrConstantC2ENS0_15DimensionHandleE (31032)
+    Value: 0x4F980
+    Size: 25
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow10DeviceBase29tensorflow_cpu_worker_threadsEv (31111)
+    Value: 0x1DCB0
+    Size: 131
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: __cxa_end_catch@@CXXABI_1.3 (31173)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIfED2Ev (31201)
+    Value: 0x29720
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN7FidIter7advanceEvENKUliPKcE_clEiS1_E17vmodule_activated (31232)
+    Value: 0x261620
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZNSt6localeC1Ev@@GLIBCXX_3.4 (31296)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN13GetSlotFidsOpD2Ev (31326)
+    Value: 0x25CF0
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIfED1Ev (31349)
+    Value: 0x29720
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt14_Function_base13_Base_managerIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation (31380)
+    Value: 0x25D30
+    Size: 137
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN17ParseFeatureVecOp7ComputeEPN10tensorflow15OpKernelContextE (31537)
+    Value: 0x459D0
+    Size: 24042
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSs6assignERKSs@@GLIBCXX_3.4 (31601)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSt6vectorIN10tensorflow10StackFrameESaIS1_EED1Ev (31632)
+    Value: 0xFA90
+    Size: 2161
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: __cxa_rethrow@@CXXABI_1.3 (31684)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSt14_Function_base13_Base_managerIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E10_M_managerERSt9_Any_dataRKS8_St18_Manager_operation (31710)
+    Value: 0x29900
+    Size: 129
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTI14GroupBySlotsOp (31876)
+    Value: 0x2608E8
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZZNK4absl14lts_2020_09_234SpanIKlEixEmENKUlvE_clEv (31897)
+    Value: 0x10310
+    Size: 35
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _init (31949)
+    Value: 0xB450
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: .init (0x9)
+  }
+  Symbol {
+    Name: _ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE21_M_insert_unique_nodeEmmPNS1_10_Hash_nodeIiLb0EEE (31955)
+    Value: 0x4BD70
+    Size: 272
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (32197)
+    Value: 0x2614B8
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTV18SplitRaggedBlockOpIlE (32302)
+    Value: 0x2607E0
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZTVN10__cxxabiv120__si_class_type_infoE@@CXXABI_1.3 (32330)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTV22FeatureVecToSegmentsOp (32383)
+    Value: 0x260858
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal21CheckOpMessageBuilder7ForVar2Ev (32412)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated (32470)
+    Value: 0x261528
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN10tensorflow12OpDefBuilder6OutputESs (32578)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextE (32618)
+    Value: 0x2FE40
+    Size: 8802
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt17_Function_handlerIFvllEZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E9_M_invokeERKSt9_Any_dataOlSB_ (32686)
+    Value: 0x2FE30
+    Size: 14
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERSA_RKSB_ (32822)
+    Value: 0x11A20
+    Size: 230
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN14GroupBySlotsOpD0Ev (32975)
+    Value: 0x3DC90
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTIZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ (32999)
+    Value: 0x2606D8
+    Size: 16
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8OpKernel11IsExpensiveEv (33078)
+    Value: 0xDED0
+    Size: 8
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: __cxa_atexit@@GLIBC_2.2.5 (33118)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSt10unique_ptrIN10tensorflow6Status5StateESt14default_deleteIS2_EED1Ev (33144)
+    Value: 0xF090
+    Size: 2555
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated (33218)
+    Value: 0x261510
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTS20PoolingBySlotsGradOp (33329)
+    Value: 0x59360
+    Size: 23
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZN10tensorflow11register_op19OpDefBuilderWrapper6OutputESs (33356)
+    Value: 0x4F460
+    Size: 203
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: __cxa_free_exception@@CXXABI_1.3 (33416)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSt17_Function_handlerIFvllEZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E9_M_invokeERKSt9_Any_dataOlSB_ (33449)
+    Value: 0x32AD0
+    Size: 14
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8OpKernel7AsAsyncEv (33585)
+    Value: 0xDEC0
+    Size: 3
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow11register_op19OpDefBuilderWrapperC2EPKc (33620)
+    Value: 0x4F2C0
+    Size: 199
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTVSt15basic_streambufIcSt11char_traitsIcEE@@GLIBCXX_3.4 (33676)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE21_M_insert_unique_nodeEmmPNS1_10_Hash_nodeIlLb0EEE (33734)
+    Value: 0x4BB20
+    Size: 272
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: malloc@@GLIBC_2.2.5 (33976)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZGVZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated (33996)
+    Value: 0x261590
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN10tensorflow16KernelDefBuilder6DeviceEPKc (34107)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated (34152)
+    Value: 0x261508
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextE (34261)
+    Value: 0x1E1C0
+    Size: 14924
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIiED2Ev (34324)
+    Value: 0x29760
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_ (34355)
+    Value: 0x260680
+    Size: 16
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm1EEEvN4absl14lts_2020_09_234SpanIKlEEPSt5arrayIlXT_EE (34425)
+    Value: 0x1DEC0
+    Size: 351
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE9_M_rehashEmRKm (34541)
+    Value: 0x4B9E0
+    Size: 308
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev (34747)
+    Value: 0x4B960
+    Size: 119
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNKSt8__detail20_Prime_rehash_policy11_M_next_bktEm (34942)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow11register_op19OpDefBuilderWrapperC1EPKc (34995)
+    Value: 0x4F2C0
+    Size: 199
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow7strings6StrCatERKNS0_8AlphaNumE (35051)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated (35099)
+    Value: 0x261588
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15shape_inference9DimensionC2El (35208)
+    Value: 0x4F8F0
+    Size: 28
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTS6IsInOpIlE (35255)
+    Value: 0x5C7B0
+    Size: 11
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE9_M_rehashEmRKm (35270)
+    Value: 0x4BC30
+    Size: 308
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTVSt9basic_iosIcSt11char_traitsIcEE@@GLIBCXX_3.4 (35476)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSs4_Rep10_M_destroyERKSaIcE@@GLIBCXX_3.4 (35527)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZSt16__ostream_insertIcSt11char_traitsIcEERSt13basic_ostreamIT_T0_ES6_PKS3_l@@GLIBCXX_3.4.9 (35571)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSt8ios_baseC2Ev@@GLIBCXX_3.4 (35664)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal21CheckOpMessageBuilder9NewStringEv (35696)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE_clEiS5_E17vmodule_activated (35756)
+    Value: 0x2615F8
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZNSt6localeD1Ev@@GLIBCXX_3.4 (35873)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal17MakeCheckOpStringImmEEPSsRKT_RKT0_PKc (35903)
+    Value: 0x116C0
+    Size: 151
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt8ios_base4InitC1Ev@@GLIBCXX_3.4 (35967)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow6Tensor30CheckIsAlignedAndSingleElementEv (36004)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ITM_registerTMCloneTable (36062)
+    Value: 0x0
+    Size: 0
+    Binding: Weak (0x2)
+    Type: None (0x0)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated (36088)
+    Value: 0x261558
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15shape_inference16InferenceContext8WithRankENS0_11ShapeHandleElPS2_ (36197)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow8OpKernel12const_tensorEv (36281)
+    Value: 0xDEE0
+    Size: 3
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN22FeatureVecToSegmentsOpD2Ev (36323)
+    Value: 0x32B80
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN20PoolingBySlotsGradOpD1Ev (36355)
+    Value: 0xDF30
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15OpKernelContext15allocate_outputEiRKNS_11TensorShapeEPPNS_6TensorE (36385)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8OpKernelC2EPNS_20OpKernelConstructionE (36469)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTSZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ (36524)
+    Value: 0x59B40
+    Size: 75
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_ (36603)
+    Value: 0x11A20
+    Size: 230
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTVSt18basic_stringstreamIcSt11char_traitsIcESaIcEE@@GLIBCXX_3.4 (36756)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTI20PoolingBySlotsGradOp (36822)
+    Value: 0x260590
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZGVZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (36849)
+    Value: 0x261610
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTVN10tensorflow14kernel_factory17OpKernelRegistrar18PtrOpKernelFactoryE (36952)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal17MakeCheckOpStringIiiEEPSsRKT_RKT0_PKc (37026)
+    Value: 0x4F5F0
+    Size: 150
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow4core10RefCountedD2Ev (37090)
+    Value: 0x1DBD0
+    Size: 180
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE0_clEllENKUliPKcE_clEiS5_E17vmodule_activated (37127)
+    Value: 0x2614B0
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZNSt6vectorIlSaIlEE17_M_realloc_insertIJRKlEEEvN9__gnu_cxx17__normal_iteratorIPlS1_EEDpOT_ (37246)
+    Value: 0x44550
+    Size: 302
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal21CheckOpMessageBuilderC1EPKc (37338)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN17ParseFeatureVecOpD0Ev (37392)
+    Value: 0x44530
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt17_Function_handlerIFvllEZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_E9_M_invokeERKSt9_Any_dataOlSA_ (37419)
+    Value: 0x25930
+    Size: 946
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEll (37546)
+    Value: 0x2BC00
+    Size: 4781
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTV6IsInOpIlE (37630)
+    Value: 0x260A30
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZTTSt18basic_stringstreamIcSt11char_traitsIcESaIcEE@@GLIBCXX_3.4 (37645)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal15LogMessageFatalD1Ev (37711)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8OpKernelD2Ev (37757)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTI13GetSlotFidsOp (37786)
+    Value: 0x260668
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZTV6IsInOpIiE (37806)
+    Value: 0x2609E8
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZTIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ (37821)
+    Value: 0x2606F8
+    Size: 16
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated (37900)
+    Value: 0x2615A8
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN6IsInOpIiED2Ev (38008)
+    Value: 0x4B860
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTS18SplitRaggedBlockOpIiE (38026)
+    Value: 0x59C10
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZNSt9basic_iosIcSt11char_traitsIcEE5clearESt12_Ios_Iostate@@GLIBCXX_3.4 (38054)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextE (38127)
+    Value: 0x21F70
+    Size: 14695
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen8internal13TensorBlockIOIflLi3ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi3EEE (38194)
+    Value: 0x17E70
+    Size: 8268
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow12OpDefBuilderD1Ev (38288)
+    Value: 0x4F9A0
+    Size: 10013
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZN17ParseFeatureVecOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (38322)
+    Value: 0x261638
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN22FeatureVecToSegmentsOpD1Ev (38426)
+    Value: 0x32B80
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextE (38458)
+    Value: 0x25DC0
+    Size: 14443
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow6Tensor21CheckTypeAndIsAlignedENS_8DataTypeE (38518)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm3EEEvN4absl14lts_2020_09_234SpanIKlEEPSt5arrayIlXT_EE (38579)
+    Value: 0x1E020
+    Size: 410
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTI18SplitRaggedBlockOpIiE (38695)
+    Value: 0x260720
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZGVZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated (38723)
+    Value: 0x2615A0
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTV18SplitRaggedBlockOpIfE (38833)
+    Value: 0x260750
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZTSZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_ (38861)
+    Value: 0x5A3E0
+    Size: 68
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15shape_inference9DimensionC1El (38933)
+    Value: 0x4F8F0
+    Size: 28
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERS8_RKS9_ (38980)
+    Value: 0x11930
+    Size: 230
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15shape_inference16InferenceContext9MakeShapeESt16initializer_listINS0_19DimensionOrConstantEE (39131)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN5Eigen8internal13TensorBlockIOIflLi2ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi2EEE (39241)
+    Value: 0x16040
+    Size: 6811
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN22FeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextE (39335)
+    Value: 0x32C00
+    Size: 24504
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow10DEVICE_CPUE (39404)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNKSt8__detail20_Prime_rehash_policy14_M_need_rehashEmmm (39433)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZGVZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE0_clEllENKUliPKcE_clEiS5_E17vmodule_activated (39491)
+    Value: 0x2614A8
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTS6IsInOpIiE (39612)
+    Value: 0x5C7A0
+    Size: 11
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZN30UnsortedFeatureVecToSegmentsOpD0Ev (39627)
+    Value: 0x32BE0
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIiED1Ev (39667)
+    Value: 0x29760
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated (39698)
+    Value: 0x261548
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN10tensorflow16KernelDefBuilder14TypeConstraintEPKcNS_8DataTypeE (39807)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSsC1EPKcRKSaIcE@@GLIBCXX_3.4 (39874)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTS30UnsortedFeatureVecToSegmentsOp (39906)
+    Value: 0x5A180
+    Size: 33
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15OpKernelContext21CtxFailureWithWarningEPKciRKNS_6StatusE (39943)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (40017)
+    Value: 0x261618
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZNSt14_Function_base13_Base_managerIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation (40118)
+    Value: 0x3DCB0
+    Size: 153
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt10unique_ptrIN10tensorflow6Status5StateESt14default_deleteIS2_EED2Ev (40277)
+    Value: 0xF090
+    Size: 2555
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal17MakeCheckOpStringIllEEPSsRKT_RKT0_PKc (40351)
+    Value: 0x11800
+    Size: 151
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEED2Ev (40415)
+    Value: 0x118A0
+    Size: 135
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow12OpDefBuilderD2Ev (40488)
+    Value: 0x4F9A0
+    Size: 10013
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
   }
 ]
```

### llvm-readobj --dyn-symbols {}

```diff
@@ -1,6 +1,3220 @@
 
-Format: Mach-O 64-bit x86-64
+Format: elf64-x86-64
 Arch: x86_64
 AddressSize: 64bit
+LoadName: <Not found>
 DynamicSymbols [
+  Symbol {
+    Name:  (0)
+    Value: 0x0
+    Size: 0
+    Binding: Local (0x0)
+    Type: None (0x0)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow5OpDefD1Ev (23853)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow12OpDefBuilder10SetShapeFnESt8functionIFNS_6StatusEPNS_15shape_inference16InferenceContextEEE (22922)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSt12length_errorC1EPKc (19547)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow15TensorShapeBaseINS_11TensorShapeEE8dim_sizeEi (8081)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZSt19__throw_logic_errorPKc@GLIBCXX_3.4 (3164)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15OpKernelContext10CtxFailureEPKciRKNS_6StatusE (9042)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: __cxa_begin_catch@CXXABI_1.3 (21291)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: memcpy@GLIBC_2.14 (3139)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZSt17__throw_bad_allocv@GLIBCXX_3.4 (16722)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSt9bad_allocD1Ev@GLIBCXX_3.4 (1159)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSt18basic_stringstreamIcSt11char_traitsIcESaIcEED1Ev@GLIBCXX_3.4 (3193)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ITM_deregisterTMCloneTable (28)
+    Value: 0x0
+    Size: 0
+    Binding: Weak (0x2)
+    Type: None (0x0)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow22CheckNotInComputeAsyncEPNS_15OpKernelContextEPKc (8976)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _Znwm@GLIBCXX_3.4 (499)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: memmove@GLIBC_2.2.5 (6426)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow11register_op19OpDefBuilderWrapperclEv (23913)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: __assert_fail@GLIBC_2.2.5 (831)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal10LogMessageC1EPKcii (8835)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow12OpDefBuilder4AttrESs (23967)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: free@GLIBC_2.2.5 (3798)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow6Tensor9CheckTypeENS_8DataTypeE (8316)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: __cxa_finalize@GLIBC_2.2.5 (82)
+    Value: 0x0
+    Size: 0
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTVSt15basic_stringbufIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4 (2702)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow6StatusC1ENS_5error4CodeEN4absl14lts_2020_09_2311string_viewEOSt6vectorINS_10StackFrameESaIS7_EE (2967)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow11TensorShape10IsSameSizeERKS0_ (8033)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal10LogMessage16VmoduleActivatedEPKci (9179)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15shape_inference16InferenceContext10ReplaceDimENS0_11ShapeHandleElNS0_15DimensionHandleEPS2_ (23442)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSs4_Rep20_S_empty_rep_storageE@GLIBCXX_3.4 (2020)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow15OpKernelContext5inputEi (7991)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: __stack_chk_fail@GLIBC_2.4 (1041)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow6thread10ThreadPool11ParallelForEllRKSt8functionIFvllEE (8556)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: memset@GLIBC_2.2.5 (2054)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSolsEi@GLIBCXX_3.4 (3651)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTISt12length_error@GLIBCXX_3.4 (19597)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: __cxa_guard_acquire@CXXABI_1.3 (1001)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3 (9931)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSt9basic_iosIcSt11char_traitsIcEE4initEPSt15basic_streambufIcS1_E@GLIBCXX_3.4 (2518)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSo9_M_insertIlEERSoT_@GLIBCXX_3.4.9 (3626)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: __cxa_allocate_exception@CXXABI_1.3 (1100)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: __pthread_key_create (10276)
+    Value: 0x0
+    Size: 0
+    Binding: Weak (0x2)
+    Type: None (0x0)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: __gmon_start__ (1)
+    Value: 0x0
+    Size: 0
+    Binding: Weak (0x2)
+    Type: None (0x0)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: strlen@GLIBC_2.2.5 (2752)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal10LogMessageD1Ev (8880)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow16KernelDefBuilderC2EPKc (7082)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow6Tensor4dataEv (20088)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTVSt9bad_alloc@GLIBCXX_3.4 (1125)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: __cxa_guard_abort@CXXABI_1.3 (9239)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSo9_M_insertImEERSoT_@GLIBCXX_3.4.9 (3367)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb (10212)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZdlPv@GLIBCXX_3.4 (344)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15TensorShapeBaseINS_11TensorShapeEEC1EN4absl14lts_2020_09_234SpanIKlEE (8145)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTISt9bad_alloc@GLIBCXX_3.4 (1142)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal21CheckOpMessageBuilderD1Ev (3510)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSt12length_errorD1Ev@GLIBCXX_3.4 (19573)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: __cxa_guard_release@CXXABI_1.3 (1021)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow16KernelDefBuilderD2Ev (7238)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal15LogMessageFatalC1EPKci (7349)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow12OpDefBuilder5InputESs (22654)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: __gxx_personality_v0@CXXABI_1.3 (575)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSs4swapERSs@GLIBCXX_3.4 (2868)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow12OpDefBuilderC1ESs (22504)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow16KernelDefBuilder5BuildEv (7196)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow14TensorShapeRep19DestructorOutOfLineEv (8921)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZSt20__throw_length_errorPKc@GLIBCXX_3.4 (16747)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: __cxa_throw@CXXABI_1.3 (1179)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTIN10tensorflow8OpKernelE (10056)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _Unwind_Resume@GCC_3.0 (560)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSt8ios_base4InitD1Ev@GLIBCXX_3.4 (7045)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow14kernel_factory17OpKernelRegistrar12InitInternalEPKNS_9KernelDefEN4absl14lts_2020_09_2311string_viewESt10unique_ptrINS0_15OpKernelFactoryESt14default_deleteIS9_EE (1617)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSs4_Rep9_S_createEmmRKSaIcE@GLIBCXX_3.4 (2837)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSt8ios_baseD2Ev@GLIBCXX_3.4 (2900)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZSt24__throw_out_of_range_fmtPKcz (22394)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSo9_M_insertIdEERSoT_@GLIBCXX_3.4.9 (12995)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: __cxa_end_catch@CXXABI_1.3 (21323)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSt6localeC1Ev@GLIBCXX_3.4 (2685)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSs6assignERKSs@GLIBCXX_3.4 (3146)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: __cxa_rethrow@CXXABI_1.3 (21309)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 (10015)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal21CheckOpMessageBuilder7ForVar2Ev (3392)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow12OpDefBuilder6OutputESs (22753)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: __cxa_atexit@GLIBC_2.2.5 (7069)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: __cxa_free_exception@CXXABI_1.3 (19618)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTVSt15basic_streambufIcSt11char_traitsIcEE@GLIBCXX_3.4 (2587)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: malloc@GLIBC_2.2.5 (6514)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow16KernelDefBuilder6DeviceEPKc (7151)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNKSt8__detail20_Prime_rehash_policy11_M_next_bktEm (22142)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow7strings6StrCatERKNS0_8AlphaNumE (2919)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTVSt9basic_iosIcSt11char_traitsIcEE@GLIBCXX_3.4 (2480)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSs4_Rep10_M_destroyERKSaIcE@GLIBCXX_3.4 (468)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZSt16__ostream_insertIcSt11char_traitsIcEERSt13basic_ostreamIT_T0_ES6_PKS3_l@GLIBCXX_3.4.9 (2759)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSt8ios_baseC2Ev@GLIBCXX_3.4 (2408)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal21CheckOpMessageBuilder9NewStringEv (3450)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSt6localeD1Ev@GLIBCXX_3.4 (2883)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSt8ios_base4InitC1Ev@GLIBCXX_3.4 (7021)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow6Tensor30CheckIsAlignedAndSingleElementEv (10800)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ITM_registerTMCloneTable (56)
+    Value: 0x0
+    Size: 0
+    Binding: Weak (0x2)
+    Type: None (0x0)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15shape_inference16InferenceContext8WithRankENS0_11ShapeHandleElPS2_ (22310)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15OpKernelContext15allocate_outputEiRKNS_11TensorShapeEPPNS_6TensorE (8232)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8OpKernelC2EPNS_20OpKernelConstructionE (505)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTVSt18basic_stringstreamIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4 (2632)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTVN10tensorflow14kernel_factory17OpKernelRegistrar18PtrOpKernelFactoryE (1543)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal21CheckOpMessageBuilderC1EPKc (3313)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZTTSt18basic_stringstreamIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4 (2427)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal15LogMessageFatalD1Ev (7398)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8OpKernelD2Ev (263)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSt9basic_iosIcSt11char_traitsIcEE5clearESt12_Ios_Iostate@GLIBCXX_3.4 (3079)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow6Tensor21CheckTypeAndIsAlignedENS_8DataTypeE (8364)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15shape_inference16InferenceContext9MakeShapeESt16initializer_listINS0_19DimensionOrConstantEE (23709)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow10DEVICE_CPUE (7122)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Object (0x1)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNKSt8__detail20_Prime_rehash_policy14_M_need_rehashEmmm (21581)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow16KernelDefBuilder14TypeConstraintEPKcNS_8DataTypeE (12066)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZNSsC1EPKcRKSaIcE@GLIBCXX_3.4 (22485)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15OpKernelContext21CtxFailureWithWarningEPKciRKNS_6StatusE (9105)
+    Value: 0x0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: Undefined (0x0)
+  }
+  Symbol {
+    Name: _ZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextE (7928)
+    Value: 0x1E1C0
+    Size: 14924
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated (14947)
+    Value: 0x261598
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZZZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (9752)
+    Value: 0x2614A0
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE1_clEiS5_E17vmodule_activated (18823)
+    Value: 0x2615D0
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15shape_inference19DimensionOrConstantC1El (23290)
+    Value: 0x4F840
+    Size: 36
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt14_Function_base13_Base_managerIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation (17315)
+    Value: 0x3DCB0
+    Size: 153
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEE8allocateEm (6434)
+    Value: 0x17C10
+    Size: 596
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15shape_inference19DimensionOrConstantC1ENS0_15DimensionHandleE (23630)
+    Value: 0x4F980
+    Size: 25
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERS8_RKS9_ (4635)
+    Value: 0x11B10
+    Size: 406
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated (14728)
+    Value: 0x2615A8
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZNSt14_Function_base13_Base_managerIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E10_M_managerERSt9_Any_dataRKS8_St18_Manager_operation (11576)
+    Value: 0x29870
+    Size: 129
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (8627)
+    Value: 0x2614B8
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEll (15412)
+    Value: 0x320B0
+    Size: 2588
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen8internal19throw_std_bad_allocEv (1058)
+    Value: 0xEA20
+    Size: 50
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN13GetSlotFidsOpD0Ev (10490)
+    Value: 0x25D10
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTS18SplitRaggedBlockOpIfE (15983)
+    Value: 0x59BF0
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIfED2Ev (10968)
+    Value: 0x29720
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTS18SplitRaggedBlockOpIlE (16095)
+    Value: 0x59C30
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated (13532)
+    Value: 0x261568
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (17710)
+    Value: 0x261618
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTSZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ (15904)
+    Value: 0x59BA0
+    Size: 75
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated (12311)
+    Value: 0x261528
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZZZN17ParseFeatureVecOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (19984)
+    Value: 0x261638
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextE (10740)
+    Value: 0x25DC0
+    Size: 14443
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated (15622)
+    Value: 0x261578
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS4_E17vmodule_activated (17915)
+    Value: 0x261608
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_ (4484)
+    Value: 0x11B10
+    Size: 406
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt17_Function_handlerIFvllEZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E9_M_invokeERKSt9_Any_dataOlSB_ (12859)
+    Value: 0x2CEB0
+    Size: 14
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTI20PoolingBySlotsGradOp (10111)
+    Value: 0x260590
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN5Eigen8internal13TensorBlockIOIflLi3ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi3EEE (6521)
+    Value: 0x17E70
+    Size: 8268
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN13GetSlotFidsOpD2Ev (10424)
+    Value: 0x25CF0
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _init (16)
+    Value: 0xB450
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: .init (0x9)
+  }
+  Symbol {
+    Name: _ZN20PoolingBySlotsGradOpD0Ev (438)
+    Value: 0xDF50
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN16PoolingBySlotsOpD0Ev (318)
+    Value: 0xDF10
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE0_clEllENKUliPKcE_clEiS5_E17vmodule_activated (9457)
+    Value: 0x2614B0
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTV6IsInOpIiE (20185)
+    Value: 0x2609E8
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZTI18SplitRaggedBlockOpIiE (16067)
+    Value: 0x260720
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN10tensorflow4core10RefCountedD0Ev (7481)
+    Value: 0x1DC90
+    Size: 18
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow11register_op19OpDefBuilderWrapperC2EPKc (22429)
+    Value: 0x4F2C0
+    Size: 199
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN22FeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (16502)
+    Value: 0x2615C0
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTSZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ (15746)
+    Value: 0x59AE0
+    Size: 75
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZN6IsInOpIiE7ComputeEPN10tensorflow15OpKernelContextE (22087)
+    Value: 0x4BE80
+    Size: 3577
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated (14300)
+    Value: 0x261530
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_ (757)
+    Value: 0x2605A8
+    Size: 16
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZTIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ (11742)
+    Value: 0x2606E8
+    Size: 16
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN20PoolingBySlotsGradOpD2Ev (351)
+    Value: 0xDF30
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN16PoolingBySlotsOpD2Ev (214)
+    Value: 0xDEF0
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow11register_op19OpDefBuilderWrapper5InputESs (22595)
+    Value: 0x4F390
+    Size: 203
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN30UnsortedFeatureVecToSegmentsOpD0Ev (16393)
+    Value: 0x32BE0
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEED1Ev (3803)
+    Value: 0x118A0
+    Size: 135
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow4core10RefCountedD2Ev (7276)
+    Value: 0x1DBD0
+    Size: 180
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated (14426)
+    Value: 0x261538
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTV14GroupBySlotsOp (17246)
+    Value: 0x260910
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN17ParseFeatureVecOpD0Ev (19253)
+    Value: 0x44530
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt17_Function_handlerIFvllEZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_E9_M_invokeERKSt9_Any_dataOlSA_ (10297)
+    Value: 0x25930
+    Size: 946
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN30UnsortedFeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (16854)
+    Value: 0x2615B0
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTVN10tensorflow4core10RefCountedE (7313)
+    Value: 0x2605B8
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZZZN30UnsortedFeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (16973)
+    Value: 0x2615B8
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZZN4absl14lts_2020_09_2311string_view19CheckLengthInternalEmENUlvE_4_FUNEv (1317)
+    Value: 0xEFC0
+    Size: 11
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt6vectorIN10tensorflow10StackFrameESaIS1_EED2Ev (2135)
+    Value: 0xFA90
+    Size: 2161
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow11register_op19OpDefBuilderWrapperC1EPKc (22539)
+    Value: 0x4F2C0
+    Size: 199
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTV17ParseFeatureVecOp (19202)
+    Value: 0x260970
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZTV30UnsortedFeatureVecToSegmentsOp (16316)
+    Value: 0x2608A0
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN30UnsortedFeatureVecToSegmentsOpD2Ev (16276)
+    Value: 0x32BC0
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEED2Ev (20695)
+    Value: 0x4B960
+    Size: 119
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN17ParseFeatureVecOpD2Ev (19175)
+    Value: 0x44510
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated (13104)
+    Value: 0x2614F0
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZZZN22FeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (16613)
+    Value: 0x2615C8
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN30UnsortedFeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextE (16777)
+    Value: 0x38BC0
+    Size: 20567
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZN5Eigen8internal20manage_caching_sizesENS_6ActionEPlS2_S2_E12m_cacheSizes (924)
+    Value: 0x2614D0
+    Size: 24
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZGVZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE0_clEllENKUliPKcE_clEiS5_E17vmodule_activated (9336)
+    Value: 0x2614A8
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN6IsInOpIlED0Ev (20287)
+    Value: 0x4B8C0
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE0_clEiS5_E17vmodule_activated (18585)
+    Value: 0x2615E0
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm1EEEvN4absl14lts_2020_09_234SpanIKlEEPSt5arrayIlXT_EE (7696)
+    Value: 0x1DEC0
+    Size: 351
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE1_clEiS5_E17vmodule_activated (18943)
+    Value: 0x2615D8
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_ (4178)
+    Value: 0x11A20
+    Size: 230
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN14GroupBySlotsOpD0Ev (17291)
+    Value: 0x3DC90
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextE (9576)
+    Value: 0x21F70
+    Size: 14695
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN6IsInOpIlED2Ev (20236)
+    Value: 0x4B8A0
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated (12639)
+    Value: 0x261500
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZGVZZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (9643)
+    Value: 0x261498
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZZZN7FidIter7advanceEvENKUliPKcE_clEiS1_E17vmodule_activated (18523)
+    Value: 0x261628
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN6IsInOpIiED1Ev (20200)
+    Value: 0x4B860
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTS6IsInOpIiE (22250)
+    Value: 0x5C7A0
+    Size: 11
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZTV16PoolingBySlotsOp (240)
+    Value: 0x2605D8
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN22FeatureVecToSegmentsOpD1Ev (16212)
+    Value: 0x32B80
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN14GroupBySlotsOpD2Ev (17222)
+    Value: 0x3DC70
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTI6IsInOpIlE (22295)
+    Value: 0x2609D0
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZGVZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated (14618)
+    Value: 0x2615A0
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZNSt10unique_ptrIN10tensorflow6Status5StateESt14default_deleteIS2_EED1Ev (2061)
+    Value: 0xF090
+    Size: 2555
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15shape_inference9DimensionC2El (23348)
+    Value: 0x4F8F0
+    Size: 28
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTSZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ (15825)
+    Value: 0x59B40
+    Size: 75
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEED2Ev (20305)
+    Value: 0x4B8E0
+    Size: 119
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTSZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_ (10898)
+    Value: 0x59880
+    Size: 66
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextE (12133)
+    Value: 0x29990
+    Size: 8805
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated (13422)
+    Value: 0x261560
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN10tensorflow11register_op19OpDefBuilderWrapper10SetShapeFnESt8functionIFNS_6StatusEPNS_15shape_inference16InferenceContextEEE (22793)
+    Value: 0x4F530
+    Size: 185
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt17_Function_handlerIFvllEZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E9_M_invokeERKSt9_Any_dataOlSB_ (15276)
+    Value: 0x32AD0
+    Size: 14
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN6IsInOpIlE7ComputeEPN10tensorflow15OpKernelContextE (22195)
+    Value: 0x4CC80
+    Size: 3625
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZNK4absl14lts_2020_09_234SpanIKlEixEmENKUlvE_clEv (2239)
+    Value: 0x10310
+    Size: 35
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTV18SplitRaggedBlockOpIiE (11120)
+    Value: 0x260798
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZNSt6vectorIPN10tensorflow15shape_inference9DimensionESaIS3_EE17_M_realloc_insertIJS3_EEEvN9__gnu_cxx17__normal_iteratorIPS3_S5_EEDpOT_ (23095)
+    Value: 0x4F690
+    Size: 302
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTSN10tensorflow4core10RefCountedE (9859)
+    Value: 0x59320
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated (12201)
+    Value: 0x261520
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIlED1Ev (11269)
+    Value: 0x297A0
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8OpKernel7AsAsyncEv (97)
+    Value: 0xDEC0
+    Size: 3
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated (12750)
+    Value: 0x261508
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIiED0Ev (11179)
+    Value: 0x29780
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal17MakeCheckOpStringImmEEPSsRKT_RKT0_PKc (3249)
+    Value: 0x116C0
+    Size: 151
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt17_Function_handlerIFvllEZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_E9_M_invokeERKSt9_Any_dataOlSA_ (18017)
+    Value: 0x444B0
+    Size: 14
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow12OpDefBuilderD2Ev (23819)
+    Value: 0x4F9A0
+    Size: 10013
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen8internal21queryCacheSizes_intelERiS1_S1_i (1191)
+    Value: 0xEA60
+    Size: 1317
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERSA_RKSB_ (5517)
+    Value: 0x15DB0
+    Size: 406
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt17_Function_handlerIFvllEZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E9_M_invokeERKSt9_Any_dataOlSB_ (14080)
+    Value: 0x2FE30
+    Size: 14
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS4_E17vmodule_activated (17811)
+    Value: 0x261600
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZGVZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated (15496)
+    Value: 0x261570
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN10tensorflow14kernel_factory17OpKernelRegistrarC2EPKNS_9KernelDefEN4absl14lts_2020_09_2311string_viewEPFPNS_8OpKernelEPNS_20OpKernelConstructionEE (1393)
+    Value: 0xEFD0
+    Size: 181
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTI14GroupBySlotsOp (19082)
+    Value: 0x2608E8
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIiED2Ev (11089)
+    Value: 0x29760
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE0_clEll (9257)
+    Value: 0x21C10
+    Size: 846
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated (13640)
+    Value: 0x261550
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_EC2ERKSF_m (19372)
+    Value: 0x44680
+    Size: 4941
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _edata (24073)
+    Value: 0x261490
+    Size: 0
+    Binding: Global (0x1)
+    Type: None (0x0)
+    Other: 0
+    Section: .data (0x18)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIfED1Ev (11027)
+    Value: 0x29720
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTV20PoolingBySlotsGradOp (381)
+    Value: 0x260620
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow8OpKernel12const_tensorEv (172)
+    Value: 0xDEE0
+    Size: 3
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTI16PoolingBySlotsOp (9992)
+    Value: 0x260578
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZNSt14_Function_base13_Base_managerIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation (596)
+    Value: 0xDF70
+    Size: 153
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow10DeviceBase29tensorflow_cpu_worker_threadsEv (7518)
+    Value: 0x1DCB0
+    Size: 131
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8OpKernel11IsExpensiveEv (132)
+    Value: 0xDED0
+    Size: 8
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15shape_inference19DimensionOrConstantC2El (23232)
+    Value: 0x4F840
+    Size: 36
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE0_clEiS5_E17vmodule_activated (18705)
+    Value: 0x2615E8
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTI13GetSlotFidsOp (10878)
+    Value: 0x260668
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZTS18SplitRaggedBlockOpIiE (16039)
+    Value: 0x59C10
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZN10tensorflow14kernel_factory17OpKernelRegistrarC1EPKNS_9KernelDefEN4absl14lts_2020_09_2311string_viewEPFPNS_8OpKernelEPNS_20OpKernelConstructionEE (1796)
+    Value: 0xEFD0
+    Size: 181
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN13GetSlotFidsOpD1Ev (10467)
+    Value: 0x25CF0
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE9_M_rehashEmRKm (21085)
+    Value: 0x4B9E0
+    Size: 308
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated (12419)
+    Value: 0x261510
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE21_M_insert_unique_nodeEmmPNS1_10_Hash_nodeIlLb0EEE (21339)
+    Value: 0x4BB20
+    Size: 272
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTSZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_ (10138)
+    Value: 0x59380
+    Size: 70
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEll (13020)
+    Value: 0x2BC00
+    Size: 4781
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTI18SplitRaggedBlockOpIfE (16011)
+    Value: 0x260708
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZTV6IsInOpIlE (20254)
+    Value: 0x260A30
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZTI30UnsortedFeatureVecToSegmentsOp (17185)
+    Value: 0x260840
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZTI18SplitRaggedBlockOpIlE (16123)
+    Value: 0x260738
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZTIN10tensorflow4core10RefCountedE (9895)
+    Value: 0x260568
+    Size: 16
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZGVZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated (15056)
+    Value: 0x261580
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextE (17546)
+    Value: 0x3DD50
+    Size: 16489
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated (13751)
+    Value: 0x261558
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTS20PoolingBySlotsGradOp (10084)
+    Value: 0x59360
+    Size: 23
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC1ERS9_RKSA_ (4949)
+    Value: 0x11CB0
+    Size: 230
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN16PoolingBySlotsOpD1Ev (292)
+    Value: 0xDEF0
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN20PoolingBySlotsGradOpD1Ev (408)
+    Value: 0xDF30
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal17MakeCheckOpStringIllEEPSsRKT_RKT0_PKc (3661)
+    Value: 0x11800
+    Size: 151
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow4core10RefCountedD1Ev (7444)
+    Value: 0x1DBD0
+    Size: 180
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (17607)
+    Value: 0x261610
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZNSt17_Function_handlerIFvllEZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_E9_M_invokeERKSt9_Any_dataOlSA_ (8425)
+    Value: 0x21F60
+    Size: 14
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE9_M_rehashEmRKm (21639)
+    Value: 0x4BC30
+    Size: 308
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (8732)
+    Value: 0x2614C0
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextE (13354)
+    Value: 0x2CEC0
+    Size: 8786
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN22FeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextE (16433)
+    Value: 0x32C00
+    Size: 24504
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN7FidIter7advanceEvENKUliPKcE_clEiS1_E17vmodule_activated (18459)
+    Value: 0x261620
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERSA_RKSB_ (4331)
+    Value: 0x11A20
+    Size: 230
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTSZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_ (19103)
+    Value: 0x5A3E0
+    Size: 68
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZNSt6vectorIN10tensorflow10StackFrameESaIS1_EED1Ev (2187)
+    Value: 0xFA90
+    Size: 2161
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated (12530)
+    Value: 0x261518
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN30UnsortedFeatureVecToSegmentsOpD1Ev (16353)
+    Value: 0x32BC0
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS3_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKSA_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSI_EEEEKNS3_ILln1EKNS4_INS5_ISI_Li2ELi1ElEELi16ES7_EEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE0EE3runERSV_RKSW_ (5112)
+    Value: 0x11DA0
+    Size: 16397
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated (13860)
+    Value: 0x261540
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal17MakeCheckOpStringIliEEPSsRKT_RKT0_PKc (3562)
+    Value: 0x11760
+    Size: 150
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZN4absl14lts_2020_09_2311string_view19CheckLengthInternalEmENKUlvE_clEv (1243)
+    Value: 0xEF90
+    Size: 35
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEED2Ev (3725)
+    Value: 0x118A0
+    Size: 135
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERS9_RKSA_ (4786)
+    Value: 0x11CB0
+    Size: 230
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev (20890)
+    Value: 0x4B960
+    Size: 119
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN17ParseFeatureVecOpD1Ev (19226)
+    Value: 0x44510
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTS17ParseFeatureVecOp (20119)
+    Value: 0x5C6A0
+    Size: 20
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE_clEiS5_E17vmodule_activated (18223)
+    Value: 0x2615F0
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKS9_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSH_EEEEKNS3_ILln1EKNS3_ILln1EKNS4_INS5_ISH_Li3ELi1ElEELi16ES7_EEEEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE1EE3runERSW_RKSX_ (6615)
+    Value: 0x19EC0
+    Size: 15630
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE_clEiS5_E17vmodule_activated (18342)
+    Value: 0x2615F8
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated (15167)
+    Value: 0x261588
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZNSt6vectorIlSaIlEE17_M_realloc_insertIJRKlEEEvN9__gnu_cxx17__normal_iteratorIPlS1_EEDpOT_ (19280)
+    Value: 0x44550
+    Size: 302
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN17ParseFeatureVecOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated (19878)
+    Value: 0x261630
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN10tensorflow11register_op19OpDefBuilderWrapper6OutputESs (22693)
+    Value: 0x4F460
+    Size: 203
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZNK4absl14lts_2020_09_234SpanIKlEixEmENUlvE_4_FUNEv (2291)
+    Value: 0x10340
+    Size: 11
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC1ERSC_RKSD_ (5989)
+    Value: 0x15F50
+    Size: 230
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN17ParseFeatureVecOp7ComputeEPN10tensorflow15OpKernelContextE (19814)
+    Value: 0x459D0
+    Size: 24042
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow8internal17MakeCheckOpStringIiiEEPSsRKT_RKT0_PKc (23031)
+    Value: 0x4F5F0
+    Size: 150
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt14_Function_base13_Base_managerIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E10_M_managerERSt9_Any_dataRKS8_St18_Manager_operation (11821)
+    Value: 0x29900
+    Size: 129
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_ (17474)
+    Value: 0x260900
+    Size: 16
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN6IsInOpIlED1Ev (20269)
+    Value: 0x4B8A0
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTI22FeatureVecToSegmentsOp (17119)
+    Value: 0x260828
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZTS30UnsortedFeatureVecToSegmentsOp (17148)
+    Value: 0x5A180
+    Size: 33
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZN6IsInOpIiED0Ev (20218)
+    Value: 0x4B880
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated (13971)
+    Value: 0x261548
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN22FeatureVecToSegmentsOpD0Ev (16244)
+    Value: 0x32BA0
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEll (14216)
+    Value: 0x2F120
+    Size: 3331
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTV13GetSlotFidsOp (10447)
+    Value: 0x260690
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: __bss_start (24080)
+    Value: 0x261490
+    Size: 0
+    Binding: Global (0x1)
+    Type: None (0x0)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated (13230)
+    Value: 0x2614F8
+    Size: 1
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERSC_RKSD_ (5823)
+    Value: 0x15F50
+    Size: 230
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERSA_RKSB_ (5670)
+    Value: 0x15DB0
+    Size: 406
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN14GroupBySlotsOpD1Ev (17267)
+    Value: 0x3DC70
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt14_Function_base13_Base_managerIZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E10_M_managerERSt9_Any_dataRKS8_St18_Manager_operation (11331)
+    Value: 0x297E0
+    Size: 129
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTV22FeatureVecToSegmentsOp (16183)
+    Value: 0x260858
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZTS6IsInOpIlE (22280)
+    Value: 0x5C7B0
+    Size: 11
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15shape_inference9DimensionC1El (23395)
+    Value: 0x4F8F0
+    Size: 28
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev (20500)
+    Value: 0x4B8E0
+    Size: 119
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _end (24092)
+    Value: 0x261640
+    Size: 0
+    Binding: Global (0x1)
+    Type: None (0x0)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZTIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ (11987)
+    Value: 0x2606F8
+    Size: 16
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm2EEEvN4absl14lts_2020_09_234SpanIKlEEPSt5arrayIlXT_EE (7580)
+    Value: 0x1DD40
+    Size: 373
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTI6IsInOpIiE (22265)
+    Value: 0x2609B8
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE21_M_insert_unique_nodeEmmPNS1_10_Hash_nodeIiLb0EEE (21845)
+    Value: 0x4BD70
+    Size: 272
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERS8_RKS9_ (4027)
+    Value: 0x11930
+    Size: 230
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen8internal13TensorBlockIOIflLi2ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi2EEE (6155)
+    Value: 0x16040
+    Size: 6811
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEll (18146)
+    Value: 0x41DC0
+    Size: 9957
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTS13GetSlotFidsOp (10858)
+    Value: 0x59860
+    Size: 16
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZTS22FeatureVecToSegmentsOp (17090)
+    Value: 0x5A160
+    Size: 25
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZN6IsInOpIiED2Ev (20167)
+    Value: 0x4B860
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN22FeatureVecToSegmentsOpD2Ev (16151)
+    Value: 0x32B80
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated (14836)
+    Value: 0x261590
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIlED0Ev (11300)
+    Value: 0x297C0
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt10unique_ptrIN10tensorflow6Status5StateESt14default_deleteIS2_EED2Ev (1946)
+    Value: 0xF090
+    Size: 2555
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTS14GroupBySlotsOp (19061)
+    Value: 0x5A3C0
+    Size: 17
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZTIZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ (11497)
+    Value: 0x2606D8
+    Size: 16
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZTV18SplitRaggedBlockOpIfE (10999)
+    Value: 0x260750
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZTV18SplitRaggedBlockOpIlE (11241)
+    Value: 0x2607E0
+    Size: 72
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN10tensorflow12OpDefBuilderD1Ev (23879)
+    Value: 0x4F9A0
+    Size: 10013
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNSt6vectorIN5Eigen8internal27TensorBlockScratchAllocatorINS0_13DefaultDeviceEE10AllocationESaIS5_EE17_M_realloc_insertIJRKS5_EEEvN9__gnu_cxx17__normal_iteratorIPS5_S7_EEDpOT_ (6249)
+    Value: 0x17AE0
+    Size: 302
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextE (14550)
+    Value: 0x2FE40
+    Size: 8802
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_ (3876)
+    Value: 0x11930
+    Size: 230
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZGVZN5Eigen8internal20manage_caching_sizesENS_6ActionEPlS2_S2_E12m_cacheSizes (845)
+    Value: 0x2614C8
+    Size: 8
+    Binding: Unique (0xA)
+    Type: Object (0x1)
+    Other: 0
+    Section: .bss (0x19)
+  }
+  Symbol {
+    Name: _ZNSt14_Function_base13_Base_managerIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation (10513)
+    Value: 0x25D30
+    Size: 137
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_ (10670)
+    Value: 0x260680
+    Size: 16
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIlED2Ev (11210)
+    Value: 0x297A0
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow6errors15InvalidArgumentIJPKcEEENS_6StatusEDpT_ (2345)
+    Value: 0x10350
+    Size: 4969
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZTS16PoolingBySlotsOp (9969)
+    Value: 0x59340
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .rodata (0xE)
+  }
+  Symbol {
+    Name: _ZTI17ParseFeatureVecOp (20143)
+    Value: 0x260958
+    Size: 24
+    Binding: Weak (0x2)
+    Type: Object (0x1)
+    Other: 0
+    Section: .data.rel.ro (0x14)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIiED1Ev (11148)
+    Value: 0x29760
+    Size: 19
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN10tensorflow15shape_inference19DimensionOrConstantC2ENS0_15DimensionHandleE (23551)
+    Value: 0x4F980
+    Size: 25
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _fini (22)
+    Value: 0x520C0
+    Size: 0
+    Binding: Global (0x1)
+    Type: Function (0x2)
+    Other: 0
+    Section: .fini (0xD)
+  }
+  Symbol {
+    Name: _ZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_EC1ERKSF_m (19639)
+    Value: 0x44680
+    Size: 4941
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZN18SplitRaggedBlockOpIfED0Ev (11058)
+    Value: 0x29740
+    Size: 32
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
+  Symbol {
+    Name: _ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm3EEEvN4absl14lts_2020_09_234SpanIKlEEPSt5arrayIlXT_EE (7812)
+    Value: 0x1E020
+    Size: 410
+    Binding: Weak (0x2)
+    Type: Function (0x2)
+    Other: 0
+    Section: .text (0xC)
+  }
 ]
```

### llvm-readobj --relocations {}

```diff
@@ -1,6 +1,428 @@
 
-Format: Mach-O 64-bit x86-64
+Format: elf64-x86-64
 Arch: x86_64
 AddressSize: 64bit
+LoadName: <Not found>
 Relocations [
+  Section (7) .rela.dyn {
+    0x260518 R_X86_64_RELATIVE - 0xDDB0
+    0x260520 R_X86_64_RELATIVE - 0xBE40
+    0x260528 R_X86_64_RELATIVE - 0xBF60
+    0x260530 R_X86_64_RELATIVE - 0xC080
+    0x260538 R_X86_64_RELATIVE - 0xC220
+    0x260540 R_X86_64_RELATIVE - 0xC340
+    0x260548 R_X86_64_RELATIVE - 0xC460
+    0x260550 R_X86_64_RELATIVE - 0xC580
+    0x260558 R_X86_64_RELATIVE - 0xDCD0
+    0x260560 R_X86_64_RELATIVE - 0xDD70
+    0x260A80 R_X86_64_RELATIVE - 0x5CB40
+    0x260A90 R_X86_64_RELATIVE - 0x5CB80
+    0x260AA0 R_X86_64_RELATIVE - 0x5CBC0
+    0x260AB0 R_X86_64_RELATIVE - 0x5CC00
+    0x260AC0 R_X86_64_RELATIVE - 0x5CC40
+    0x260AD0 R_X86_64_RELATIVE - 0x5CC80
+    0x260AE0 R_X86_64_RELATIVE - 0x5CCC0
+    0x261480 R_X86_64_RELATIVE - 0x261480
+    0x260568 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3 0x10
+    0x2605A8 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3 0x10
+    0x260680 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3 0x10
+    0x2606D8 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3 0x10
+    0x2606E8 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3 0x10
+    0x2606F8 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3 0x10
+    0x260900 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3 0x10
+    0x260A78 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3 0x10
+    0x260A88 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3 0x10
+    0x260A98 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3 0x10
+    0x260AA8 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3 0x10
+    0x260AB8 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3 0x10
+    0x260AC8 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3 0x10
+    0x260AD8 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE@CXXABI_1.3 0x10
+    0x260570 R_X86_64_64 _ZTSN10tensorflow4core10RefCountedE 0x0
+    0x260578 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 0x10
+    0x260590 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 0x10
+    0x260668 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 0x10
+    0x260708 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 0x10
+    0x260720 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 0x10
+    0x260738 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 0x10
+    0x260828 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 0x10
+    0x260840 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 0x10
+    0x2608E8 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 0x10
+    0x260958 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 0x10
+    0x2609B8 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 0x10
+    0x2609D0 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE@CXXABI_1.3 0x10
+    0x260580 R_X86_64_64 _ZTS16PoolingBySlotsOp 0x0
+    0x260588 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+    0x2605A0 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+    0x260678 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+    0x260718 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+    0x260730 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+    0x260748 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+    0x260838 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+    0x260850 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+    0x2608F8 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+    0x260968 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+    0x2609C8 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+    0x2609E0 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+    0x260598 R_X86_64_64 _ZTS20PoolingBySlotsGradOp 0x0
+    0x2605B0 R_X86_64_64 _ZTSZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_ 0x0
+    0x2605C0 R_X86_64_64 _ZTIN10tensorflow4core10RefCountedE 0x0
+    0x2605C8 R_X86_64_64 _ZN10tensorflow4core10RefCountedD1Ev 0x0
+    0x2605D0 R_X86_64_64 _ZN10tensorflow4core10RefCountedD0Ev 0x0
+    0x2605E0 R_X86_64_64 _ZTI16PoolingBySlotsOp 0x0
+    0x2605E8 R_X86_64_64 _ZN16PoolingBySlotsOpD1Ev 0x0
+    0x2605F0 R_X86_64_64 _ZN16PoolingBySlotsOpD0Ev 0x0
+    0x2605F8 R_X86_64_64 _ZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextE 0x0
+    0x260600 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+    0x260648 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+    0x2606B8 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+    0x260778 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+    0x2607C0 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+    0x260808 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+    0x260880 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+    0x2608C8 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+    0x260938 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+    0x260998 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+    0x260A10 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+    0x260A58 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+    0x260608 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+    0x260650 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+    0x2606C0 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+    0x260780 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+    0x2607C8 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+    0x260810 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+    0x260888 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+    0x2608D0 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+    0x260940 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+    0x2609A0 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+    0x260A18 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+    0x260A60 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+    0x260610 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+    0x260658 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+    0x2606C8 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+    0x260788 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+    0x2607D0 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+    0x260818 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+    0x260890 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+    0x2608D8 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+    0x260948 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+    0x2609A8 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+    0x260A20 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+    0x260A68 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+    0x260618 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+    0x260660 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+    0x2606D0 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+    0x260790 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+    0x2607D8 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+    0x260820 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+    0x260898 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+    0x2608E0 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+    0x260950 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+    0x2609B0 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+    0x260A28 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+    0x260A70 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+    0x260628 R_X86_64_64 _ZTI20PoolingBySlotsGradOp 0x0
+    0x260630 R_X86_64_64 _ZN20PoolingBySlotsGradOpD1Ev 0x0
+    0x260638 R_X86_64_64 _ZN20PoolingBySlotsGradOpD0Ev 0x0
+    0x260640 R_X86_64_64 _ZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextE 0x0
+    0x260670 R_X86_64_64 _ZTS13GetSlotFidsOp 0x0
+    0x260688 R_X86_64_64 _ZTSZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_ 0x0
+    0x260698 R_X86_64_64 _ZTI13GetSlotFidsOp 0x0
+    0x2606A0 R_X86_64_64 _ZN13GetSlotFidsOpD1Ev 0x0
+    0x2606A8 R_X86_64_64 _ZN13GetSlotFidsOpD0Ev 0x0
+    0x2606B0 R_X86_64_64 _ZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextE 0x0
+    0x2606E0 R_X86_64_64 _ZTSZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ 0x0
+    0x2606F0 R_X86_64_64 _ZTSZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ 0x0
+    0x260700 R_X86_64_64 _ZTSZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ 0x0
+    0x260710 R_X86_64_64 _ZTS18SplitRaggedBlockOpIfE 0x0
+    0x260728 R_X86_64_64 _ZTS18SplitRaggedBlockOpIiE 0x0
+    0x260740 R_X86_64_64 _ZTS18SplitRaggedBlockOpIlE 0x0
+    0x260758 R_X86_64_64 _ZTI18SplitRaggedBlockOpIfE 0x0
+    0x260760 R_X86_64_64 _ZN18SplitRaggedBlockOpIfED1Ev 0x0
+    0x260768 R_X86_64_64 _ZN18SplitRaggedBlockOpIfED0Ev 0x0
+    0x260770 R_X86_64_64 _ZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextE 0x0
+    0x2607A0 R_X86_64_64 _ZTI18SplitRaggedBlockOpIiE 0x0
+    0x2607A8 R_X86_64_64 _ZN18SplitRaggedBlockOpIiED1Ev 0x0
+    0x2607B0 R_X86_64_64 _ZN18SplitRaggedBlockOpIiED0Ev 0x0
+    0x2607B8 R_X86_64_64 _ZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextE 0x0
+    0x2607E8 R_X86_64_64 _ZTI18SplitRaggedBlockOpIlE 0x0
+    0x2607F0 R_X86_64_64 _ZN18SplitRaggedBlockOpIlED1Ev 0x0
+    0x2607F8 R_X86_64_64 _ZN18SplitRaggedBlockOpIlED0Ev 0x0
+    0x260800 R_X86_64_64 _ZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextE 0x0
+    0x260830 R_X86_64_64 _ZTS22FeatureVecToSegmentsOp 0x0
+    0x260848 R_X86_64_64 _ZTS30UnsortedFeatureVecToSegmentsOp 0x0
+    0x260860 R_X86_64_64 _ZTI22FeatureVecToSegmentsOp 0x0
+    0x260868 R_X86_64_64 _ZN22FeatureVecToSegmentsOpD1Ev 0x0
+    0x260870 R_X86_64_64 _ZN22FeatureVecToSegmentsOpD0Ev 0x0
+    0x260878 R_X86_64_64 _ZN22FeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextE 0x0
+    0x2608A8 R_X86_64_64 _ZTI30UnsortedFeatureVecToSegmentsOp 0x0
+    0x2608B0 R_X86_64_64 _ZN30UnsortedFeatureVecToSegmentsOpD1Ev 0x0
+    0x2608B8 R_X86_64_64 _ZN30UnsortedFeatureVecToSegmentsOpD0Ev 0x0
+    0x2608C0 R_X86_64_64 _ZN30UnsortedFeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextE 0x0
+    0x2608F0 R_X86_64_64 _ZTS14GroupBySlotsOp 0x0
+    0x260908 R_X86_64_64 _ZTSZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_ 0x0
+    0x260918 R_X86_64_64 _ZTI14GroupBySlotsOp 0x0
+    0x260920 R_X86_64_64 _ZN14GroupBySlotsOpD1Ev 0x0
+    0x260928 R_X86_64_64 _ZN14GroupBySlotsOpD0Ev 0x0
+    0x260930 R_X86_64_64 _ZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextE 0x0
+    0x260960 R_X86_64_64 _ZTS17ParseFeatureVecOp 0x0
+    0x260978 R_X86_64_64 _ZTI17ParseFeatureVecOp 0x0
+    0x260980 R_X86_64_64 _ZN17ParseFeatureVecOpD1Ev 0x0
+    0x260988 R_X86_64_64 _ZN17ParseFeatureVecOpD0Ev 0x0
+    0x260990 R_X86_64_64 _ZN17ParseFeatureVecOp7ComputeEPN10tensorflow15OpKernelContextE 0x0
+    0x2609C0 R_X86_64_64 _ZTS6IsInOpIiE 0x0
+    0x2609D8 R_X86_64_64 _ZTS6IsInOpIlE 0x0
+    0x2609F0 R_X86_64_64 _ZTI6IsInOpIiE 0x0
+    0x2609F8 R_X86_64_64 _ZN6IsInOpIiED1Ev 0x0
+    0x260A00 R_X86_64_64 _ZN6IsInOpIiED0Ev 0x0
+    0x260A08 R_X86_64_64 _ZN6IsInOpIiE7ComputeEPN10tensorflow15OpKernelContextE 0x0
+    0x260A38 R_X86_64_64 _ZTI6IsInOpIlE 0x0
+    0x260A40 R_X86_64_64 _ZN6IsInOpIlED1Ev 0x0
+    0x260A48 R_X86_64_64 _ZN6IsInOpIlED0Ev 0x0
+    0x260A50 R_X86_64_64 _ZN6IsInOpIlE7ComputeEPN10tensorflow15OpKernelContextE 0x0
+    0x260CD8 R_X86_64_GLOB_DAT _ZNSt17_Function_handlerIFvllEZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_E9_M_invokeERKSt9_Any_dataOlSA_ 0x0
+    0x260CE0 R_X86_64_GLOB_DAT _ZNSt17_Function_handlerIFvllEZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_E9_M_invokeERKSt9_Any_dataOlSA_ 0x0
+    0x260CE8 R_X86_64_GLOB_DAT _ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated 0x0
+    0x260CF0 R_X86_64_GLOB_DAT _ZGVZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated 0x0
+    0x260CF8 R_X86_64_GLOB_DAT _ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated 0x0
+    0x260D00 R_X86_64_GLOB_DAT _ZNSt9bad_allocD1Ev@GLIBCXX_3.4 0x0
+    0x260D08 R_X86_64_GLOB_DAT _ZGVZZN17ParseFeatureVecOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+    0x260D10 R_X86_64_GLOB_DAT _ZTV18SplitRaggedBlockOpIiE 0x0
+    0x260D18 R_X86_64_GLOB_DAT _ZZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated 0x0
+    0x260D20 R_X86_64_GLOB_DAT _ITM_deregisterTMCloneTable 0x0
+    0x260D28 R_X86_64_GLOB_DAT _ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated 0x0
+    0x260D30 R_X86_64_GLOB_DAT _ZGVZZN22FeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+    0x260D38 R_X86_64_GLOB_DAT _ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated 0x0
+    0x260D40 R_X86_64_GLOB_DAT _ZTV14GroupBySlotsOp 0x0
+    0x260D48 R_X86_64_GLOB_DAT __cxa_finalize@GLIBC_2.2.5 0x0
+    0x260D50 R_X86_64_GLOB_DAT _ZTVSt15basic_stringbufIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4 0x0
+    0x260D58 R_X86_64_GLOB_DAT _ZNSs4_Rep20_S_empty_rep_storageE@GLIBCXX_3.4 0x0
+    0x260D60 R_X86_64_GLOB_DAT _ZTIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ 0x0
+    0x260D68 R_X86_64_GLOB_DAT _ZGVZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated 0x0
+    0x260D70 R_X86_64_GLOB_DAT _ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated 0x0
+    0x260D78 R_X86_64_GLOB_DAT _ZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+    0x260D80 R_X86_64_GLOB_DAT _ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE1_clEiS5_E17vmodule_activated 0x0
+    0x260D88 R_X86_64_GLOB_DAT _ZTV13GetSlotFidsOp 0x0
+    0x260D90 R_X86_64_GLOB_DAT _ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE_clEiS5_E17vmodule_activated 0x0
+    0x260D98 R_X86_64_GLOB_DAT _ZZN5Eigen8internal20manage_caching_sizesENS_6ActionEPlS2_S2_E12m_cacheSizes 0x0
+    0x260DA0 R_X86_64_GLOB_DAT _ZTISt12length_error@GLIBCXX_3.4 0x0
+    0x260DA8 R_X86_64_GLOB_DAT _ZZZN30UnsortedFeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+    0x260DB0 R_X86_64_GLOB_DAT __pthread_key_create 0x0
+    0x260DB8 R_X86_64_GLOB_DAT __gmon_start__ 0x0
+    0x260DC0 R_X86_64_GLOB_DAT _ZTVSt9bad_alloc@GLIBCXX_3.4 0x0
+    0x260DC8 R_X86_64_GLOB_DAT _ZTV17ParseFeatureVecOp 0x0
+    0x260DD0 R_X86_64_GLOB_DAT _ZZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated 0x0
+    0x260DD8 R_X86_64_GLOB_DAT _ZGVZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated 0x0
+    0x260DE0 R_X86_64_GLOB_DAT _ZGVZZN30UnsortedFeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+    0x260DE8 R_X86_64_GLOB_DAT _ZZZN7FidIter7advanceEvENKUliPKcE_clEiS1_E17vmodule_activated 0x0
+    0x260DF0 R_X86_64_GLOB_DAT _ZGVZZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+    0x260DF8 R_X86_64_GLOB_DAT _ZTV30UnsortedFeatureVecToSegmentsOp 0x0
+    0x260E00 R_X86_64_GLOB_DAT _ZTISt9bad_alloc@GLIBCXX_3.4 0x0
+    0x260E08 R_X86_64_GLOB_DAT _ZTIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_ 0x0
+    0x260E10 R_X86_64_GLOB_DAT _ZNSt12length_errorD1Ev@GLIBCXX_3.4 0x0
+    0x260E18 R_X86_64_GLOB_DAT _ZNSt14_Function_base13_Base_managerIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E10_M_managerERSt9_Any_dataRKS8_St18_Manager_operation 0x0
+    0x260E20 R_X86_64_GLOB_DAT _ZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS4_E17vmodule_activated 0x0
+    0x260E28 R_X86_64_GLOB_DAT _ZGVZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated 0x0
+    0x260E30 R_X86_64_GLOB_DAT _ZTVN10tensorflow4core10RefCountedE 0x0
+    0x260E38 R_X86_64_GLOB_DAT _ZTV16PoolingBySlotsOp 0x0
+    0x260E40 R_X86_64_GLOB_DAT _ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated 0x0
+    0x260E48 R_X86_64_GLOB_DAT _ZGVZN5Eigen8internal20manage_caching_sizesENS_6ActionEPlS2_S2_E12m_cacheSizes 0x0
+    0x260E50 R_X86_64_GLOB_DAT _ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE0_clEiS5_E17vmodule_activated 0x0
+    0x260E58 R_X86_64_GLOB_DAT _ZTIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_ 0x0
+    0x260E60 R_X86_64_GLOB_DAT _ZZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated 0x0
+    0x260E68 R_X86_64_GLOB_DAT _ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated 0x0
+    0x260E70 R_X86_64_GLOB_DAT _ZNSt8ios_base4InitD1Ev@GLIBCXX_3.4 0x0
+    0x260E78 R_X86_64_GLOB_DAT _ZZZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+    0x260E80 R_X86_64_GLOB_DAT _ZTV20PoolingBySlotsGradOp 0x0
+    0x260E88 R_X86_64_GLOB_DAT _ZNSt14_Function_base13_Base_managerIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation 0x0
+    0x260E90 R_X86_64_GLOB_DAT _ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE0_clEiS5_E17vmodule_activated 0x0
+    0x260E98 R_X86_64_GLOB_DAT _ZNSt17_Function_handlerIFvllEZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E9_M_invokeERKSt9_Any_dataOlSB_ 0x0
+    0x260EA0 R_X86_64_GLOB_DAT _ZNSt14_Function_base13_Base_managerIZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E10_M_managerERSt9_Any_dataRKS8_St18_Manager_operation 0x0
+    0x260EA8 R_X86_64_GLOB_DAT _ZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated 0x0
+    0x260EB0 R_X86_64_GLOB_DAT _ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE1_clEiS5_E17vmodule_activated 0x0
+    0x260EB8 R_X86_64_GLOB_DAT _ZZZN22FeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+    0x260EC0 R_X86_64_GLOB_DAT _ZGVZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS4_E17vmodule_activated 0x0
+    0x260EC8 R_X86_64_GLOB_DAT _ZNK10tensorflow10DeviceBase29tensorflow_cpu_worker_threadsEv 0x0
+    0x260ED0 R_X86_64_GLOB_DAT _ZGVZZN7FidIter7advanceEvENKUliPKcE_clEiS1_E17vmodule_activated 0x0
+    0x260ED8 R_X86_64_GLOB_DAT _ZNSt14_Function_base13_Base_managerIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation 0x0
+    0x260EE0 R_X86_64_GLOB_DAT _ZNSt14_Function_base13_Base_managerIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E10_M_managerERSt9_Any_dataRKS8_St18_Manager_operation 0x0
+    0x260EE8 R_X86_64_GLOB_DAT _ZGVZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+    0x260EF0 R_X86_64_GLOB_DAT _ZTV18SplitRaggedBlockOpIlE 0x0
+    0x260EF8 R_X86_64_GLOB_DAT _ZTV22FeatureVecToSegmentsOp 0x0
+    0x260F00 R_X86_64_GLOB_DAT _ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated 0x0
+    0x260F08 R_X86_64_GLOB_DAT _ZNSt17_Function_handlerIFvllEZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E9_M_invokeERKSt9_Any_dataOlSB_ 0x0
+    0x260F10 R_X86_64_GLOB_DAT _ZTIZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ 0x0
+    0x260F18 R_X86_64_GLOB_DAT _ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated 0x0
+    0x260F20 R_X86_64_GLOB_DAT _ZNSt17_Function_handlerIFvllEZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E9_M_invokeERKSt9_Any_dataOlSB_ 0x0
+    0x260F28 R_X86_64_GLOB_DAT _ZTVSt15basic_streambufIcSt11char_traitsIcEE@GLIBCXX_3.4 0x0
+    0x260F30 R_X86_64_GLOB_DAT _ZGVZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated 0x0
+    0x260F38 R_X86_64_GLOB_DAT _ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated 0x0
+    0x260F40 R_X86_64_GLOB_DAT _ZTIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_ 0x0
+    0x260F48 R_X86_64_GLOB_DAT _ZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated 0x0
+    0x260F50 R_X86_64_GLOB_DAT _ZTVSt9basic_iosIcSt11char_traitsIcEE@GLIBCXX_3.4 0x0
+    0x260F58 R_X86_64_GLOB_DAT _ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE_clEiS5_E17vmodule_activated 0x0
+    0x260F60 R_X86_64_GLOB_DAT _ITM_registerTMCloneTable 0x0
+    0x260F68 R_X86_64_GLOB_DAT _ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated 0x0
+    0x260F70 R_X86_64_GLOB_DAT _ZTVSt18basic_stringstreamIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4 0x0
+    0x260F78 R_X86_64_GLOB_DAT _ZGVZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+    0x260F80 R_X86_64_GLOB_DAT _ZTVN10tensorflow14kernel_factory17OpKernelRegistrar18PtrOpKernelFactoryE 0x0
+    0x260F88 R_X86_64_GLOB_DAT _ZZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE0_clEllENKUliPKcE_clEiS5_E17vmodule_activated 0x0
+    0x260F90 R_X86_64_GLOB_DAT _ZNSt17_Function_handlerIFvllEZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_E9_M_invokeERKSt9_Any_dataOlSA_ 0x0
+    0x260F98 R_X86_64_GLOB_DAT _ZTV6IsInOpIlE 0x0
+    0x260FA0 R_X86_64_GLOB_DAT _ZTTSt18basic_stringstreamIcSt11char_traitsIcESaIcEE@GLIBCXX_3.4 0x0
+    0x260FA8 R_X86_64_GLOB_DAT _ZTV6IsInOpIiE 0x0
+    0x260FB0 R_X86_64_GLOB_DAT _ZTIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ 0x0
+    0x260FB8 R_X86_64_GLOB_DAT _ZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated 0x0
+    0x260FC0 R_X86_64_GLOB_DAT _ZZZN17ParseFeatureVecOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+    0x260FC8 R_X86_64_GLOB_DAT _ZGVZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated 0x0
+    0x260FD0 R_X86_64_GLOB_DAT _ZTV18SplitRaggedBlockOpIfE 0x0
+    0x260FD8 R_X86_64_GLOB_DAT _ZN10tensorflow10DEVICE_CPUE 0x0
+    0x260FE0 R_X86_64_GLOB_DAT _ZGVZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE0_clEllENKUliPKcE_clEiS5_E17vmodule_activated 0x0
+    0x260FE8 R_X86_64_GLOB_DAT _ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated 0x0
+    0x260FF0 R_X86_64_GLOB_DAT _ZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+    0x260FF8 R_X86_64_GLOB_DAT _ZNSt14_Function_base13_Base_managerIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation 0x0
+    0x261488 R_X86_64_64 __gxx_personality_v0@CXXABI_1.3 0x0
+  }
+  Section (8) .rela.plt {
+    0x261018 R_X86_64_JUMP_SLOT _ZN10tensorflow5OpDefD1Ev 0x0
+    0x261020 R_X86_64_JUMP_SLOT _ZN10tensorflow12OpDefBuilder10SetShapeFnESt8functionIFNS_6StatusEPNS_15shape_inference16InferenceContextEEE 0x0
+    0x261028 R_X86_64_JUMP_SLOT _ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEE8allocateEm 0x0
+    0x261030 R_X86_64_JUMP_SLOT _ZN10tensorflow15shape_inference19DimensionOrConstantC1El 0x0
+    0x261038 R_X86_64_JUMP_SLOT _ZNSt12length_errorC1EPKc 0x0
+    0x261040 R_X86_64_JUMP_SLOT _ZNK10tensorflow15TensorShapeBaseINS_11TensorShapeEE8dim_sizeEi 0x0
+    0x261048 R_X86_64_JUMP_SLOT _ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm2EEEvN4absl14lts_2020_09_234SpanIKlEEPSt5arrayIlXT_EE 0x0
+    0x261050 R_X86_64_JUMP_SLOT _ZSt19__throw_logic_errorPKc@GLIBCXX_3.4 0x0
+    0x261058 R_X86_64_JUMP_SLOT _ZN10tensorflow15OpKernelContext10CtxFailureEPKciRKNS_6StatusE 0x0
+    0x261060 R_X86_64_JUMP_SLOT __cxa_begin_catch@CXXABI_1.3 0x0
+    0x261068 R_X86_64_JUMP_SLOT _ZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEll 0x0
+    0x261070 R_X86_64_JUMP_SLOT memcpy@GLIBC_2.14 0x0
+    0x261078 R_X86_64_JUMP_SLOT _ZSt17__throw_bad_allocv@GLIBCXX_3.4 0x0
+    0x261080 R_X86_64_JUMP_SLOT _ZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEll 0x0
+    0x261088 R_X86_64_JUMP_SLOT _ZNSt18basic_stringstreamIcSt11char_traitsIcESaIcEED1Ev@GLIBCXX_3.4 0x0
+    0x261090 R_X86_64_JUMP_SLOT _ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKS9_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSH_EEEEKNS3_ILln1EKNS3_ILln1EKNS4_INS5_ISH_Li3ELi1ElEELi16ES7_EEEEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE1EE3runERSW_RKSX_ 0x0
+    0x261098 R_X86_64_JUMP_SLOT _ZN5Eigen8internal19throw_std_bad_allocEv 0x0
+    0x2610A0 R_X86_64_JUMP_SLOT _ZN10tensorflow22CheckNotInComputeAsyncEPNS_15OpKernelContextEPKc 0x0
+    0x2610A8 R_X86_64_JUMP_SLOT _ZN10tensorflow15shape_inference19DimensionOrConstantC1ENS0_15DimensionHandleE 0x0
+    0x2610B0 R_X86_64_JUMP_SLOT _Znwm@GLIBCXX_3.4 0x0
+    0x2610B8 R_X86_64_JUMP_SLOT memmove@GLIBC_2.2.5 0x0
+    0x2610C0 R_X86_64_JUMP_SLOT _ZN10tensorflow11register_op19OpDefBuilderWrapperclEv 0x0
+    0x2610C8 R_X86_64_JUMP_SLOT __assert_fail@GLIBC_2.2.5 0x0
+    0x2610D0 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal10LogMessageC1EPKcii 0x0
+    0x2610D8 R_X86_64_JUMP_SLOT _ZN10tensorflow12OpDefBuilder4AttrESs 0x0
+    0x2610E0 R_X86_64_JUMP_SLOT free@GLIBC_2.2.5 0x0
+    0x2610E8 R_X86_64_JUMP_SLOT _ZNK10tensorflow6Tensor9CheckTypeENS_8DataTypeE 0x0
+    0x2610F0 R_X86_64_JUMP_SLOT _ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev 0x0
+    0x2610F8 R_X86_64_JUMP_SLOT _ZN10tensorflow6StatusC1ENS_5error4CodeEN4absl14lts_2020_09_2311string_viewEOSt6vectorINS_10StackFrameESaIS7_EE 0x0
+    0x261100 R_X86_64_JUMP_SLOT _ZNK10tensorflow11TensorShape10IsSameSizeERKS0_ 0x0
+    0x261108 R_X86_64_JUMP_SLOT _ZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEll 0x0
+    0x261110 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal17MakeCheckOpStringIliEEPSsRKT_RKT0_PKc 0x0
+    0x261118 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal10LogMessage16VmoduleActivatedEPKci 0x0
+    0x261120 R_X86_64_JUMP_SLOT _ZN10tensorflow15shape_inference16InferenceContext10ReplaceDimENS0_11ShapeHandleElNS0_15DimensionHandleEPS2_ 0x0
+    0x261128 R_X86_64_JUMP_SLOT _ZN5Eigen8internal21queryCacheSizes_intelERiS1_S1_i 0x0
+    0x261130 R_X86_64_JUMP_SLOT _ZNK10tensorflow15OpKernelContext5inputEi 0x0
+    0x261138 R_X86_64_JUMP_SLOT _ZNSt6vectorIN5Eigen8internal27TensorBlockScratchAllocatorINS0_13DefaultDeviceEE10AllocationESaIS5_EE17_M_realloc_insertIJRKS5_EEEvN9__gnu_cxx17__normal_iteratorIPS5_S7_EEDpOT_ 0x0
+    0x261140 R_X86_64_JUMP_SLOT __stack_chk_fail@GLIBC_2.4 0x0
+    0x261148 R_X86_64_JUMP_SLOT _ZN10tensorflow6thread10ThreadPool11ParallelForEllRKSt8functionIFvllEE 0x0
+    0x261150 R_X86_64_JUMP_SLOT _ZN10tensorflow14kernel_factory17OpKernelRegistrarC1EPKNS_9KernelDefEN4absl14lts_2020_09_2311string_viewEPFPNS_8OpKernelEPNS_20OpKernelConstructionEE 0x0
+    0x261158 R_X86_64_JUMP_SLOT _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERS9_RKSA_ 0x0
+    0x261160 R_X86_64_JUMP_SLOT memset@GLIBC_2.2.5 0x0
+    0x261168 R_X86_64_JUMP_SLOT _ZN10tensorflow6errors15InvalidArgumentIJPKcEEENS_6StatusEDpT_ 0x0
+    0x261170 R_X86_64_JUMP_SLOT _ZNSolsEi@GLIBCXX_3.4 0x0
+    0x261178 R_X86_64_JUMP_SLOT _ZN10tensorflow11register_op19OpDefBuilderWrapper10SetShapeFnESt8functionIFNS_6StatusEPNS_15shape_inference16InferenceContextEEE 0x0
+    0x261180 R_X86_64_JUMP_SLOT _ZN10tensorflow11register_op19OpDefBuilderWrapper5InputESs 0x0
+    0x261188 R_X86_64_JUMP_SLOT __cxa_guard_acquire@CXXABI_1.3 0x0
+    0x261190 R_X86_64_JUMP_SLOT _ZNSt9basic_iosIcSt11char_traitsIcEE4initEPSt15basic_streambufIcS1_E@GLIBCXX_3.4 0x0
+    0x261198 R_X86_64_JUMP_SLOT _ZNSo9_M_insertIlEERSoT_@GLIBCXX_3.4.9 0x0
+    0x2611A0 R_X86_64_JUMP_SLOT __cxa_allocate_exception@CXXABI_1.3 0x0
+    0x2611A8 R_X86_64_JUMP_SLOT strlen@GLIBC_2.2.5 0x0
+    0x2611B0 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal10LogMessageD1Ev 0x0
+    0x2611B8 R_X86_64_JUMP_SLOT _ZN10tensorflow16KernelDefBuilderC2EPKc 0x0
+    0x2611C0 R_X86_64_JUMP_SLOT _ZNK10tensorflow6Tensor4dataEv 0x0
+    0x2611C8 R_X86_64_JUMP_SLOT __cxa_guard_abort@CXXABI_1.3 0x0
+    0x2611D0 R_X86_64_JUMP_SLOT _ZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_EC1ERKSF_m 0x0
+    0x2611D8 R_X86_64_JUMP_SLOT _ZNSo9_M_insertImEERSoT_@GLIBCXX_3.4.9 0x0
+    0x2611E0 R_X86_64_JUMP_SLOT _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_ 0x0
+    0x2611E8 R_X86_64_JUMP_SLOT _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC1ERS9_RKSA_ 0x0
+    0x2611F0 R_X86_64_JUMP_SLOT _ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEED1Ev 0x0
+    0x2611F8 R_X86_64_JUMP_SLOT _ZNSt6vectorIPN10tensorflow15shape_inference9DimensionESaIS3_EE17_M_realloc_insertIJS3_EEEvN9__gnu_cxx17__normal_iteratorIPS3_S5_EEDpOT_ 0x0
+    0x261200 R_X86_64_JUMP_SLOT _ZdlPv@GLIBCXX_3.4 0x0
+    0x261208 R_X86_64_JUMP_SLOT _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_ 0x0
+    0x261210 R_X86_64_JUMP_SLOT _ZN10tensorflow15TensorShapeBaseINS_11TensorShapeEEC1EN4absl14lts_2020_09_234SpanIKlEE 0x0
+    0x261218 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal21CheckOpMessageBuilderD1Ev 0x0
+    0x261220 R_X86_64_JUMP_SLOT __cxa_guard_release@CXXABI_1.3 0x0
+    0x261228 R_X86_64_JUMP_SLOT _ZN10tensorflow16KernelDefBuilderD2Ev 0x0
+    0x261230 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal15LogMessageFatalC1EPKci 0x0
+    0x261238 R_X86_64_JUMP_SLOT _ZN10tensorflow12OpDefBuilder5InputESs 0x0
+    0x261240 R_X86_64_JUMP_SLOT _ZNSs4swapERSs@GLIBCXX_3.4 0x0
+    0x261248 R_X86_64_JUMP_SLOT _ZN10tensorflow12OpDefBuilderC1ESs 0x0
+    0x261250 R_X86_64_JUMP_SLOT _ZN10tensorflow16KernelDefBuilder5BuildEv 0x0
+    0x261258 R_X86_64_JUMP_SLOT _ZN10tensorflow14TensorShapeRep19DestructorOutOfLineEv 0x0
+    0x261260 R_X86_64_JUMP_SLOT _ZSt20__throw_length_errorPKc@GLIBCXX_3.4 0x0
+    0x261268 R_X86_64_JUMP_SLOT _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERSA_RKSB_ 0x0
+    0x261270 R_X86_64_JUMP_SLOT _ZN10tensorflow4core10RefCountedD1Ev 0x0
+    0x261278 R_X86_64_JUMP_SLOT __cxa_throw@CXXABI_1.3 0x0
+    0x261280 R_X86_64_JUMP_SLOT _ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS3_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKSA_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSI_EEEEKNS3_ILln1EKNS4_INS5_ISI_Li2ELi1ElEELi16ES7_EEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE0EE3runERSV_RKSW_ 0x0
+    0x261288 R_X86_64_JUMP_SLOT _Unwind_Resume@GCC_3.0 0x0
+    0x261290 R_X86_64_JUMP_SLOT _ZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE0_clEll 0x0
+    0x261298 R_X86_64_JUMP_SLOT _ZN10tensorflow14kernel_factory17OpKernelRegistrar12InitInternalEPKNS_9KernelDefEN4absl14lts_2020_09_2311string_viewESt10unique_ptrINS0_15OpKernelFactoryESt14default_deleteIS9_EE 0x0
+    0x2612A0 R_X86_64_JUMP_SLOT _ZNSs4_Rep9_S_createEmmRKSaIcE@GLIBCXX_3.4 0x0
+    0x2612A8 R_X86_64_JUMP_SLOT _ZZN4absl14lts_2020_09_2311string_view19CheckLengthInternalEmENKUlvE_clEv 0x0
+    0x2612B0 R_X86_64_JUMP_SLOT _ZNSt8ios_baseD2Ev@GLIBCXX_3.4 0x0
+    0x2612B8 R_X86_64_JUMP_SLOT _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC1ERSC_RKSD_ 0x0
+    0x2612C0 R_X86_64_JUMP_SLOT _ZSt24__throw_out_of_range_fmtPKcz 0x0
+    0x2612C8 R_X86_64_JUMP_SLOT _ZNSo9_M_insertIdEERSoT_@GLIBCXX_3.4.9 0x0
+    0x2612D0 R_X86_64_JUMP_SLOT __cxa_end_catch@CXXABI_1.3 0x0
+    0x2612D8 R_X86_64_JUMP_SLOT _ZNSt6localeC1Ev@GLIBCXX_3.4 0x0
+    0x2612E0 R_X86_64_JUMP_SLOT _ZNSs6assignERKSs@GLIBCXX_3.4 0x0
+    0x2612E8 R_X86_64_JUMP_SLOT _ZNSt6vectorIN10tensorflow10StackFrameESaIS1_EED1Ev 0x0
+    0x2612F0 R_X86_64_JUMP_SLOT __cxa_rethrow@CXXABI_1.3 0x0
+    0x2612F8 R_X86_64_JUMP_SLOT _ZZNK4absl14lts_2020_09_234SpanIKlEixEmENKUlvE_clEv 0x0
+    0x261300 R_X86_64_JUMP_SLOT _ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE21_M_insert_unique_nodeEmmPNS1_10_Hash_nodeIiLb0EEE 0x0
+    0x261308 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal21CheckOpMessageBuilder7ForVar2Ev 0x0
+    0x261310 R_X86_64_JUMP_SLOT _ZN10tensorflow12OpDefBuilder6OutputESs 0x0
+    0x261318 R_X86_64_JUMP_SLOT _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERSA_RKSB_ 0x0
+    0x261320 R_X86_64_JUMP_SLOT __cxa_atexit@GLIBC_2.2.5 0x0
+    0x261328 R_X86_64_JUMP_SLOT _ZNSt10unique_ptrIN10tensorflow6Status5StateESt14default_deleteIS2_EED1Ev 0x0
+    0x261330 R_X86_64_JUMP_SLOT _ZN10tensorflow11register_op19OpDefBuilderWrapper6OutputESs 0x0
+    0x261338 R_X86_64_JUMP_SLOT __cxa_free_exception@CXXABI_1.3 0x0
+    0x261340 R_X86_64_JUMP_SLOT _ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE21_M_insert_unique_nodeEmmPNS1_10_Hash_nodeIlLb0EEE 0x0
+    0x261348 R_X86_64_JUMP_SLOT malloc@GLIBC_2.2.5 0x0
+    0x261350 R_X86_64_JUMP_SLOT _ZN10tensorflow16KernelDefBuilder6DeviceEPKc 0x0
+    0x261358 R_X86_64_JUMP_SLOT _ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm1EEEvN4absl14lts_2020_09_234SpanIKlEEPSt5arrayIlXT_EE 0x0
+    0x261360 R_X86_64_JUMP_SLOT _ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE9_M_rehashEmRKm 0x0
+    0x261368 R_X86_64_JUMP_SLOT _ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev 0x0
+    0x261370 R_X86_64_JUMP_SLOT _ZNKSt8__detail20_Prime_rehash_policy11_M_next_bktEm 0x0
+    0x261378 R_X86_64_JUMP_SLOT _ZN10tensorflow11register_op19OpDefBuilderWrapperC1EPKc 0x0
+    0x261380 R_X86_64_JUMP_SLOT _ZN10tensorflow7strings6StrCatERKNS0_8AlphaNumE 0x0
+    0x261388 R_X86_64_JUMP_SLOT _ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE9_M_rehashEmRKm 0x0
+    0x261390 R_X86_64_JUMP_SLOT _ZNSs4_Rep10_M_destroyERKSaIcE@GLIBCXX_3.4 0x0
+    0x261398 R_X86_64_JUMP_SLOT _ZSt16__ostream_insertIcSt11char_traitsIcEERSt13basic_ostreamIT_T0_ES6_PKS3_l@GLIBCXX_3.4.9 0x0
+    0x2613A0 R_X86_64_JUMP_SLOT _ZNSt8ios_baseC2Ev@GLIBCXX_3.4 0x0
+    0x2613A8 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal21CheckOpMessageBuilder9NewStringEv 0x0
+    0x2613B0 R_X86_64_JUMP_SLOT _ZNSt6localeD1Ev@GLIBCXX_3.4 0x0
+    0x2613B8 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal17MakeCheckOpStringImmEEPSsRKT_RKT0_PKc 0x0
+    0x2613C0 R_X86_64_JUMP_SLOT _ZNSt8ios_base4InitC1Ev@GLIBCXX_3.4 0x0
+    0x2613C8 R_X86_64_JUMP_SLOT _ZNK10tensorflow6Tensor30CheckIsAlignedAndSingleElementEv 0x0
+    0x2613D0 R_X86_64_JUMP_SLOT _ZN10tensorflow15shape_inference16InferenceContext8WithRankENS0_11ShapeHandleElPS2_ 0x0
+    0x2613D8 R_X86_64_JUMP_SLOT _ZN10tensorflow15OpKernelContext15allocate_outputEiRKNS_11TensorShapeEPPNS_6TensorE 0x0
+    0x2613E0 R_X86_64_JUMP_SLOT _ZN10tensorflow8OpKernelC2EPNS_20OpKernelConstructionE 0x0
+    0x2613E8 R_X86_64_JUMP_SLOT _ZNSt6vectorIlSaIlEE17_M_realloc_insertIJRKlEEEvN9__gnu_cxx17__normal_iteratorIPlS1_EEDpOT_ 0x0
+    0x2613F0 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal21CheckOpMessageBuilderC1EPKc 0x0
+    0x2613F8 R_X86_64_JUMP_SLOT _ZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEll 0x0
+    0x261400 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal15LogMessageFatalD1Ev 0x0
+    0x261408 R_X86_64_JUMP_SLOT _ZN10tensorflow8OpKernelD2Ev 0x0
+    0x261410 R_X86_64_JUMP_SLOT _ZNSt9basic_iosIcSt11char_traitsIcEE5clearESt12_Ios_Iostate@GLIBCXX_3.4 0x0
+    0x261418 R_X86_64_JUMP_SLOT _ZN5Eigen8internal13TensorBlockIOIflLi3ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi3EEE 0x0
+    0x261420 R_X86_64_JUMP_SLOT _ZN10tensorflow12OpDefBuilderD1Ev 0x0
+    0x261428 R_X86_64_JUMP_SLOT _ZNK10tensorflow6Tensor21CheckTypeAndIsAlignedENS_8DataTypeE 0x0
+    0x261430 R_X86_64_JUMP_SLOT _ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm3EEEvN4absl14lts_2020_09_234SpanIKlEEPSt5arrayIlXT_EE 0x0
+    0x261438 R_X86_64_JUMP_SLOT _ZN10tensorflow15shape_inference9DimensionC1El 0x0
+    0x261440 R_X86_64_JUMP_SLOT _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERS8_RKS9_ 0x0
+    0x261448 R_X86_64_JUMP_SLOT _ZN10tensorflow15shape_inference16InferenceContext9MakeShapeESt16initializer_listINS0_19DimensionOrConstantEE 0x0
+    0x261450 R_X86_64_JUMP_SLOT _ZN5Eigen8internal13TensorBlockIOIflLi2ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi2EEE 0x0
+    0x261458 R_X86_64_JUMP_SLOT _ZNKSt8__detail20_Prime_rehash_policy14_M_need_rehashEmmm 0x0
+    0x261460 R_X86_64_JUMP_SLOT _ZN10tensorflow16KernelDefBuilder14TypeConstraintEPKcNS_8DataTypeE 0x0
+    0x261468 R_X86_64_JUMP_SLOT _ZNSsC1EPKcRKSaIcE@GLIBCXX_3.4 0x0
+    0x261470 R_X86_64_JUMP_SLOT _ZN10tensorflow15OpKernelContext21CtxFailureWithWarningEPKciRKNS_6StatusE 0x0
+    0x261478 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal17MakeCheckOpStringIllEEPSsRKT_RKT0_PKc 0x0
+  }
 ]
```

### llvm-readobj --dyn-relocations {}

```diff
@@ -1,4 +1,424 @@
 
-Format: Mach-O 64-bit x86-64
+Format: elf64-x86-64
 Arch: x86_64
 AddressSize: 64bit
+LoadName: <Not found>
+Dynamic Relocations {
+  0x260518 R_X86_64_RELATIVE - 0xDDB0
+  0x260520 R_X86_64_RELATIVE - 0xBE40
+  0x260528 R_X86_64_RELATIVE - 0xBF60
+  0x260530 R_X86_64_RELATIVE - 0xC080
+  0x260538 R_X86_64_RELATIVE - 0xC220
+  0x260540 R_X86_64_RELATIVE - 0xC340
+  0x260548 R_X86_64_RELATIVE - 0xC460
+  0x260550 R_X86_64_RELATIVE - 0xC580
+  0x260558 R_X86_64_RELATIVE - 0xDCD0
+  0x260560 R_X86_64_RELATIVE - 0xDD70
+  0x260A80 R_X86_64_RELATIVE - 0x5CB40
+  0x260A90 R_X86_64_RELATIVE - 0x5CB80
+  0x260AA0 R_X86_64_RELATIVE - 0x5CBC0
+  0x260AB0 R_X86_64_RELATIVE - 0x5CC00
+  0x260AC0 R_X86_64_RELATIVE - 0x5CC40
+  0x260AD0 R_X86_64_RELATIVE - 0x5CC80
+  0x260AE0 R_X86_64_RELATIVE - 0x5CCC0
+  0x261480 R_X86_64_RELATIVE - 0x261480
+  0x260568 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE 0x10
+  0x2605A8 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE 0x10
+  0x260680 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE 0x10
+  0x2606D8 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE 0x10
+  0x2606E8 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE 0x10
+  0x2606F8 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE 0x10
+  0x260900 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE 0x10
+  0x260A78 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE 0x10
+  0x260A88 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE 0x10
+  0x260A98 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE 0x10
+  0x260AA8 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE 0x10
+  0x260AB8 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE 0x10
+  0x260AC8 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE 0x10
+  0x260AD8 R_X86_64_64 _ZTVN10__cxxabiv117__class_type_infoE 0x10
+  0x260570 R_X86_64_64 _ZTSN10tensorflow4core10RefCountedE 0x0
+  0x260578 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE 0x10
+  0x260590 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE 0x10
+  0x260668 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE 0x10
+  0x260708 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE 0x10
+  0x260720 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE 0x10
+  0x260738 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE 0x10
+  0x260828 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE 0x10
+  0x260840 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE 0x10
+  0x2608E8 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE 0x10
+  0x260958 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE 0x10
+  0x2609B8 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE 0x10
+  0x2609D0 R_X86_64_64 _ZTVN10__cxxabiv120__si_class_type_infoE 0x10
+  0x260580 R_X86_64_64 _ZTS16PoolingBySlotsOp 0x0
+  0x260588 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+  0x2605A0 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+  0x260678 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+  0x260718 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+  0x260730 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+  0x260748 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+  0x260838 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+  0x260850 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+  0x2608F8 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+  0x260968 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+  0x2609C8 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+  0x2609E0 R_X86_64_64 _ZTIN10tensorflow8OpKernelE 0x0
+  0x260598 R_X86_64_64 _ZTS20PoolingBySlotsGradOp 0x0
+  0x2605B0 R_X86_64_64 _ZTSZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_ 0x0
+  0x2605C0 R_X86_64_64 _ZTIN10tensorflow4core10RefCountedE 0x0
+  0x2605C8 R_X86_64_64 _ZN10tensorflow4core10RefCountedD1Ev 0x0
+  0x2605D0 R_X86_64_64 _ZN10tensorflow4core10RefCountedD0Ev 0x0
+  0x2605E0 R_X86_64_64 _ZTI16PoolingBySlotsOp 0x0
+  0x2605E8 R_X86_64_64 _ZN16PoolingBySlotsOpD1Ev 0x0
+  0x2605F0 R_X86_64_64 _ZN16PoolingBySlotsOpD0Ev 0x0
+  0x2605F8 R_X86_64_64 _ZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextE 0x0
+  0x260600 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+  0x260648 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+  0x2606B8 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+  0x260778 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+  0x2607C0 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+  0x260808 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+  0x260880 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+  0x2608C8 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+  0x260938 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+  0x260998 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+  0x260A10 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+  0x260A58 R_X86_64_64 _ZN10tensorflow8OpKernel7AsAsyncEv 0x0
+  0x260608 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+  0x260650 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+  0x2606C0 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+  0x260780 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+  0x2607C8 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+  0x260810 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+  0x260888 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+  0x2608D0 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+  0x260940 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+  0x2609A0 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+  0x260A18 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+  0x260A60 R_X86_64_64 _ZN10tensorflow8OpKernel11IsExpensiveEv 0x0
+  0x260610 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+  0x260658 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+  0x2606C8 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+  0x260788 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+  0x2607D0 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+  0x260818 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+  0x260890 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+  0x2608D8 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+  0x260948 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+  0x2609A8 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+  0x260A20 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+  0x260A68 R_X86_64_64 _ZNK10tensorflow8OpKernel12const_tensorEv 0x0
+  0x260618 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+  0x260660 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+  0x2606D0 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+  0x260790 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+  0x2607D8 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+  0x260820 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+  0x260898 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+  0x2608E0 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+  0x260950 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+  0x2609B0 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+  0x260A28 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+  0x260A70 R_X86_64_64 _ZNK10tensorflow8OpKernel11TraceStringERKNS_15OpKernelContextEb 0x0
+  0x260628 R_X86_64_64 _ZTI20PoolingBySlotsGradOp 0x0
+  0x260630 R_X86_64_64 _ZN20PoolingBySlotsGradOpD1Ev 0x0
+  0x260638 R_X86_64_64 _ZN20PoolingBySlotsGradOpD0Ev 0x0
+  0x260640 R_X86_64_64 _ZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextE 0x0
+  0x260670 R_X86_64_64 _ZTS13GetSlotFidsOp 0x0
+  0x260688 R_X86_64_64 _ZTSZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_ 0x0
+  0x260698 R_X86_64_64 _ZTI13GetSlotFidsOp 0x0
+  0x2606A0 R_X86_64_64 _ZN13GetSlotFidsOpD1Ev 0x0
+  0x2606A8 R_X86_64_64 _ZN13GetSlotFidsOpD0Ev 0x0
+  0x2606B0 R_X86_64_64 _ZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextE 0x0
+  0x2606E0 R_X86_64_64 _ZTSZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ 0x0
+  0x2606F0 R_X86_64_64 _ZTSZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ 0x0
+  0x260700 R_X86_64_64 _ZTSZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ 0x0
+  0x260710 R_X86_64_64 _ZTS18SplitRaggedBlockOpIfE 0x0
+  0x260728 R_X86_64_64 _ZTS18SplitRaggedBlockOpIiE 0x0
+  0x260740 R_X86_64_64 _ZTS18SplitRaggedBlockOpIlE 0x0
+  0x260758 R_X86_64_64 _ZTI18SplitRaggedBlockOpIfE 0x0
+  0x260760 R_X86_64_64 _ZN18SplitRaggedBlockOpIfED1Ev 0x0
+  0x260768 R_X86_64_64 _ZN18SplitRaggedBlockOpIfED0Ev 0x0
+  0x260770 R_X86_64_64 _ZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextE 0x0
+  0x2607A0 R_X86_64_64 _ZTI18SplitRaggedBlockOpIiE 0x0
+  0x2607A8 R_X86_64_64 _ZN18SplitRaggedBlockOpIiED1Ev 0x0
+  0x2607B0 R_X86_64_64 _ZN18SplitRaggedBlockOpIiED0Ev 0x0
+  0x2607B8 R_X86_64_64 _ZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextE 0x0
+  0x2607E8 R_X86_64_64 _ZTI18SplitRaggedBlockOpIlE 0x0
+  0x2607F0 R_X86_64_64 _ZN18SplitRaggedBlockOpIlED1Ev 0x0
+  0x2607F8 R_X86_64_64 _ZN18SplitRaggedBlockOpIlED0Ev 0x0
+  0x260800 R_X86_64_64 _ZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextE 0x0
+  0x260830 R_X86_64_64 _ZTS22FeatureVecToSegmentsOp 0x0
+  0x260848 R_X86_64_64 _ZTS30UnsortedFeatureVecToSegmentsOp 0x0
+  0x260860 R_X86_64_64 _ZTI22FeatureVecToSegmentsOp 0x0
+  0x260868 R_X86_64_64 _ZN22FeatureVecToSegmentsOpD1Ev 0x0
+  0x260870 R_X86_64_64 _ZN22FeatureVecToSegmentsOpD0Ev 0x0
+  0x260878 R_X86_64_64 _ZN22FeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextE 0x0
+  0x2608A8 R_X86_64_64 _ZTI30UnsortedFeatureVecToSegmentsOp 0x0
+  0x2608B0 R_X86_64_64 _ZN30UnsortedFeatureVecToSegmentsOpD1Ev 0x0
+  0x2608B8 R_X86_64_64 _ZN30UnsortedFeatureVecToSegmentsOpD0Ev 0x0
+  0x2608C0 R_X86_64_64 _ZN30UnsortedFeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextE 0x0
+  0x2608F0 R_X86_64_64 _ZTS14GroupBySlotsOp 0x0
+  0x260908 R_X86_64_64 _ZTSZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_ 0x0
+  0x260918 R_X86_64_64 _ZTI14GroupBySlotsOp 0x0
+  0x260920 R_X86_64_64 _ZN14GroupBySlotsOpD1Ev 0x0
+  0x260928 R_X86_64_64 _ZN14GroupBySlotsOpD0Ev 0x0
+  0x260930 R_X86_64_64 _ZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextE 0x0
+  0x260960 R_X86_64_64 _ZTS17ParseFeatureVecOp 0x0
+  0x260978 R_X86_64_64 _ZTI17ParseFeatureVecOp 0x0
+  0x260980 R_X86_64_64 _ZN17ParseFeatureVecOpD1Ev 0x0
+  0x260988 R_X86_64_64 _ZN17ParseFeatureVecOpD0Ev 0x0
+  0x260990 R_X86_64_64 _ZN17ParseFeatureVecOp7ComputeEPN10tensorflow15OpKernelContextE 0x0
+  0x2609C0 R_X86_64_64 _ZTS6IsInOpIiE 0x0
+  0x2609D8 R_X86_64_64 _ZTS6IsInOpIlE 0x0
+  0x2609F0 R_X86_64_64 _ZTI6IsInOpIiE 0x0
+  0x2609F8 R_X86_64_64 _ZN6IsInOpIiED1Ev 0x0
+  0x260A00 R_X86_64_64 _ZN6IsInOpIiED0Ev 0x0
+  0x260A08 R_X86_64_64 _ZN6IsInOpIiE7ComputeEPN10tensorflow15OpKernelContextE 0x0
+  0x260A38 R_X86_64_64 _ZTI6IsInOpIlE 0x0
+  0x260A40 R_X86_64_64 _ZN6IsInOpIlED1Ev 0x0
+  0x260A48 R_X86_64_64 _ZN6IsInOpIlED0Ev 0x0
+  0x260A50 R_X86_64_64 _ZN6IsInOpIlE7ComputeEPN10tensorflow15OpKernelContextE 0x0
+  0x260CD8 R_X86_64_GLOB_DAT _ZNSt17_Function_handlerIFvllEZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_E9_M_invokeERKSt9_Any_dataOlSA_ 0x0
+  0x260CE0 R_X86_64_GLOB_DAT _ZNSt17_Function_handlerIFvllEZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_E9_M_invokeERKSt9_Any_dataOlSA_ 0x0
+  0x260CE8 R_X86_64_GLOB_DAT _ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated 0x0
+  0x260CF0 R_X86_64_GLOB_DAT _ZGVZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated 0x0
+  0x260CF8 R_X86_64_GLOB_DAT _ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated 0x0
+  0x260D00 R_X86_64_GLOB_DAT _ZNSt9bad_allocD1Ev 0x0
+  0x260D08 R_X86_64_GLOB_DAT _ZGVZZN17ParseFeatureVecOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+  0x260D10 R_X86_64_GLOB_DAT _ZTV18SplitRaggedBlockOpIiE 0x0
+  0x260D18 R_X86_64_GLOB_DAT _ZZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated 0x0
+  0x260D20 R_X86_64_GLOB_DAT _ITM_deregisterTMCloneTable 0x0
+  0x260D28 R_X86_64_GLOB_DAT _ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated 0x0
+  0x260D30 R_X86_64_GLOB_DAT _ZGVZZN22FeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+  0x260D38 R_X86_64_GLOB_DAT _ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated 0x0
+  0x260D40 R_X86_64_GLOB_DAT _ZTV14GroupBySlotsOp 0x0
+  0x260D48 R_X86_64_GLOB_DAT __cxa_finalize 0x0
+  0x260D50 R_X86_64_GLOB_DAT _ZTVSt15basic_stringbufIcSt11char_traitsIcESaIcEE 0x0
+  0x260D58 R_X86_64_GLOB_DAT _ZNSs4_Rep20_S_empty_rep_storageE 0x0
+  0x260D60 R_X86_64_GLOB_DAT _ZTIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ 0x0
+  0x260D68 R_X86_64_GLOB_DAT _ZGVZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated 0x0
+  0x260D70 R_X86_64_GLOB_DAT _ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated 0x0
+  0x260D78 R_X86_64_GLOB_DAT _ZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+  0x260D80 R_X86_64_GLOB_DAT _ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE1_clEiS5_E17vmodule_activated 0x0
+  0x260D88 R_X86_64_GLOB_DAT _ZTV13GetSlotFidsOp 0x0
+  0x260D90 R_X86_64_GLOB_DAT _ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE_clEiS5_E17vmodule_activated 0x0
+  0x260D98 R_X86_64_GLOB_DAT _ZZN5Eigen8internal20manage_caching_sizesENS_6ActionEPlS2_S2_E12m_cacheSizes 0x0
+  0x260DA0 R_X86_64_GLOB_DAT _ZTISt12length_error 0x0
+  0x260DA8 R_X86_64_GLOB_DAT _ZZZN30UnsortedFeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+  0x260DB0 R_X86_64_GLOB_DAT __pthread_key_create 0x0
+  0x260DB8 R_X86_64_GLOB_DAT __gmon_start__ 0x0
+  0x260DC0 R_X86_64_GLOB_DAT _ZTVSt9bad_alloc 0x0
+  0x260DC8 R_X86_64_GLOB_DAT _ZTV17ParseFeatureVecOp 0x0
+  0x260DD0 R_X86_64_GLOB_DAT _ZZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated 0x0
+  0x260DD8 R_X86_64_GLOB_DAT _ZGVZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated 0x0
+  0x260DE0 R_X86_64_GLOB_DAT _ZGVZZN30UnsortedFeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+  0x260DE8 R_X86_64_GLOB_DAT _ZZZN7FidIter7advanceEvENKUliPKcE_clEiS1_E17vmodule_activated 0x0
+  0x260DF0 R_X86_64_GLOB_DAT _ZGVZZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+  0x260DF8 R_X86_64_GLOB_DAT _ZTV30UnsortedFeatureVecToSegmentsOp 0x0
+  0x260E00 R_X86_64_GLOB_DAT _ZTISt9bad_alloc 0x0
+  0x260E08 R_X86_64_GLOB_DAT _ZTIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_ 0x0
+  0x260E10 R_X86_64_GLOB_DAT _ZNSt12length_errorD1Ev 0x0
+  0x260E18 R_X86_64_GLOB_DAT _ZNSt14_Function_base13_Base_managerIZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E10_M_managerERSt9_Any_dataRKS8_St18_Manager_operation 0x0
+  0x260E20 R_X86_64_GLOB_DAT _ZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS4_E17vmodule_activated 0x0
+  0x260E28 R_X86_64_GLOB_DAT _ZGVZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated 0x0
+  0x260E30 R_X86_64_GLOB_DAT _ZTVN10tensorflow4core10RefCountedE 0x0
+  0x260E38 R_X86_64_GLOB_DAT _ZTV16PoolingBySlotsOp 0x0
+  0x260E40 R_X86_64_GLOB_DAT _ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated 0x0
+  0x260E48 R_X86_64_GLOB_DAT _ZGVZN5Eigen8internal20manage_caching_sizesENS_6ActionEPlS2_S2_E12m_cacheSizes 0x0
+  0x260E50 R_X86_64_GLOB_DAT _ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE0_clEiS5_E17vmodule_activated 0x0
+  0x260E58 R_X86_64_GLOB_DAT _ZTIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_ 0x0
+  0x260E60 R_X86_64_GLOB_DAT _ZZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEllENKUliPKcE_clEiS6_E17vmodule_activated 0x0
+  0x260E68 R_X86_64_GLOB_DAT _ZGVZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated 0x0
+  0x260E70 R_X86_64_GLOB_DAT _ZNSt8ios_base4InitD1Ev 0x0
+  0x260E78 R_X86_64_GLOB_DAT _ZZZN20PoolingBySlotsGradOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+  0x260E80 R_X86_64_GLOB_DAT _ZTV20PoolingBySlotsGradOp 0x0
+  0x260E88 R_X86_64_GLOB_DAT _ZNSt14_Function_base13_Base_managerIZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE0_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation 0x0
+  0x260E90 R_X86_64_GLOB_DAT _ZGVZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE0_clEiS5_E17vmodule_activated 0x0
+  0x260E98 R_X86_64_GLOB_DAT _ZNSt17_Function_handlerIFvllEZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E9_M_invokeERKSt9_Any_dataOlSB_ 0x0
+  0x260EA0 R_X86_64_GLOB_DAT _ZNSt14_Function_base13_Base_managerIZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E10_M_managerERSt9_Any_dataRKS8_St18_Manager_operation 0x0
+  0x260EA8 R_X86_64_GLOB_DAT _ZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated 0x0
+  0x260EB0 R_X86_64_GLOB_DAT _ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE1_clEiS5_E17vmodule_activated 0x0
+  0x260EB8 R_X86_64_GLOB_DAT _ZZZN22FeatureVecToSegmentsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+  0x260EC0 R_X86_64_GLOB_DAT _ZGVZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS4_E17vmodule_activated 0x0
+  0x260EC8 R_X86_64_GLOB_DAT _ZNK10tensorflow10DeviceBase29tensorflow_cpu_worker_threadsEv 0x0
+  0x260ED0 R_X86_64_GLOB_DAT _ZGVZZN7FidIter7advanceEvENKUliPKcE_clEiS1_E17vmodule_activated 0x0
+  0x260ED8 R_X86_64_GLOB_DAT _ZNSt14_Function_base13_Base_managerIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation 0x0
+  0x260EE0 R_X86_64_GLOB_DAT _ZNSt14_Function_base13_Base_managerIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E10_M_managerERSt9_Any_dataRKS8_St18_Manager_operation 0x0
+  0x260EE8 R_X86_64_GLOB_DAT _ZGVZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+  0x260EF0 R_X86_64_GLOB_DAT _ZTV18SplitRaggedBlockOpIlE 0x0
+  0x260EF8 R_X86_64_GLOB_DAT _ZTV22FeatureVecToSegmentsOp 0x0
+  0x260F00 R_X86_64_GLOB_DAT _ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated 0x0
+  0x260F08 R_X86_64_GLOB_DAT _ZNSt17_Function_handlerIFvllEZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E9_M_invokeERKSt9_Any_dataOlSB_ 0x0
+  0x260F10 R_X86_64_GLOB_DAT _ZTIZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ 0x0
+  0x260F18 R_X86_64_GLOB_DAT _ZGVZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated 0x0
+  0x260F20 R_X86_64_GLOB_DAT _ZNSt17_Function_handlerIFvllEZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_E9_M_invokeERKSt9_Any_dataOlSB_ 0x0
+  0x260F28 R_X86_64_GLOB_DAT _ZTVSt15basic_streambufIcSt11char_traitsIcEE 0x0
+  0x260F30 R_X86_64_GLOB_DAT _ZGVZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated 0x0
+  0x260F38 R_X86_64_GLOB_DAT _ZZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated 0x0
+  0x260F40 R_X86_64_GLOB_DAT _ZTIZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_ 0x0
+  0x260F48 R_X86_64_GLOB_DAT _ZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated 0x0
+  0x260F50 R_X86_64_GLOB_DAT _ZTVSt9basic_iosIcSt11char_traitsIcEE 0x0
+  0x260F58 R_X86_64_GLOB_DAT _ZZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEllENKUliPKcE_clEiS5_E17vmodule_activated 0x0
+  0x260F60 R_X86_64_GLOB_DAT _ITM_registerTMCloneTable 0x0
+  0x260F68 R_X86_64_GLOB_DAT _ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE0_clEiS5_E17vmodule_activated 0x0
+  0x260F70 R_X86_64_GLOB_DAT _ZTVSt18basic_stringstreamIcSt11char_traitsIcESaIcEE 0x0
+  0x260F78 R_X86_64_GLOB_DAT _ZGVZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+  0x260F80 R_X86_64_GLOB_DAT _ZTVN10tensorflow14kernel_factory17OpKernelRegistrar18PtrOpKernelFactoryE 0x0
+  0x260F88 R_X86_64_GLOB_DAT _ZZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE0_clEllENKUliPKcE_clEiS5_E17vmodule_activated 0x0
+  0x260F90 R_X86_64_GLOB_DAT _ZNSt17_Function_handlerIFvllEZN13GetSlotFidsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE_E9_M_invokeERKSt9_Any_dataOlSA_ 0x0
+  0x260F98 R_X86_64_GLOB_DAT _ZTV6IsInOpIlE 0x0
+  0x260FA0 R_X86_64_GLOB_DAT _ZTTSt18basic_stringstreamIcSt11char_traitsIcESaIcEE 0x0
+  0x260FA8 R_X86_64_GLOB_DAT _ZTV6IsInOpIiE 0x0
+  0x260FB0 R_X86_64_GLOB_DAT _ZTIZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEEUlllE2_ 0x0
+  0x260FB8 R_X86_64_GLOB_DAT _ZZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated 0x0
+  0x260FC0 R_X86_64_GLOB_DAT _ZZZN17ParseFeatureVecOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+  0x260FC8 R_X86_64_GLOB_DAT _ZGVZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS5_E17vmodule_activated 0x0
+  0x260FD0 R_X86_64_GLOB_DAT _ZTV18SplitRaggedBlockOpIfE 0x0
+  0x260FD8 R_X86_64_GLOB_DAT _ZN10tensorflow10DEVICE_CPUE 0x0
+  0x260FE0 R_X86_64_GLOB_DAT _ZGVZZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE0_clEllENKUliPKcE_clEiS5_E17vmodule_activated 0x0
+  0x260FE8 R_X86_64_GLOB_DAT _ZZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE1_clEiS5_E17vmodule_activated 0x0
+  0x260FF0 R_X86_64_GLOB_DAT _ZZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUliPKcE_clEiS4_E17vmodule_activated 0x0
+  0x260FF8 R_X86_64_GLOB_DAT _ZNSt14_Function_base13_Base_managerIZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEEUlllE1_E10_M_managerERSt9_Any_dataRKS7_St18_Manager_operation 0x0
+  0x261488 R_X86_64_64 __gxx_personality_v0 0x0
+  0x261018 R_X86_64_JUMP_SLOT _ZN10tensorflow5OpDefD1Ev 0x0
+  0x261020 R_X86_64_JUMP_SLOT _ZN10tensorflow12OpDefBuilder10SetShapeFnESt8functionIFNS_6StatusEPNS_15shape_inference16InferenceContextEEE 0x0
+  0x261028 R_X86_64_JUMP_SLOT _ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEE8allocateEm 0x0
+  0x261030 R_X86_64_JUMP_SLOT _ZN10tensorflow15shape_inference19DimensionOrConstantC1El 0x0
+  0x261038 R_X86_64_JUMP_SLOT _ZNSt12length_errorC1EPKc 0x0
+  0x261040 R_X86_64_JUMP_SLOT _ZNK10tensorflow15TensorShapeBaseINS_11TensorShapeEE8dim_sizeEi 0x0
+  0x261048 R_X86_64_JUMP_SLOT _ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm2EEEvN4absl14lts_2020_09_234SpanIKlEEPSt5arrayIlXT_EE 0x0
+  0x261050 R_X86_64_JUMP_SLOT _ZSt19__throw_logic_errorPKc 0x0
+  0x261058 R_X86_64_JUMP_SLOT _ZN10tensorflow15OpKernelContext10CtxFailureEPKciRKNS_6StatusE 0x0
+  0x261060 R_X86_64_JUMP_SLOT __cxa_begin_catch 0x0
+  0x261068 R_X86_64_JUMP_SLOT _ZZN18SplitRaggedBlockOpIlE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEll 0x0
+  0x261070 R_X86_64_JUMP_SLOT memcpy 0x0
+  0x261078 R_X86_64_JUMP_SLOT _ZSt17__throw_bad_allocv 0x0
+  0x261080 R_X86_64_JUMP_SLOT _ZZN14GroupBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE1_clEll 0x0
+  0x261088 R_X86_64_JUMP_SLOT _ZNSt18basic_stringstreamIcSt11char_traitsIcESaIcEED1Ev 0x0
+  0x261090 R_X86_64_JUMP_SLOT _ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKS9_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSH_EEEEKNS3_ILln1EKNS3_ILln1EKNS4_INS5_ISH_Li3ELi1ElEELi16ES7_EEEEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE1EE3runERSW_RKSX_ 0x0
+  0x261098 R_X86_64_JUMP_SLOT _ZN5Eigen8internal19throw_std_bad_allocEv 0x0
+  0x2610A0 R_X86_64_JUMP_SLOT _ZN10tensorflow22CheckNotInComputeAsyncEPNS_15OpKernelContextEPKc 0x0
+  0x2610A8 R_X86_64_JUMP_SLOT _ZN10tensorflow15shape_inference19DimensionOrConstantC1ENS0_15DimensionHandleE 0x0
+  0x2610B0 R_X86_64_JUMP_SLOT _Znwm 0x0
+  0x2610B8 R_X86_64_JUMP_SLOT memmove 0x0
+  0x2610C0 R_X86_64_JUMP_SLOT _ZN10tensorflow11register_op19OpDefBuilderWrapperclEv 0x0
+  0x2610C8 R_X86_64_JUMP_SLOT __assert_fail 0x0
+  0x2610D0 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal10LogMessageC1EPKcii 0x0
+  0x2610D8 R_X86_64_JUMP_SLOT _ZN10tensorflow12OpDefBuilder4AttrESs 0x0
+  0x2610E0 R_X86_64_JUMP_SLOT free 0x0
+  0x2610E8 R_X86_64_JUMP_SLOT _ZNK10tensorflow6Tensor9CheckTypeENS_8DataTypeE 0x0
+  0x2610F0 R_X86_64_JUMP_SLOT _ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev 0x0
+  0x2610F8 R_X86_64_JUMP_SLOT _ZN10tensorflow6StatusC1ENS_5error4CodeEN4absl14lts_2020_09_2311string_viewEOSt6vectorINS_10StackFrameESaIS7_EE 0x0
+  0x261100 R_X86_64_JUMP_SLOT _ZNK10tensorflow11TensorShape10IsSameSizeERKS0_ 0x0
+  0x261108 R_X86_64_JUMP_SLOT _ZZN18SplitRaggedBlockOpIiE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEll 0x0
+  0x261110 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal17MakeCheckOpStringIliEEPSsRKT_RKT0_PKc 0x0
+  0x261118 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal10LogMessage16VmoduleActivatedEPKci 0x0
+  0x261120 R_X86_64_JUMP_SLOT _ZN10tensorflow15shape_inference16InferenceContext10ReplaceDimENS0_11ShapeHandleElNS0_15DimensionHandleEPS2_ 0x0
+  0x261128 R_X86_64_JUMP_SLOT _ZN5Eigen8internal21queryCacheSizes_intelERiS1_S1_i 0x0
+  0x261130 R_X86_64_JUMP_SLOT _ZNK10tensorflow15OpKernelContext5inputEi 0x0
+  0x261138 R_X86_64_JUMP_SLOT _ZNSt6vectorIN5Eigen8internal27TensorBlockScratchAllocatorINS0_13DefaultDeviceEE10AllocationESaIS5_EE17_M_realloc_insertIJRKS5_EEEvN9__gnu_cxx17__normal_iteratorIPS5_S7_EEDpOT_ 0x0
+  0x261140 R_X86_64_JUMP_SLOT __stack_chk_fail 0x0
+  0x261148 R_X86_64_JUMP_SLOT _ZN10tensorflow6thread10ThreadPool11ParallelForEllRKSt8functionIFvllEE 0x0
+  0x261150 R_X86_64_JUMP_SLOT _ZN10tensorflow14kernel_factory17OpKernelRegistrarC1EPKNS_9KernelDefEN4absl14lts_2020_09_2311string_viewEPFPNS_8OpKernelEPNS_20OpKernelConstructionEE 0x0
+  0x261158 R_X86_64_JUMP_SLOT _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC2ERS9_RKSA_ 0x0
+  0x261160 R_X86_64_JUMP_SLOT memset 0x0
+  0x261168 R_X86_64_JUMP_SLOT _ZN10tensorflow6errors15InvalidArgumentIJPKcEEENS_6StatusEDpT_ 0x0
+  0x261170 R_X86_64_JUMP_SLOT _ZNSolsEi 0x0
+  0x261178 R_X86_64_JUMP_SLOT _ZN10tensorflow11register_op19OpDefBuilderWrapper10SetShapeFnESt8functionIFNS_6StatusEPNS_15shape_inference16InferenceContextEEE 0x0
+  0x261180 R_X86_64_JUMP_SLOT _ZN10tensorflow11register_op19OpDefBuilderWrapper5InputESs 0x0
+  0x261188 R_X86_64_JUMP_SLOT __cxa_guard_acquire 0x0
+  0x261190 R_X86_64_JUMP_SLOT _ZNSt9basic_iosIcSt11char_traitsIcEE4initEPSt15basic_streambufIcS1_E 0x0
+  0x261198 R_X86_64_JUMP_SLOT _ZNSo9_M_insertIlEERSoT_ 0x0
+  0x2611A0 R_X86_64_JUMP_SLOT __cxa_allocate_exception 0x0
+  0x2611A8 R_X86_64_JUMP_SLOT strlen 0x0
+  0x2611B0 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal10LogMessageD1Ev 0x0
+  0x2611B8 R_X86_64_JUMP_SLOT _ZN10tensorflow16KernelDefBuilderC2EPKc 0x0
+  0x2611C0 R_X86_64_JUMP_SLOT _ZNK10tensorflow6Tensor4dataEv 0x0
+  0x2611C8 R_X86_64_JUMP_SLOT __cxa_guard_abort 0x0
+  0x2611D0 R_X86_64_JUMP_SLOT _ZN6google15dense_hashtableISt4pairIKliElNSt3tr14hashIlEENS_14dense_hash_mapIliS6_St8equal_toIlENS_27libc_allocator_with_reallocIS3_EEE9SelectKeyENSC_6SetKeyES9_SB_EC1ERKSF_m 0x0
+  0x2611D8 R_X86_64_JUMP_SLOT _ZNSo9_M_insertImEERSoT_ 0x0
+  0x2611E0 R_X86_64_JUMP_SLOT _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_ 0x0
+  0x2611E8 R_X86_64_JUMP_SLOT _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS1_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC1ERS9_RKSA_ 0x0
+  0x2611F0 R_X86_64_JUMP_SLOT _ZN5Eigen8internal27TensorBlockScratchAllocatorINS_13DefaultDeviceEED1Ev 0x0
+  0x2611F8 R_X86_64_JUMP_SLOT _ZNSt6vectorIPN10tensorflow15shape_inference9DimensionESaIS3_EE17_M_realloc_insertIJS3_EEEvN9__gnu_cxx17__normal_iteratorIPS3_S5_EEDpOT_ 0x0
+  0x261200 R_X86_64_JUMP_SLOT _ZdlPv 0x0
+  0x261208 R_X86_64_JUMP_SLOT _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC2ERS8_RKS9_ 0x0
+  0x261210 R_X86_64_JUMP_SLOT _ZN10tensorflow15TensorShapeBaseINS_11TensorShapeEEC1EN4absl14lts_2020_09_234SpanIKlEE 0x0
+  0x261218 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal21CheckOpMessageBuilderD1Ev 0x0
+  0x261220 R_X86_64_JUMP_SLOT __cxa_guard_release 0x0
+  0x261228 R_X86_64_JUMP_SLOT _ZN10tensorflow16KernelDefBuilderD2Ev 0x0
+  0x261230 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal15LogMessageFatalC1EPKci 0x0
+  0x261238 R_X86_64_JUMP_SLOT _ZN10tensorflow12OpDefBuilder5InputESs 0x0
+  0x261240 R_X86_64_JUMP_SLOT _ZNSs4swapERSs 0x0
+  0x261248 R_X86_64_JUMP_SLOT _ZN10tensorflow12OpDefBuilderC1ESs 0x0
+  0x261250 R_X86_64_JUMP_SLOT _ZN10tensorflow16KernelDefBuilder5BuildEv 0x0
+  0x261258 R_X86_64_JUMP_SLOT _ZN10tensorflow14TensorShapeRep19DestructorOutOfLineEv 0x0
+  0x261260 R_X86_64_JUMP_SLOT _ZSt20__throw_length_errorPKc 0x0
+  0x261268 R_X86_64_JUMP_SLOT _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERSA_RKSB_ 0x0
+  0x261270 R_X86_64_JUMP_SLOT _ZN10tensorflow4core10RefCountedD1Ev 0x0
+  0x261278 R_X86_64_JUMP_SLOT __cxa_throw 0x0
+  0x261280 R_X86_64_JUMP_SLOT _ZN5Eigen8internal14TensorExecutorIKNS_14TensorAssignOpINS_16TensorChippingOpILln1ENS3_ILln1ENS_9TensorMapINS_6TensorIfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEEKNS_19TensorCwiseBinaryOpINS0_13scalar_sum_opIffEEKSA_KNS_18TensorCwiseUnaryOpINS0_10bind1st_opINS0_17scalar_product_opIKfSI_EEEEKNS3_ILln1EKNS4_INS5_ISI_Li2ELi1ElEELi16ES7_EEEEEEEEEENS_13DefaultDeviceELb1ELNS0_15TiledEvaluationE0EE3runERSV_RKSW_ 0x0
+  0x261288 R_X86_64_JUMP_SLOT _Unwind_Resume 0x0
+  0x261290 R_X86_64_JUMP_SLOT _ZZN16PoolingBySlotsOp7ComputeEPN10tensorflow15OpKernelContextEENKUlllE0_clEll 0x0
+  0x261298 R_X86_64_JUMP_SLOT _ZN10tensorflow14kernel_factory17OpKernelRegistrar12InitInternalEPKNS_9KernelDefEN4absl14lts_2020_09_2311string_viewESt10unique_ptrINS0_15OpKernelFactoryESt14default_deleteIS9_EE 0x0
+  0x2612A0 R_X86_64_JUMP_SLOT _ZNSs4_Rep9_S_createEmmRKSaIcE 0x0
+  0x2612A8 R_X86_64_JUMP_SLOT _ZZN4absl14lts_2020_09_2311string_view19CheckLengthInternalEmENKUlvE_clEv 0x0
+  0x2612B0 R_X86_64_JUMP_SLOT _ZNSt8ios_baseD2Ev 0x0
+  0x2612B8 R_X86_64_JUMP_SLOT _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS1_ILln1EKNS_9TensorMapINS_6TensorIKfLi3ELi1ElEELi16ENS_11MakePointerEEEEEEENS_13DefaultDeviceEEC1ERSC_RKSD_ 0x0
+  0x2612C0 R_X86_64_JUMP_SLOT _ZSt24__throw_out_of_range_fmtPKcz 0x0
+  0x2612C8 R_X86_64_JUMP_SLOT _ZNSo9_M_insertIdEERSoT_ 0x0
+  0x2612D0 R_X86_64_JUMP_SLOT __cxa_end_catch 0x0
+  0x2612D8 R_X86_64_JUMP_SLOT _ZNSt6localeC1Ev 0x0
+  0x2612E0 R_X86_64_JUMP_SLOT _ZNSs6assignERKSs 0x0
+  0x2612E8 R_X86_64_JUMP_SLOT _ZNSt6vectorIN10tensorflow10StackFrameESaIS1_EED1Ev 0x0
+  0x2612F0 R_X86_64_JUMP_SLOT __cxa_rethrow 0x0
+  0x2612F8 R_X86_64_JUMP_SLOT _ZZNK4absl14lts_2020_09_234SpanIKlEixEmENKUlvE_clEv 0x0
+  0x261300 R_X86_64_JUMP_SLOT _ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE21_M_insert_unique_nodeEmmPNS1_10_Hash_nodeIiLb0EEE 0x0
+  0x261308 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal21CheckOpMessageBuilder7ForVar2Ev 0x0
+  0x261310 R_X86_64_JUMP_SLOT _ZN10tensorflow12OpDefBuilder6OutputESs 0x0
+  0x261318 R_X86_64_JUMP_SLOT _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1EKNS_9TensorMapINS_6TensorIKfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERSA_RKSB_ 0x0
+  0x261320 R_X86_64_JUMP_SLOT __cxa_atexit 0x0
+  0x261328 R_X86_64_JUMP_SLOT _ZNSt10unique_ptrIN10tensorflow6Status5StateESt14default_deleteIS2_EED1Ev 0x0
+  0x261330 R_X86_64_JUMP_SLOT _ZN10tensorflow11register_op19OpDefBuilderWrapper6OutputESs 0x0
+  0x261338 R_X86_64_JUMP_SLOT __cxa_free_exception 0x0
+  0x261340 R_X86_64_JUMP_SLOT _ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE21_M_insert_unique_nodeEmmPNS1_10_Hash_nodeIlLb0EEE 0x0
+  0x261348 R_X86_64_JUMP_SLOT malloc 0x0
+  0x261350 R_X86_64_JUMP_SLOT _ZN10tensorflow16KernelDefBuilder6DeviceEPKc 0x0
+  0x261358 R_X86_64_JUMP_SLOT _ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm1EEEvN4absl14lts_2020_09_234SpanIKlEEPSt5arrayIlXT_EE 0x0
+  0x261360 R_X86_64_JUMP_SLOT _ZNSt10_HashtableIllSaIlENSt8__detail9_IdentityESt8equal_toIlESt4hashIlENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE9_M_rehashEmRKm 0x0
+  0x261368 R_X86_64_JUMP_SLOT _ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEED1Ev 0x0
+  0x261370 R_X86_64_JUMP_SLOT _ZNKSt8__detail20_Prime_rehash_policy11_M_next_bktEm 0x0
+  0x261378 R_X86_64_JUMP_SLOT _ZN10tensorflow11register_op19OpDefBuilderWrapperC1EPKc 0x0
+  0x261380 R_X86_64_JUMP_SLOT _ZN10tensorflow7strings6StrCatERKNS0_8AlphaNumE 0x0
+  0x261388 R_X86_64_JUMP_SLOT _ZNSt10_HashtableIiiSaIiENSt8__detail9_IdentityESt8equal_toIiESt4hashIiENS1_18_Mod_range_hashingENS1_20_Default_ranged_hashENS1_20_Prime_rehash_policyENS1_17_Hashtable_traitsILb0ELb1ELb1EEEE9_M_rehashEmRKm 0x0
+  0x261390 R_X86_64_JUMP_SLOT _ZNSs4_Rep10_M_destroyERKSaIcE 0x0
+  0x261398 R_X86_64_JUMP_SLOT _ZSt16__ostream_insertIcSt11char_traitsIcEERSt13basic_ostreamIT_T0_ES6_PKS3_l 0x0
+  0x2613A0 R_X86_64_JUMP_SLOT _ZNSt8ios_baseC2Ev 0x0
+  0x2613A8 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal21CheckOpMessageBuilder9NewStringEv 0x0
+  0x2613B0 R_X86_64_JUMP_SLOT _ZNSt6localeD1Ev 0x0
+  0x2613B8 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal17MakeCheckOpStringImmEEPSsRKT_RKT0_PKc 0x0
+  0x2613C0 R_X86_64_JUMP_SLOT _ZNSt8ios_base4InitC1Ev 0x0
+  0x2613C8 R_X86_64_JUMP_SLOT _ZNK10tensorflow6Tensor30CheckIsAlignedAndSingleElementEv 0x0
+  0x2613D0 R_X86_64_JUMP_SLOT _ZN10tensorflow15shape_inference16InferenceContext8WithRankENS0_11ShapeHandleElPS2_ 0x0
+  0x2613D8 R_X86_64_JUMP_SLOT _ZN10tensorflow15OpKernelContext15allocate_outputEiRKNS_11TensorShapeEPPNS_6TensorE 0x0
+  0x2613E0 R_X86_64_JUMP_SLOT _ZN10tensorflow8OpKernelC2EPNS_20OpKernelConstructionE 0x0
+  0x2613E8 R_X86_64_JUMP_SLOT _ZNSt6vectorIlSaIlEE17_M_realloc_insertIJRKlEEEvN9__gnu_cxx17__normal_iteratorIPlS1_EEDpOT_ 0x0
+  0x2613F0 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal21CheckOpMessageBuilderC1EPKc 0x0
+  0x2613F8 R_X86_64_JUMP_SLOT _ZZN18SplitRaggedBlockOpIfE7ComputeEPN10tensorflow15OpKernelContextEENKUlllE2_clEll 0x0
+  0x261400 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal15LogMessageFatalD1Ev 0x0
+  0x261408 R_X86_64_JUMP_SLOT _ZN10tensorflow8OpKernelD2Ev 0x0
+  0x261410 R_X86_64_JUMP_SLOT _ZNSt9basic_iosIcSt11char_traitsIcEE5clearESt12_Ios_Iostate 0x0
+  0x261418 R_X86_64_JUMP_SLOT _ZN5Eigen8internal13TensorBlockIOIflLi3ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi3EEE 0x0
+  0x261420 R_X86_64_JUMP_SLOT _ZN10tensorflow12OpDefBuilderD1Ev 0x0
+  0x261428 R_X86_64_JUMP_SLOT _ZNK10tensorflow6Tensor21CheckTypeAndIsAlignedENS_8DataTypeE 0x0
+  0x261430 R_X86_64_JUMP_SLOT _ZNK10tensorflow6Tensor34FillDimsAndValidateCompatibleShapeILm3EEEvN4absl14lts_2020_09_234SpanIKlEEPSt5arrayIlXT_EE 0x0
+  0x261438 R_X86_64_JUMP_SLOT _ZN10tensorflow15shape_inference9DimensionC1El 0x0
+  0x261440 R_X86_64_JUMP_SLOT _ZN5Eigen15TensorEvaluatorIKNS_16TensorChippingOpILln1ENS_9TensorMapINS_6TensorIfLi2ELi1ElEELi16ENS_11MakePointerEEEEENS_13DefaultDeviceEEC1ERS8_RKS9_ 0x0
+  0x261448 R_X86_64_JUMP_SLOT _ZN10tensorflow15shape_inference16InferenceContext9MakeShapeESt16initializer_listINS0_19DimensionOrConstantEE 0x0
+  0x261450 R_X86_64_JUMP_SLOT _ZN5Eigen8internal13TensorBlockIOIflLi2ELi1EE4CopyERKNS2_3DstERKNS2_3SrcERKNS_6DSizesIiLi2EEE 0x0
+  0x261458 R_X86_64_JUMP_SLOT _ZNKSt8__detail20_Prime_rehash_policy14_M_need_rehashEmmm 0x0
+  0x261460 R_X86_64_JUMP_SLOT _ZN10tensorflow16KernelDefBuilder14TypeConstraintEPKcNS_8DataTypeE 0x0
+  0x261468 R_X86_64_JUMP_SLOT _ZNSsC1EPKcRKSaIcE 0x0
+  0x261470 R_X86_64_JUMP_SLOT _ZN10tensorflow15OpKernelContext21CtxFailureWithWarningEPKciRKNS_6StatusE 0x0
+  0x261478 R_X86_64_JUMP_SLOT _ZN10tensorflow8internal17MakeCheckOpStringIllEEPSsRKT_RKT0_PKc 0x0
+}
```

## tensorflow_hs_addon/python/ops/reco_ops.py

```diff
@@ -2,35 +2,38 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 from tensorflow.python.framework import load_library
 from tensorflow.python.platform import resource_loader
 from tensorflow.python.framework import ops
+import tensorflow
 
 
 lib_path = resource_loader.get_path_to_datafile('_reco_ops.so')
 reco_ops = load_library.load_op_library(lib_path)
 
-group_by_slots = reco_ops.group_by_slots
-split_ragged_block = reco_ops.split_ragged_block
-
 pooling_by_slots = reco_ops.pooling_by_slots
 pooling_by_slots_grad = reco_ops.pooling_by_slots_grad
 
 get_slot_fids = reco_ops.get_slot_fids
 
+feature_vec_to_segments = reco_ops.feature_vec_to_segments
+unsorted_feature_vec_to_segments = reco_ops.unsorted_feature_vec_to_segments
+
+parse_feature_vec = reco_ops.parse_feature_vec
+
 
 def isin(values, filter):
     return reco_ops.tfhs_is_in(values, filter)
 
 
 @ops.RegisterGradient("PoolingBySlots")
 def _feature_pooling_grad(op, pooled_grad, *unused):
     fid_indices, fid_slots, fid_weights, unique_embeddings, slots = op.inputs
-    #print("grad inputs", fid_indices, fid_slots, fid_weights, unique_embeddings, slots)
-    #print("grad outputs", op.outputs[0], op.outputs[1])
-    #print("pooled grad", pooled_grad)
+    # print("grad inputs", fid_indices, fid_slots, fid_weights, unique_embeddings, slots)
+    # print("grad outputs", op.outputs[0], op.outputs[1])
+    # print("pooled grad", pooled_grad)
 
     grad = pooling_by_slots_grad(
         fid_indices, fid_slots, fid_weights, unique_embeddings, pooled_grad, slots)
     return [None, None, None, grad, None]
```

## Comparing `tensorflow_hs_addon-0.0.4.dist-info/LICENSE` & `tensorflow_hs_addon-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tensorflow_hs_addon-0.0.4.dist-info/METADATA` & `tensorflow_hs_addon-0.0.5.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: tensorflow-hs-addon
-Version: 0.0.4
+Version: 0.0.5
 Summary: tensorflow-custom-ops is an examples for custom ops for TensorFlow
-Home-page: UNKNOWN
 Author: Google Inc.
 Author-email: opensource@google.com
 License: Apache 2.0
 Keywords: tensorflow custom op machine learning
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
@@ -19,9 +17,7 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
 Requires-Dist: tensorflow (>=2.5.0)
 
-UNKNOWN
-
```

## Comparing `tensorflow_hs_addon-0.0.4.dist-info/RECORD` & `tensorflow_hs_addon-0.0.5.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-tensorflow_hs_addon/__init__.py,sha256=maFA7Fuoer1CHRVvOdLr4xkJqDKmE_fNVkVDwPS8aRw,165
+tensorflow_hs_addon/__init__.py,sha256=GP34wTO6UimigKKm_PGKM_WdoQEtdPR4BbbHH8K9Fdo,216
 tensorflow_hs_addon/python/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tensorflow_hs_addon/python/ops/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tensorflow_hs_addon/python/ops/_reco_ops.so,sha256=voH0Ah2uhfLGrkcdv1POa1Fk_Uq_UN9tlbzLQwnuJ2U,240080
-tensorflow_hs_addon/python/ops/reco_ops.py,sha256=cZtsg5k2G1flY74JSU2TXCSRnO9vZU8KhRMihpoOQfQ,1205
-tensorflow_hs_addon-0.0.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-tensorflow_hs_addon-0.0.4.dist-info/METADATA,sha256=PPa2VHOxKd7EffSVl3djB3iUWiVcxa5R5guEZjXi_kQ,998
-tensorflow_hs_addon-0.0.4.dist-info/WHEEL,sha256=OERMYppr9MrFNH42dDDDfOcxOhh5Bh5GM82gXZaphW4,111
-tensorflow_hs_addon-0.0.4.dist-info/top_level.txt,sha256=Wn4b5da7c1r2Jl4dfITWm8A4LjXZs4xlKjb8lNn3JhQ,20
-tensorflow_hs_addon-0.0.4.dist-info/RECORD,,
+tensorflow_hs_addon/python/ops/_reco_ops.so,sha256=Vxixf0HIC4Xl6zR5olPobMXZwjqZwp4pYRwnVlXgkx8,454424
+tensorflow_hs_addon/python/ops/reco_ops.py,sha256=IMCXglu7rtyBE3--WxPojtzcSDDBFTYfuYaoOBK7vm0,1320
+tensorflow_hs_addon/python/ops/test.py,sha256=X7jxYPbze0K1WKTYUmEV6YMGtj2XEpHWhXKnf06wIQg,6951
+tensorflow_hs_addon-0.0.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+tensorflow_hs_addon-0.0.5.dist-info/METADATA,sha256=yhOh3SW43Ve-xQ-wG4GaeM82UucbCOSgOlR8u6jBGuU,952
+tensorflow_hs_addon-0.0.5.dist-info/WHEEL,sha256=emAqEHGNSYSq0RZ8xpOvIfw0eVJRhiVt8BUGEyWshfE,104
+tensorflow_hs_addon-0.0.5.dist-info/top_level.txt,sha256=Wn4b5da7c1r2Jl4dfITWm8A4LjXZs4xlKjb8lNn3JhQ,20
+tensorflow_hs_addon-0.0.5.dist-info/RECORD,,
```

