# Comparing `tmp/triton_xpu-3.0.0b1-cp39-cp39-manylinux_2_31_x86_64.manylinux_2_35_x86_64.whl.zip` & `tmp/triton_xpu-3.0.0b2-cp39-cp39-manylinux_2_34_x86_64.manylinux_2_35_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,151 +1,160 @@
-Zip file size: 3332332 bytes, number of entries: 149
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:59 triton/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:59 triton_xpu.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:59 triton_xpu-3.0.0b1.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:59 triton/compiler/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:59 triton/language/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:59 triton/backends/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:59 triton/_C/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:59 triton/ops/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:59 triton/runtime/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:59 triton/tools/
--rw-r--r--  2.0 unx    18449 b- defN 24-Apr-29 19:59 triton/testing.py
--rw-r--r--  2.0 unx       89 b- defN 24-Apr-29 19:59 triton/errors.py
--rw-r--r--  2.0 unx     1349 b- defN 24-Apr-29 19:59 triton/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 19:59 triton/compiler/make_launcher.py
--rw-r--r--  2.0 unx    55248 b- defN 24-Apr-29 19:59 triton/compiler/code_generator.py
--rw-r--r--  2.0 unx    16434 b- defN 24-Apr-29 19:59 triton/compiler/compiler.py
--rw-r--r--  2.0 unx     1732 b- defN 24-Apr-29 19:59 triton/compiler/errors.py
--rw-r--r--  2.0 unx      256 b- defN 24-Apr-29 19:59 triton/compiler/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:59 triton/language/extra/
--rw-r--r--  2.0 unx     6736 b- defN 24-Apr-29 19:59 triton/language/random.py
--rw-r--r--  2.0 unx    72243 b- defN 24-Apr-29 19:59 triton/language/semantic.py
--rw-r--r--  2.0 unx    13132 b- defN 24-Apr-29 19:59 triton/language/standard.py
--rw-r--r--  2.0 unx    88021 b- defN 24-Apr-29 19:59 triton/language/core.py
--rw-r--r--  2.0 unx     4613 b- defN 24-Apr-29 19:59 triton/language/__init__.py
--rw-r--r--  2.0 unx     7094 b- defN 24-Apr-29 19:59 triton/language/math.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:59 triton/language/extra/intel/
--rw-r--r--  2.0 unx       41 b- defN 24-Apr-29 19:59 triton/language/extra/__init__.py
--rw-r--r--  2.0 unx     1674 b- defN 24-Apr-29 19:59 triton/language/extra/intel/utils.py
--rw-r--r--  2.0 unx    44326 b- defN 24-Apr-29 19:59 triton/language/extra/intel/libdevice.py
--rw-r--r--  2.0 unx      212 b- defN 24-Apr-29 19:59 triton/language/extra/intel/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:59 triton/backends/amd/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:59 triton/backends/intel/
--rw-r--r--  2.0 unx      977 b- defN 24-Apr-29 19:59 triton/backends/driver.py
--rw-r--r--  2.0 unx     2726 b- defN 24-Apr-29 19:59 triton/backends/compiler.py
--rw-r--r--  2.0 unx     1600 b- defN 24-Apr-29 19:59 triton/backends/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:59 triton/backends/amd/include/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:59 triton/backends/amd/lib/
--rw-r--r--  2.0 unx    15959 b- defN 24-Apr-29 19:59 triton/backends/amd/driver.py
--rw-r--r--  2.0 unx     9845 b- defN 24-Apr-29 19:59 triton/backends/amd/compiler.py
--rw-r--r--  2.0 unx     8061 b- defN 24-Apr-29 19:59 triton/backends/amd/driver.c
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:59 triton/backends/amd/include/hip/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/
--rw-r--r--  2.0 unx     6687 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/texture_types.h
--rw-r--r--  2.0 unx     1307 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/hip_hcc.h
--rw-r--r--  2.0 unx     1523 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/hip_fp16.h
--rw-r--r--  2.0 unx     1594 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/hip_complex.h
--rw-r--r--  2.0 unx     1878 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/hip_cooperative_groups.h
--rw-r--r--  2.0 unx     1630 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/hip_vector_types.h
--rw-r--r--  2.0 unx     1438 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/hip_gl_interop.h
--rw-r--r--  2.0 unx     1815 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/math_functions.h
--rw-r--r--  2.0 unx     1237 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/hip_texture_types.h
--rw-r--r--  2.0 unx     8514 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/hip_ext.h
--rw-r--r--  2.0 unx     1755 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/hip_bfloat16.h
--rw-r--r--  2.0 unx     3058 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/hip_runtime.h
--rw-r--r--  2.0 unx     6339 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/hip_deprecated.h
--rw-r--r--  2.0 unx     1304 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/hip_profile.h
--rw-r--r--  2.0 unx   373379 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/hip_runtime_api.h
--rw-r--r--  2.0 unx     1588 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/hip_math_constants.h
--rw-r--r--  2.0 unx     1959 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/surface_types.h
--rw-r--r--  2.0 unx    18816 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/driver_types.h
--rw-r--r--  2.0 unx     1571 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/hip_bf16.h
--rw-r--r--  2.0 unx     2370 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/library_types.h
--rw-r--r--  2.0 unx     3450 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/hip_common.h
--rw-r--r--  2.0 unx     1589 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/device_functions.h
--rw-r--r--  2.0 unx    14764 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/hiprtc.h
--rw-r--r--  2.0 unx     1773 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/channel_descriptor.h
--rw-r--r--  2.0 unx      407 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/hip_version.h
--rw-r--r--  2.0 unx     3151 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/amd_math_functions.h
--rw-r--r--  2.0 unx     1252 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/concepts.hpp
--rw-r--r--  2.0 unx     3652 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/hip_ldg.h
--rw-r--r--  2.0 unx     1830 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/grid_launch.h
--rw-r--r--  2.0 unx    30346 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/amd_hip_bf16.h
--rw-r--r--  2.0 unx     8129 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/functional_grid_launch.hpp
--rw-r--r--  2.0 unx    57854 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/amd_hip_fp16.h
--rw-r--r--  2.0 unx     1370 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/amd_hip_common.h
--rw-r--r--  2.0 unx     3232 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/hsa_helpers.hpp
--rw-r--r--  2.0 unx    14679 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/amd_hip_complex.h
--rw-r--r--  2.0 unx    67925 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/macro_based_grid_launch.hpp
--rw-r--r--  2.0 unx    33980 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/amd_device_functions.h
--rw-r--r--  2.0 unx     5890 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/amd_hip_math_constants.h
--rw-r--r--  2.0 unx     9484 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/amd_hip_bfloat16.h
--rw-r--r--  2.0 unx     7038 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/host_defines.h
--rw-r--r--  2.0 unx    11062 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/amd_surface_functions.h
--rw-r--r--  2.0 unx    32159 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/amd_hip_cooperative_groups.h
--rw-r--r--  2.0 unx     3154 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/program_state.hpp
--rw-r--r--  2.0 unx     5134 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/hip_fp16_math_fwd.h
--rw-r--r--  2.0 unx     9986 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/amd_hip_runtime_pt_api.h
--rw-r--r--  2.0 unx     2715 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/hip_runtime_prof.h
--rw-r--r--  2.0 unx     3860 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/amd_hip_gl_interop.h
--rw-r--r--  2.0 unx     7957 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/hip_cooperative_groups_helper.h
--rw-r--r--  2.0 unx   618543 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/hip_prof_str.h
--rw-r--r--  2.0 unx     1370 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/grid_launch.hpp
--rw-r--r--  2.0 unx    50307 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/amd_hip_atomic.h
--rw-r--r--  2.0 unx     6660 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/hip_fp16_gcc.h
--rw-r--r--  2.0 unx    18966 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/amd_warp_functions.h
--rw-r--r--  2.0 unx    55689 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/amd_hip_vector_types.h
--rw-r--r--  2.0 unx    17787 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/texture_fetch_functions.h
--rw-r--r--  2.0 unx    17000 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/math_fwd.h
--rw-r--r--  2.0 unx    10538 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/ockl_image.h
--rw-r--r--  2.0 unx     5707 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/helpers.hpp
--rw-r--r--  2.0 unx    11708 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/amd_channel_descriptor.h
--rw-r--r--  2.0 unx    18447 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/texture_indirect_functions.h
--rw-r--r--  2.0 unx    14891 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/amd_hip_runtime.h
--rw-r--r--  2.0 unx     1219 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/grid_launch_GGL.hpp
--rw-r--r--  2.0 unx    24202 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/amd_hip_unsafe_atomics.h
--rw-r--r--  2.0 unx     7457 b- defN 24-Apr-29 19:59 triton/backends/amd/include/hip/amd_detail/device_library_decls.h
--rw-r--r--  2.0 unx  2700232 b- defN 24-Apr-29 19:59 triton/backends/amd/lib/opencl.bc
--rw-r--r--  2.0 unx    41568 b- defN 24-Apr-29 19:59 triton/backends/amd/lib/cuda2gcn.bc
--rw-r--r--  2.0 unx   246124 b- defN 24-Apr-29 19:59 triton/backends/amd/lib/ockl.bc
--rw-r--r--  2.0 unx   205964 b- defN 24-Apr-29 19:59 triton/backends/amd/lib/ocml.bc
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:59 triton/backends/intel/bin/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:59 triton/backends/intel/lib/
--rw-r--r--  2.0 unx     2634 b- defN 24-Apr-29 19:59 triton/backends/intel/arch_parser.c
--rw-r--r--  2.0 unx    15137 b- defN 24-Apr-29 19:59 triton/backends/intel/driver.py
--rw-r--r--  2.0 unx     9075 b- defN 24-Apr-29 19:59 triton/backends/intel/compiler.py
--rw-r--r--  2.0 unx    13891 b- defN 24-Apr-29 19:59 triton/backends/intel/driver.c
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 19:59 triton/backends/intel/__init__.py
--rwxr-xr-x  2.0 unx  5104880 b- defN 24-Apr-29 19:59 triton/backends/intel/bin/spirv-dis
--rw-r--r--  2.0 unx  1703916 b- defN 24-Apr-29 19:59 triton/backends/intel/lib/libsycl-spir64-unknown-unknown.bc
--rwxr-xr-x  2.0 unx        0 b- defN 24-Apr-29 19:59 triton/_C/libtriton.so
--rw-r--r--  2.0 unx     1972 b- defN 24-Apr-29 19:59 triton/_C/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-29 19:59 triton/ops/blocksparse/
--rw-r--r--  2.0 unx     9278 b- defN 24-Apr-29 19:59 triton/ops/matmul.py
--rw-r--r--  2.0 unx     6697 b- defN 24-Apr-29 19:59 triton/ops/matmul_perf_model.py
--rw-r--r--  2.0 unx     3451 b- defN 24-Apr-29 19:59 triton/ops/cross_entropy.py
--rw-r--r--  2.0 unx    18201 b- defN 24-Apr-29 19:59 triton/ops/flash_attention.py
--rw-r--r--  2.0 unx      324 b- defN 24-Apr-29 19:59 triton/ops/__init__.py
--rw-r--r--  2.0 unx     8243 b- defN 24-Apr-29 19:59 triton/ops/blocksparse/softmax.py
--rw-r--r--  2.0 unx    15920 b- defN 24-Apr-29 19:59 triton/ops/blocksparse/matmul.py
--rw-r--r--  2.0 unx      100 b- defN 24-Apr-29 19:59 triton/ops/blocksparse/__init__.py
--rw-r--r--  2.0 unx     9759 b- defN 24-Apr-29 19:59 triton/runtime/cache.py
--rw-r--r--  2.0 unx     3292 b- defN 24-Apr-29 19:59 triton/runtime/build.py
--rw-r--r--  2.0 unx    27693 b- defN 24-Apr-29 19:59 triton/runtime/jit.py
--rw-r--r--  2.0 unx     1509 b- defN 24-Apr-29 19:59 triton/runtime/driver.py
--rw-r--r--  2.0 unx    47640 b- defN 24-Apr-29 19:59 triton/runtime/interpreter.py
--rw-r--r--  2.0 unx      787 b- defN 24-Apr-29 19:59 triton/runtime/errors.py
--rw-r--r--  2.0 unx    13556 b- defN 24-Apr-29 19:59 triton/runtime/autotuner.py
--rw-r--r--  2.0 unx      621 b- defN 24-Apr-29 19:59 triton/runtime/__init__.py
--rw-r--r--  2.0 unx     5080 b- defN 24-Apr-29 19:59 triton/tools/disasm.py
--rw-r--r--  2.0 unx    13673 b- defN 24-Apr-29 19:59 triton/tools/build_extern.py
--rw-r--r--  2.0 unx      332 b- defN 24-Apr-29 19:59 triton/tools/compile.h
--rw-r--r--  2.0 unx     6467 b- defN 24-Apr-29 19:59 triton/tools/compile.py
--rw-r--r--  2.0 unx    11871 b- defN 24-Apr-29 19:59 triton/tools/link.py
--rw-r--r--  2.0 unx     2090 b- defN 24-Apr-29 19:59 triton/tools/compile.c
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 19:59 triton/tools/__init__.py
--rw-r--r--  2.0 unx      219 b- defN 24-Apr-29 19:59 triton_xpu-3.0.0b1.dist-info/top_level.txt
--rw-r--r--  2.0 unx      149 b- defN 24-Apr-29 19:59 triton_xpu-3.0.0b1.dist-info/WHEEL
--rw-rw-r--  2.0 unx    12800 b- defN 24-Apr-29 19:59 triton_xpu-3.0.0b1.dist-info/RECORD
--rw-r--r--  2.0 unx     1426 b- defN 24-Apr-29 19:59 triton_xpu-3.0.0b1.dist-info/METADATA
-149 files, 12305463 bytes uncompressed, 3309294 bytes compressed:  73.1%
+Zip file size: 5817132 bytes, number of entries: 158
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton_xpu-3.0.0b2.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton_xpu.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton/compiler/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton/language/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton/backends/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton/_C/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton/ops/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton/runtime/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton/tools/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton/profiler/
+-rw-r--r--  2.0 unx    18449 b- defN 24-May-01 03:17 triton/testing.py
+-rw-r--r--  2.0 unx       89 b- defN 24-May-01 03:17 triton/errors.py
+-rw-r--r--  2.0 unx     1349 b- defN 24-May-01 03:17 triton/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-01 03:17 triton/compiler/make_launcher.py
+-rw-r--r--  2.0 unx    57598 b- defN 24-May-01 03:17 triton/compiler/code_generator.py
+-rw-r--r--  2.0 unx    16445 b- defN 24-May-01 03:17 triton/compiler/compiler.py
+-rw-r--r--  2.0 unx     1732 b- defN 24-May-01 03:17 triton/compiler/errors.py
+-rw-r--r--  2.0 unx      256 b- defN 24-May-01 03:17 triton/compiler/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton/language/extra/
+-rw-r--r--  2.0 unx     6736 b- defN 24-May-01 03:17 triton/language/random.py
+-rw-r--r--  2.0 unx    72753 b- defN 24-May-01 03:17 triton/language/semantic.py
+-rw-r--r--  2.0 unx    13132 b- defN 24-May-01 03:17 triton/language/standard.py
+-rw-r--r--  2.0 unx    88535 b- defN 24-May-01 03:17 triton/language/core.py
+-rw-r--r--  2.0 unx     4722 b- defN 24-May-01 03:17 triton/language/__init__.py
+-rw-r--r--  2.0 unx     7332 b- defN 24-May-01 03:17 triton/language/math.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton/language/extra/intel/
+-rw-r--r--  2.0 unx       41 b- defN 24-May-01 03:17 triton/language/extra/__init__.py
+-rw-r--r--  2.0 unx     1674 b- defN 24-May-01 03:17 triton/language/extra/intel/utils.py
+-rw-r--r--  2.0 unx    44326 b- defN 24-May-01 03:17 triton/language/extra/intel/libdevice.py
+-rw-r--r--  2.0 unx      212 b- defN 24-May-01 03:17 triton/language/extra/intel/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton/backends/amd/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton/backends/intel/
+-rw-r--r--  2.0 unx      977 b- defN 24-May-01 03:17 triton/backends/driver.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-May-01 03:17 triton/backends/compiler.py
+-rw-r--r--  2.0 unx     1600 b- defN 24-May-01 03:17 triton/backends/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton/backends/amd/include/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton/backends/amd/lib/
+-rw-r--r--  2.0 unx    15959 b- defN 24-May-01 03:17 triton/backends/amd/driver.py
+-rw-r--r--  2.0 unx     9917 b- defN 24-May-01 03:17 triton/backends/amd/compiler.py
+-rw-r--r--  2.0 unx     8061 b- defN 24-May-01 03:17 triton/backends/amd/driver.c
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton/backends/amd/include/hip/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/
+-rw-r--r--  2.0 unx     6687 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/texture_types.h
+-rw-r--r--  2.0 unx     1307 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/hip_hcc.h
+-rw-r--r--  2.0 unx     1523 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/hip_fp16.h
+-rw-r--r--  2.0 unx     1594 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/hip_complex.h
+-rw-r--r--  2.0 unx     1878 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/hip_cooperative_groups.h
+-rw-r--r--  2.0 unx     1630 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/hip_vector_types.h
+-rw-r--r--  2.0 unx     1438 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/hip_gl_interop.h
+-rw-r--r--  2.0 unx     1815 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/math_functions.h
+-rw-r--r--  2.0 unx     1237 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/hip_texture_types.h
+-rw-r--r--  2.0 unx     8514 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/hip_ext.h
+-rw-r--r--  2.0 unx     1755 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/hip_bfloat16.h
+-rw-r--r--  2.0 unx     3058 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/hip_runtime.h
+-rw-r--r--  2.0 unx     6339 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/hip_deprecated.h
+-rw-r--r--  2.0 unx     1304 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/hip_profile.h
+-rw-r--r--  2.0 unx   373379 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/hip_runtime_api.h
+-rw-r--r--  2.0 unx     1588 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/hip_math_constants.h
+-rw-r--r--  2.0 unx     1959 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/surface_types.h
+-rw-r--r--  2.0 unx    18816 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/driver_types.h
+-rw-r--r--  2.0 unx     1571 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/hip_bf16.h
+-rw-r--r--  2.0 unx     2370 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/library_types.h
+-rw-r--r--  2.0 unx     3450 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/hip_common.h
+-rw-r--r--  2.0 unx     1589 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/device_functions.h
+-rw-r--r--  2.0 unx    14764 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/hiprtc.h
+-rw-r--r--  2.0 unx     1773 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/channel_descriptor.h
+-rw-r--r--  2.0 unx      407 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/hip_version.h
+-rw-r--r--  2.0 unx     3151 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/amd_math_functions.h
+-rw-r--r--  2.0 unx     1252 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/concepts.hpp
+-rw-r--r--  2.0 unx     3652 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/hip_ldg.h
+-rw-r--r--  2.0 unx     1830 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/grid_launch.h
+-rw-r--r--  2.0 unx    30346 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/amd_hip_bf16.h
+-rw-r--r--  2.0 unx     8129 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/functional_grid_launch.hpp
+-rw-r--r--  2.0 unx    57854 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/amd_hip_fp16.h
+-rw-r--r--  2.0 unx     1370 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/amd_hip_common.h
+-rw-r--r--  2.0 unx     3232 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/hsa_helpers.hpp
+-rw-r--r--  2.0 unx    14679 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/amd_hip_complex.h
+-rw-r--r--  2.0 unx    67925 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/macro_based_grid_launch.hpp
+-rw-r--r--  2.0 unx    33980 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/amd_device_functions.h
+-rw-r--r--  2.0 unx     5890 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/amd_hip_math_constants.h
+-rw-r--r--  2.0 unx     9484 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/amd_hip_bfloat16.h
+-rw-r--r--  2.0 unx     7038 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/host_defines.h
+-rw-r--r--  2.0 unx    11062 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/amd_surface_functions.h
+-rw-r--r--  2.0 unx    32159 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/amd_hip_cooperative_groups.h
+-rw-r--r--  2.0 unx     3154 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/program_state.hpp
+-rw-r--r--  2.0 unx     5134 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/hip_fp16_math_fwd.h
+-rw-r--r--  2.0 unx     9986 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/amd_hip_runtime_pt_api.h
+-rw-r--r--  2.0 unx     2715 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/hip_runtime_prof.h
+-rw-r--r--  2.0 unx     3860 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/amd_hip_gl_interop.h
+-rw-r--r--  2.0 unx     7957 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/hip_cooperative_groups_helper.h
+-rw-r--r--  2.0 unx   618543 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/hip_prof_str.h
+-rw-r--r--  2.0 unx     1370 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/grid_launch.hpp
+-rw-r--r--  2.0 unx    50307 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/amd_hip_atomic.h
+-rw-r--r--  2.0 unx     6660 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/hip_fp16_gcc.h
+-rw-r--r--  2.0 unx    18966 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/amd_warp_functions.h
+-rw-r--r--  2.0 unx    55689 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/amd_hip_vector_types.h
+-rw-r--r--  2.0 unx    17787 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/texture_fetch_functions.h
+-rw-r--r--  2.0 unx    17000 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/math_fwd.h
+-rw-r--r--  2.0 unx    10538 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/ockl_image.h
+-rw-r--r--  2.0 unx     5707 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/helpers.hpp
+-rw-r--r--  2.0 unx    11708 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/amd_channel_descriptor.h
+-rw-r--r--  2.0 unx    18447 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/texture_indirect_functions.h
+-rw-r--r--  2.0 unx    14891 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/amd_hip_runtime.h
+-rw-r--r--  2.0 unx     1219 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/grid_launch_GGL.hpp
+-rw-r--r--  2.0 unx    24202 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/amd_hip_unsafe_atomics.h
+-rw-r--r--  2.0 unx     7457 b- defN 24-May-01 03:17 triton/backends/amd/include/hip/amd_detail/device_library_decls.h
+-rw-r--r--  2.0 unx  2700232 b- defN 24-May-01 03:17 triton/backends/amd/lib/opencl.bc
+-rw-r--r--  2.0 unx    41568 b- defN 24-May-01 03:17 triton/backends/amd/lib/cuda2gcn.bc
+-rw-r--r--  2.0 unx   246124 b- defN 24-May-01 03:17 triton/backends/amd/lib/ockl.bc
+-rw-r--r--  2.0 unx   205964 b- defN 24-May-01 03:17 triton/backends/amd/lib/ocml.bc
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton/backends/intel/bin/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton/backends/intel/lib/
+-rw-r--r--  2.0 unx     2634 b- defN 24-May-01 03:17 triton/backends/intel/arch_parser.c
+-rw-r--r--  2.0 unx    15137 b- defN 24-May-01 03:17 triton/backends/intel/driver.py
+-rw-r--r--  2.0 unx     8589 b- defN 24-May-01 03:17 triton/backends/intel/compiler.py
+-rw-r--r--  2.0 unx    13891 b- defN 24-May-01 03:17 triton/backends/intel/driver.c
+-rw-r--r--  2.0 unx        0 b- defN 24-May-01 03:17 triton/backends/intel/__init__.py
+-rwxr-xr-x  2.0 unx  5104880 b- defN 24-May-01 03:17 triton/backends/intel/bin/spirv-dis
+-rw-r--r--  2.0 unx  1703916 b- defN 24-May-01 03:17 triton/backends/intel/lib/libsycl-spir64-unknown-unknown.bc
+-rwxr-xr-x  2.0 unx        0 b- defN 24-May-01 03:17 triton/_C/libtriton.so
+-rwxr-xr-x  2.0 unx 10462160 b- defN 24-May-01 03:17 triton/_C/libproton.so
+-rw-r--r--  2.0 unx     1972 b- defN 24-May-01 03:17 triton/_C/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-01 03:17 triton/ops/blocksparse/
+-rw-r--r--  2.0 unx     9278 b- defN 24-May-01 03:17 triton/ops/matmul.py
+-rw-r--r--  2.0 unx     6697 b- defN 24-May-01 03:17 triton/ops/matmul_perf_model.py
+-rw-r--r--  2.0 unx     3451 b- defN 24-May-01 03:17 triton/ops/cross_entropy.py
+-rw-r--r--  2.0 unx    18201 b- defN 24-May-01 03:17 triton/ops/flash_attention.py
+-rw-r--r--  2.0 unx      324 b- defN 24-May-01 03:17 triton/ops/__init__.py
+-rw-r--r--  2.0 unx     8243 b- defN 24-May-01 03:17 triton/ops/blocksparse/softmax.py
+-rw-r--r--  2.0 unx    15920 b- defN 24-May-01 03:17 triton/ops/blocksparse/matmul.py
+-rw-r--r--  2.0 unx      100 b- defN 24-May-01 03:17 triton/ops/blocksparse/__init__.py
+-rw-r--r--  2.0 unx     9759 b- defN 24-May-01 03:17 triton/runtime/cache.py
+-rw-r--r--  2.0 unx     3292 b- defN 24-May-01 03:17 triton/runtime/build.py
+-rw-r--r--  2.0 unx    27693 b- defN 24-May-01 03:17 triton/runtime/jit.py
+-rw-r--r--  2.0 unx     1509 b- defN 24-May-01 03:17 triton/runtime/driver.py
+-rw-r--r--  2.0 unx    47864 b- defN 24-May-01 03:17 triton/runtime/interpreter.py
+-rw-r--r--  2.0 unx      787 b- defN 24-May-01 03:17 triton/runtime/errors.py
+-rw-r--r--  2.0 unx    13556 b- defN 24-May-01 03:17 triton/runtime/autotuner.py
+-rw-r--r--  2.0 unx      621 b- defN 24-May-01 03:17 triton/runtime/__init__.py
+-rw-r--r--  2.0 unx     5080 b- defN 24-May-01 03:17 triton/tools/disasm.py
+-rw-r--r--  2.0 unx    13673 b- defN 24-May-01 03:17 triton/tools/build_extern.py
+-rw-r--r--  2.0 unx      332 b- defN 24-May-01 03:17 triton/tools/compile.h
+-rw-r--r--  2.0 unx     6467 b- defN 24-May-01 03:17 triton/tools/compile.py
+-rw-r--r--  2.0 unx    11871 b- defN 24-May-01 03:17 triton/tools/link.py
+-rw-r--r--  2.0 unx     2090 b- defN 24-May-01 03:17 triton/tools/compile.c
+-rw-r--r--  2.0 unx        0 b- defN 24-May-01 03:17 triton/tools/__init__.py
+-rw-r--r--  2.0 unx      367 b- defN 24-May-01 03:17 triton/profiler/flags.py
+-rw-r--r--  2.0 unx     1061 b- defN 24-May-01 03:17 triton/profiler/hook.py
+-rw-r--r--  2.0 unx     8178 b- defN 24-May-01 03:17 triton/profiler/viewer.py
+-rw-r--r--  2.0 unx     2563 b- defN 24-May-01 03:17 triton/profiler/scope.py
+-rw-r--r--  2.0 unx     4599 b- defN 24-May-01 03:17 triton/profiler/profile.py
+-rw-r--r--  2.0 unx      184 b- defN 24-May-01 03:17 triton/profiler/__init__.py
+-rw-r--r--  2.0 unx      235 b- defN 24-May-01 03:17 triton_xpu-3.0.0b2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      149 b- defN 24-May-01 03:17 triton_xpu-3.0.0b2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx    13480 b- defN 24-May-01 03:17 triton_xpu-3.0.0b2.dist-info/RECORD
+-rw-r--r--  2.0 unx     1454 b- defN 24-May-01 03:17 triton_xpu-3.0.0b2.dist-info/METADATA
+-rw-r--r--  2.0 unx       63 b- defN 24-May-01 03:17 triton_xpu-3.0.0b2.dist-info/entry_points.txt
+158 files, 22788904 bytes uncompressed, 5792946 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -1,14 +1,14 @@
 Filename: triton/
 Comment: 
 
-Filename: triton_xpu.libs/
+Filename: triton_xpu-3.0.0b2.dist-info/
 Comment: 
 
-Filename: triton_xpu-3.0.0b1.dist-info/
+Filename: triton_xpu.libs/
 Comment: 
 
 Filename: triton/compiler/
 Comment: 
 
 Filename: triton/language/
 Comment: 
@@ -24,14 +24,17 @@
 
 Filename: triton/runtime/
 Comment: 
 
 Filename: triton/tools/
 Comment: 
 
+Filename: triton/profiler/
+Comment: 
+
 Filename: triton/testing.py
 Comment: 
 
 Filename: triton/errors.py
 Comment: 
 
 Filename: triton/__init__.py
@@ -354,14 +357,17 @@
 
 Filename: triton/backends/intel/lib/libsycl-spir64-unknown-unknown.bc
 Comment: 
 
 Filename: triton/_C/libtriton.so
 Comment: 
 
+Filename: triton/_C/libproton.so
+Comment: 
+
 Filename: triton/_C/__init__.py
 Comment: 
 
 Filename: triton/ops/blocksparse/
 Comment: 
 
 Filename: triton/ops/matmul.py
@@ -429,20 +435,41 @@
 
 Filename: triton/tools/compile.c
 Comment: 
 
 Filename: triton/tools/__init__.py
 Comment: 
 
-Filename: triton_xpu-3.0.0b1.dist-info/top_level.txt
+Filename: triton/profiler/flags.py
+Comment: 
+
+Filename: triton/profiler/hook.py
+Comment: 
+
+Filename: triton/profiler/viewer.py
+Comment: 
+
+Filename: triton/profiler/scope.py
+Comment: 
+
+Filename: triton/profiler/profile.py
+Comment: 
+
+Filename: triton/profiler/__init__.py
+Comment: 
+
+Filename: triton_xpu-3.0.0b2.dist-info/top_level.txt
+Comment: 
+
+Filename: triton_xpu-3.0.0b2.dist-info/WHEEL
 Comment: 
 
-Filename: triton_xpu-3.0.0b1.dist-info/WHEEL
+Filename: triton_xpu-3.0.0b2.dist-info/RECORD
 Comment: 
 
-Filename: triton_xpu-3.0.0b1.dist-info/RECORD
+Filename: triton_xpu-3.0.0b2.dist-info/METADATA
 Comment: 
 
-Filename: triton_xpu-3.0.0b1.dist-info/METADATA
+Filename: triton_xpu-3.0.0b2.dist-info/entry_points.txt
 Comment: 
 
 Zip file comment:
```

## triton/__init__.py

```diff
@@ -1,9 +1,9 @@
 """isort:skip_file"""
-__version__ = '3.0.0b1'
+__version__ = '3.0.0b2'
 
 # ---------------------------------------
 # Note: import order is significant here.
 
 # submodules
 from .runtime import (
     autotune,
```

## triton/compiler/code_generator.py

```diff
@@ -1,19 +1,23 @@
 import ast
 import inspect
 import re
 import sys
 import warnings
+import os
+import textwrap
 from typing import Any, Callable, Dict, Optional, Tuple, Type, Union
 from .. import language
 from .._C.libtriton import ir
 from ..language import constexpr, tensor, str_to_ty
+from ..runtime.jit import _normalize_ty
 # ideally we wouldn't need any runtime component
 from ..runtime import JITFunction
 from .errors import (CompilationError, CompileTimeAssertionFailure, UnsupportedLanguageConstruct)
+from types import ModuleType
 
 
 def mangle_ty(ty):
     if ty.is_ptr():
         return 'P' + mangle_ty(ty.element_ty)
     if ty.is_int():
         SIGNED = language.dtype.SIGNEDNESS.SIGNED
@@ -235,42 +239,83 @@
         self.debug = options.debug if debug is None else debug
         self.noinline = noinline
         self.scf_stack = []
         self.ret_type = None
         # SSA-construction
         # name => language.tensor
         self.local_defs: Dict[str, tensor] = {}
-        self.global_uses: Dict[str, tensor] = {}
         self.dereference_name: Callable[[str], Any] = self._define_name_lookup()
         self.fn = None
+        # Are we currently visiting an ast.arg's default value?  These have some
+        # special handling.
+        self.visiting_arg_default_value = False
 
     builtin_namespace: Dict[str, Any] = {_.__name__: _ for _ in (len, list, range, float, int, isinstance, getattr)}
     builtin_namespace.update((
         ('print', language.core.device_print),
         ('min', language.minimum),
         ('max', language.maximum),
     ))
 
     def _unsupported(self, node, message):
         return UnsupportedLanguageConstruct(self.jit_fn.src, node, message)
 
+    def _is_constexpr_global(self, name):
+        absent_marker = object()
+        val = self.gscope.get(name, absent_marker)
+        if val is absent_marker:
+            return False
+
+        if _is_constexpr(val):
+            return True
+
+        if a := self.gscope.get("__annotations__", {}).get(name):
+            return _normalize_ty(a) == "constexpr"
+
+        return False
+
     def _define_name_lookup(self):
 
         def local_lookup(name: str, absent):
             # this needs to be re-fetched from `self` every time, because it gets switched occasionally
-            value = self.lscope.get(name, absent)
-            if value is not absent and name not in self.local_defs:
-                self.global_uses[name] = value
-            return value
+            return self.lscope.get(name, absent)
+
+        def global_lookup(name: str, absent):
+            val = self.gscope.get(name, absent)
+            # The high-level rule is that only constexpr globals are allowed.
+            # But actually a bunch of other things, such as module imports, are
+            # technically Python globals. We have to allow these too!
+            if (val is absent  #
+                    or name in self.builtin_namespace  #
+                    or type(val) == ModuleType  #
+                    or isinstance(val, JITFunction)  #
+                    or getattr(val, "__triton_builtin__", False)  #
+                    or getattr(val, "__module__", "").startswith("triton.language")  #
+                    or isinstance(val, language.dtype)  #
+                    or self._is_constexpr_global(name)  #
+                    # Allow accesses to globals while visiting an ast.arg
+                    # because you should be able to do
+                    #   @triton.jit def fn(x: tl.constexpr = GLOBAL): ...
+                    or self.visiting_arg_default_value  #
+                    or os.environ.get("TRITON_ALLOW_NON_CONSTEXPR_GLOBALS", "0") == "1"):
+                return val
+            raise NameError(
+                textwrap.dedent(f"""\
+                Cannot access global variable {name} from within @jit'ed
+                function. Triton kernels can only access global variables that
+                are annotated as constexpr (`x: triton.language.constexpr = 42`
+                or `x = triton.language.constexpr(42)`).  Alternatively, set the
+                envvar TRITON_ALLOW_NON_CONSTEXPR_GLOBALS=1, but we do not
+                promise to support this forever.""").replace("\n", " "))
 
         absent_marker = object()
 
         def name_lookup(name: str) -> Any:
             absent = absent_marker
-            for lookup_function in local_lookup, self.gscope.get, self.builtin_namespace.get:
+            for lookup_function in local_lookup, global_lookup, self.builtin_namespace.get:
                 value = lookup_function(name, absent)
                 if value is not absent:
                     return value
             raise NameError(f'{name} is not defined')
 
         return name_lookup
 
@@ -356,15 +401,22 @@
             annotation = arg_node.annotation
             name = arg_node.arg
             st_target = ast.Name(id=name, ctx=ast.Store())
             if annotation is None:
                 init_node = ast.Assign(targets=[st_target], value=default_value)
             else:
                 init_node = ast.AnnAssign(target=st_target, value=default_value, annotation=annotation)
-            self.visit(init_node)
+
+            try:
+                assert not self.visiting_arg_default_value
+                self.visiting_arg_default_value = True
+                self.visit(init_node)
+            finally:
+                self.visiting_arg_default_value = False
+
         # initialize function
         visibility = "public" if self.is_kernel else "private"
         self.fn = self.builder.get_or_insert_function(self.module, self.function_name,
                                                       self.prototype.to_ir(self.builder), visibility, self.noinline)
         self.module.push_back(self.fn)
         entry = self.fn.add_entry_block()
         arg_values = []
@@ -770,15 +822,15 @@
             # collect loop-carried values
             names = []
             ret_types = []
             init_args = []
             for name in loop_defs:
                 if name in liveins:
                     # We should not def new constexpr
-                    assert _is_triton_tensor(loop_defs[name]), f'cannoe reassign constxpr {name} in the loop'
+                    assert _is_triton_tensor(loop_defs[name]), f'cannot reassign constxpr {name} in the loop'
                     assert _is_triton_tensor(liveins[name]), f'cannot reasign constexpr {name} in the loop'
                     assert loop_defs[name].type == liveins[name].type, \
                         f'Loop-carried variable {name} has initial type {liveins[name].type} '\
                         f'but is re-assigned to {loop_defs[name].type} in loop! '\
                         f'Please make sure that the type stays consistent.'
 
                     # these are loop-carried values
```

## triton/compiler/compiler.py

```diff
@@ -383,16 +383,16 @@
         if CompiledKernel.launch_enter_hook is None:
             return None
         ret = LazyDict({"name": self.name, "function": self.function, "stream": stream})
         if not isinstance(self.src, ASTSource) or self.src.fn.launch_metadata is None:
             return ret
         arg_dict = {}
         arg_idx = 0
-        for arg_name in self.src.fn.arg_names:
-            if arg_name in self.src.constants:
+        for i, arg_name in enumerate(self.src.fn.arg_names):
+            if i in self.src.fn.constexprs:
                 arg_dict[arg_name] = self.src.constants[arg_name]
             else:
                 arg_dict[arg_name] = args[arg_idx]
                 arg_idx += 1
         ret.add(self.src.fn.launch_metadata, (grid, self.metadata, arg_dict))
         return ret
```

## triton/language/semantic.py

```diff
@@ -1032,14 +1032,23 @@
         # Load by a block pointer: `pointer_type<block_type<>>`
         return _load_block_pointer(ptr, mask, other, boundary_check, padding, cache, eviction, is_volatile, builder)
     else:
         # Load by a tensor of pointers or a pointer of scalar: `block_type<pointer_type<>>` or `pointer_type<>`
         return _load_legacy(ptr, mask, other, boundary_check, padding, cache, eviction, is_volatile, builder)
 
 
+def descriptor_load(desc_ptr: tl.tensor, offsets, cache_modifier: str, eviction_policy: str, type,
+                    builder: ir.builder) -> tl.tensor:
+    offsets = _convert_to_ir_values(builder, offsets, require_i64=False)
+    x = builder.create_descriptor_load(desc_ptr.handle, offsets, type.to_ir(builder),
+                                       _str_to_load_cache_modifier(cache_modifier),
+                                       _str_to_eviction_policy(eviction_policy))
+    return tl.tensor(x, type)
+
+
 def _store_block_pointer(ptr, val, mask, boundary_check, cache, eviction, builder):
     # Store by a block pointer: `pointer_type<block_type<>>`
     # Block pointers can not have the `mask` argument
     if mask is not None:
         raise ValueError("`mask` and `other` arguments cannot be specified for loading block pointers")
 
     # Check same shape and element type
```

## triton/language/core.py

```diff
@@ -1586,14 +1586,26 @@
     cache_modifier = _constexpr_to_value(cache_modifier)
     eviction_policy = _constexpr_to_value(eviction_policy)
     volatile = _constexpr_to_value(volatile)
     return semantic.load(pointer, mask, other, boundary_check, padding_option, cache_modifier, eviction_policy,
                          volatile, _builder)
 
 
+@builtin
+def _experimental_descriptor_load(desc_pointer, offsets, shape, dtype, _builder=None):
+    """
+    Experimental feature to access TMA descriptors loads. This is an escape hatch to easily exercise TTGIR operations.
+    This will be removed in the future and shouldn't be used in production code.
+
+    This loads a tensor of data based on the descriptor and offsets.
+    """
+    type = block_type(dtype.element_ty, shape)
+    return semantic.descriptor_load(desc_pointer, offsets, "", "", type, _builder)
+
+
 @_tensor_member_fn
 @builtin
 def store(pointer, value, mask=None, boundary_check=(), cache_modifier="", eviction_policy="", _builder=None):
     """
     Store a tensor of data into memory locations defined by `pointer`.
 
         (1) If `pointer` is a single element pointer, a scalar is stored.  In
```

## triton/language/__init__.py

```diff
@@ -24,14 +24,15 @@
     zeros_like,
 )
 from .core import (
     PropagateNan,
     TRITON_MAX_TENSOR_NUMEL,
     _experimental_join,
     _experimental_split,
+    _experimental_descriptor_load,
     advance,
     arange,
     associative_scan,
     atomic_add,
     atomic_and,
     atomic_cas,
     atomic_max,
@@ -98,15 +99,16 @@
     uint32,
     uint64,
     uint8,
     view,
     void,
     where,
 )
-from .math import (umulhi, exp, exp2, fma, log, log2, cos, rsqrt, sin, sqrt, sqrt_rn, abs, fdiv, div_rn, erf, floor)
+from .math import (umulhi, exp, exp2, fma, log, log2, cos, rsqrt, sin, sqrt, sqrt_rn, abs, fdiv, div_rn, erf, floor,
+                   ceil)
 from .random import (
     pair_uniform_to_normal,
     philox,
     philox_impl,
     rand,
     rand4x,
     randint,
@@ -117,14 +119,15 @@
 )
 
 __all__ = [
     "PropagateNan",
     "TRITON_MAX_TENSOR_NUMEL",
     "_experimental_join",
     "_experimental_split",
+    "_experimental_descriptor_load",
     "abs",
     "advance",
     "arange",
     "argmax",
     "argmin",
     "associative_scan",
     "atomic_add",
@@ -138,14 +141,15 @@
     "bfloat16",
     "block_type",
     "broadcast",
     "broadcast_to",
     "builtin",
     "cat",
     "cdiv",
+    "ceil",
     "clamp",
     "const",
     "const_pointer_type",
     "constexpr",
     "cos",
     "cumprod",
     "cumsum",
```

## triton/language/math.py

```diff
@@ -226,14 +226,23 @@
 @core._tensor_member_fn
 def floor(x, _builder=None):
     x = core._to_tensor(x, _builder)
     return core.tensor(_builder.create_floor(x.handle), x.type)
 
 
 @core.builtin
+@_check_dtype(dtypes=["fp32", "fp64"])
+@_add_math_1arg_docstr("ceil")
+@core._tensor_member_fn
+def ceil(x, _builder=None):
+    x = core._to_tensor(x, _builder)
+    return core.tensor(_builder.create_ceil(x.handle), x.type)
+
+
+@core.builtin
 @_add_math_3arg_docstr("fused multiply-add")
 def fma(x, y, z, _builder=None):
     x = core._to_tensor(x, _builder)
     y = core._to_tensor(y, _builder)
     z = core._to_tensor(z, _builder)
     x, y = core.binary_op_type_legalization(x, y, _builder)
     z, x = core.binary_op_type_legalization(z, x, _builder)
```

## triton/backends/amd/compiler.py

```diff
@@ -111,29 +111,30 @@
         pm.run(mod)
         return mod
 
     @staticmethod
     def make_ttgir(mod, metadata, options):
         pm = ir.pass_manager(mod.context)
         pm.enable_debug()
-        passes.ttir.add_convert_to_ttgpuir(pm, options.num_warps, options.warp_size, options.num_ctas, None)
+        passes.ttir.add_convert_to_ttgpuir(pm, f"hip:{options.arch}", options.num_warps, options.warp_size,
+                                           options.num_ctas)
         pm.run(mod)
         pm = ir.pass_manager(mod.context)
         pm.enable_debug()
         passes.ttgpuir.add_coalesce(pm)
         amd.passes.ttgpuir.add_remove_layout_conversions(pm)
         passes.ttgpuir.add_optimize_thread_locality(pm)
         amd.passes.ttgpuir.add_accelerate_matmul(pm, options.arch, options.matrix_instr_nonkdim, options.kpack)
         amd.passes.ttgpuir.add_remove_layout_conversions(pm)
         amd.passes.ttgpuir.add_optimize_epilogue(pm)
-        passes.ttgpuir.add_optimize_dot_operands(pm)
+        passes.ttgpuir.add_optimize_dot_operands(pm, True)
         if options.num_stages == 0 and amd.has_matrix_core_feature(options.arch):
             amd.passes.ttgpuir.add_stream_pipeline(pm)
             passes.common.add_canonicalizer(pm)
-        passes.ttgpuir.add_optimize_dot_operands(pm)
+        passes.ttgpuir.add_optimize_dot_operands(pm, True)
         amd.passes.ttgpuir.add_remove_layout_conversions(pm)
         passes.ttgpuir.add_reduce_data_duplication(pm)
         if options.num_stages != 0:
             amd.passes.ttgpuir.add_reorder_instructions(pm)
         passes.common.add_cse(pm)
         passes.common.add_symbol_dce(pm)
         pm.run(mod)
```

## triton/backends/intel/compiler.py

```diff
@@ -116,45 +116,37 @@
         passes.common.add_licm(pm)
         passes.common.add_symbol_dce(pm)
         pm.run(mod)
         return mod
 
     @staticmethod
     def make_ttgir(mod, metadata, opt, device_arch):
-        cluster_info = intel.ClusterInfo()
-        if opt.cluster_dims is not None:
-            cluster_info.clusterDimX = opt.cluster_dims[0]
-            cluster_info.clusterDimY = opt.cluster_dims[1]
-            cluster_info.clusterDimZ = opt.cluster_dims[2]
         # TTIR -> TTGIR
         pm = ir.pass_manager(mod.context)
         pm.enable_debug()
-        passes.ttir.add_convert_to_ttgpuir(pm, opt.num_warps, opt.threads_per_warp, opt.num_ctas, device_arch)
+        passes.ttir.add_convert_to_ttgpuir(pm, f"xpu:{device_arch}", opt.num_warps, opt.threads_per_warp, opt.num_ctas)
         # optimize TTGIR
         passes.ttgpuir.add_coalesce(pm)
-        # TODO(Qingyi): Move PlanCTAPass to the front of CoalescePass
-        intel.passes.ttnvgpuir.add_plan_cta(pm, cluster_info)
         passes.ttgpuir.add_remove_layout_conversions(pm)
         passes.ttgpuir.add_optimize_thread_locality(pm)
         intel.passes.ttgpuir.add_accelerate_matmul(pm, device_arch)
         passes.ttgpuir.add_remove_layout_conversions(pm)
         if opt.optimize_epilogue:
             passes.ttgpuir.add_optimize_epilogue(pm)
-        passes.ttgpuir.add_optimize_dot_operands(pm)
+        passes.ttgpuir.add_optimize_dot_operands(pm, True)
         passes.common.add_cse(pm)
         passes.ttgpuir.add_prefetch(pm)
-        passes.ttgpuir.add_optimize_dot_operands(pm)
+        passes.ttgpuir.add_optimize_dot_operands(pm, True)
         passes.ttgpuir.add_remove_layout_conversions(pm)
         passes.ttgpuir.add_reduce_data_duplication(pm)
         passes.ttgpuir.add_reorder_instructions(pm)
         passes.common.add_cse(pm)
         passes.common.add_symbol_dce(pm)
         passes.common.add_canonicalizer(pm)
         pm.run(mod)
-        metadata["cluster_dims"] = (cluster_info.clusterDimX, cluster_info.clusterDimY, cluster_info.clusterDimZ)
         return mod
 
     @staticmethod
     def make_llir(src, metadata, options, device_arch):
         # warp-specialization mutates num_warps
         num_warp_groups = src.get_int_attr("triton_gpu.num-warp-groups-per-cta")
         if num_warp_groups is not None:
```

## triton/_C/__init__.py

```diff
@@ -11,15 +11,15 @@
 def _target_platform():
     return (
         f'py{sys.version_info.major}.{sys.version_info.minor}'
         f'-{platform.system().lower()}-{platform.machine().lower()}'
     )
 
 
-_version = os.getenv('TRITON_WHEEL_VERSION', '3.0.0b1')
+_version = os.getenv('TRITON_WHEEL_VERSION', '3.0.0b2')
 _debug = os.getenv('TRITON_XPU_DEBUG_IMPORT') is not None
 _platform = _target_platform()
 _cache_home = pathlib.Path(os.getenv('XDG_CACHE_HOME') or os.path.expanduser('~/.cache'))
 _cache_path = _cache_home / 'triton-xpu' / _version / _platform
 _store_path = _cache_path / 'libtriton.so'
 
 if _debug:
```

## triton/runtime/interpreter.py

```diff
@@ -499,14 +499,15 @@
         return TensorHandle(ret, arg.dtype.scalar)
 
     create_cos = lambda self, arg: self.unary_op(arg, np.cos)
     create_exp = lambda self, arg: self.unary_op(arg, np.exp)
     create_exp2 = lambda self, arg: self.unary_op(arg, np.exp2)
     create_iabs = lambda self, arg: self.unary_op(arg, np.abs)
     create_floor = lambda self, arg: self.unary_op(arg, np.floor)
+    create_ceil = lambda self, arg: self.unary_op(arg, np.ceil)
     create_log = lambda self, arg: self.unary_op(arg, np.log)
     create_log2 = lambda self, arg: self.unary_op(arg, np.log2)
     create_precise_sqrt = lambda self, arg: self.unary_op(arg, np.sqrt)
     create_sqrt = lambda self, arg: self.unary_op(arg, np.sqrt)
     create_sin = lambda self, arg: self.unary_op(arg, np.sin)
 
     def create_erf(self, arg):
@@ -611,21 +612,25 @@
 
     def create_extern_elementwise(self, libName, libPath, symbol, argList, retType, isPure):
         raise NotImplementedError("extern_elementwise not supported in interpreter mode")
 
     def create_inline_asm(self, inlineAsm, constraints, values, type, isPure, pack):
         raise NotImplementedError("inline_asm not supported in interpreter mode")
 
-    def create_print(self, prefix, values):
+    def create_print(self, prefix, hex, values):
         # Interpreter's device_print function has a different format than Triton's device_print
         msg = f"({self.grid_idx[0]}, {self.grid_idx[1]}, {self.grid_idx[2]})"
         if prefix:
             msg += f" {prefix}"
+        if hex:
+            np.set_printoptions(formatter={'all': lambda x: f"0x{x:02x}"})
         for value in values:
             print(msg + f" {value.data}")
+        if hex:
+            np.set_printoptions(formatter=None)
 
     def create_assert(self, condition, message, fileName, funcName, lineNo):
         # Interpreter's device_assert function has a different format than Triton's device_assert
         assert condition, f"{message} in {fileName}:{funcName}:{lineNo}"
 
     def create_barrier(self):
         # Triton's barrier applies to each program in a grid, so it's a no-op in the interpreter
```

## Comparing `triton_xpu-3.0.0b1.dist-info/RECORD` & `triton_xpu-3.0.0b2.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 triton/testing.py,sha256=0AVJtM3dm3aLX9wYAeBEi4sa1AelJNLkI4sFJmf_bjw,18449
 triton/errors.py,sha256=8WfnuRKLG578mgY6cBA3ECruVMf9ULEKFNgRcJ6IhWM,89
-triton/__init__.py,sha256=SG59-GvrFeQO3j8dBeGUDfQ4lG-cWGvyBdfaVCXTBBY,1349
+triton/__init__.py,sha256=RZ5ooR6xv8imYNe5aZnUo-k7v5A1QIN3hEWl4cQh0Sk,1349
 triton/compiler/make_launcher.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-triton/compiler/code_generator.py,sha256=SFbSYWSSX9lVx3nY9n7PR8xXVAUrAIcUs6WA1wixPdg,55248
-triton/compiler/compiler.py,sha256=qxtom7rvr1Sbo0vG0W0QPkfSuPLdvsa345HZLG9f-Uc,16434
+triton/compiler/code_generator.py,sha256=8iFIBXwk34RuOra7n9PrXFEKD_ZCaC4Wer5SoFXvi3c,57598
+triton/compiler/compiler.py,sha256=GD2P3F8cnOvXinKmZWjZhQIVmGms7cdfgEqbqRDggrk,16445
 triton/compiler/errors.py,sha256=I9Y15pDWcL9heY4SWWdLeMDtW6Iiq2pFXzKfJ6dY_C0,1732
 triton/compiler/__init__.py,sha256=PD2VOiqnb3qUrti77C_E83lX8Rch-jLVwN98I7XiMRA,256
 triton/language/random.py,sha256=NhMKN68bGaDexWmqCNMLAMdMjwK2tjKZnYbeoWkUZ5I,6736
-triton/language/semantic.py,sha256=_6C37hdjFVeEFLD3QLf5DAGtyGfyt0Vf9LzGeR6Y56Q,72243
+triton/language/semantic.py,sha256=paZNQRbuk1xHDCO5ct0IUvxZjEm2d4bt5_QIclWn4G0,72753
 triton/language/standard.py,sha256=as6VZm9qTs0rGn_HroZdGpI5YIvQIMtuS40VIzwt2bM,13132
-triton/language/core.py,sha256=rImmV0AIpjA7pKW5NnBZeHX1YFv-Vxc6GIKsXvMQDZ4,88021
-triton/language/__init__.py,sha256=diEYqW2GUrycBQ3PLuh1W7gEYBVgcELfpQpwkdUXzrQ,4613
-triton/language/math.py,sha256=udgGkLMQnCqvXs5FDWLpOzfrarOFUgiXlLO7NuNqIrM,7094
+triton/language/core.py,sha256=g41aReuW6BiXi5-NgW_UsQKb9VEMiFFPXY2mXFP1REg,88535
+triton/language/__init__.py,sha256=9dxG0-c2cU7Xa-zNKCZyCKwoQ4yEhShhosEMEo5fvZ0,4722
+triton/language/math.py,sha256=o0vg065LOsmu3hlc_aQvigoJeyvJZC-1lnPOaztgfxA,7332
 triton/language/extra/__init__.py,sha256=D4xBOLkBT00QvoR9NGlMSm1YiV78OYQBnBAhOhCtUH0,41
 triton/language/extra/intel/utils.py,sha256=wwh73ItWacLHiwRfN1sIKyjg07dqJPYzFKwd-XO_bYQ,1674
 triton/language/extra/intel/libdevice.py,sha256=kFuJ9q9MYWjUnP54nw0ZtS-SAEv5KQisHUbze5e2Poc,44326
 triton/language/extra/intel/__init__.py,sha256=HQkHZeHhgjZWs5yTZfK0MoXkNKT-KaCIa0V_884Tb64,212
 triton/backends/driver.py,sha256=9EM4ox4FNCkLCGUwUIBMP6u95AOm0wBK4E8MKElfCAI,977
 triton/backends/compiler.py,sha256=HJE6rbHfu3enS7FgHoxunVK5vj8eqtqFIYiN4owv5PQ,2726
 triton/backends/__init__.py,sha256=IqprKlbbTM6n-JCl6VeE5VU8kVOiaIP7UZSQPz8w4dw,1600
 triton/backends/amd/driver.py,sha256=WZm05plz7mKqMkzs5msaP6ldSLrwSkqIoQ0_D2QVRCQ,15959
-triton/backends/amd/compiler.py,sha256=5gyGBtWlSoWewyy5H3bS8vMZ8RqxlCknnk5_e5acNns,9845
+triton/backends/amd/compiler.py,sha256=T_-Bt3b3wPJS6IWh37IiN01ltmXaXjgHKCIbsi7aaQA,9917
 triton/backends/amd/driver.c,sha256=0lCBWQSHPXEVBiONEKwkUBcPVIj8cYCvga4Rwp6VfXE,8061
 triton/backends/amd/include/hip/texture_types.h,sha256=CtmdykZfDikhnrVfdJk3w2VK5X3Af_6rEKzU-VgLu24,6687
 triton/backends/amd/include/hip/hip_hcc.h,sha256=RYrArDlnTEP89xKbzIpW17_bsBY5moCitq00PL-4oWI,1307
 triton/backends/amd/include/hip/hip_fp16.h,sha256=vKJh-zgDWUW7NyXxtv2ho6aVLXX8BIPfzCigEQ5d6I4,1523
 triton/backends/amd/include/hip/hip_complex.h,sha256=TmdzQP5oVPfhBVARJYcR5eyv9HInmKMFuFoQ_1ECk_I,1594
 triton/backends/amd/include/hip/hip_cooperative_groups.h,sha256=gMLvaYQ3b-f1vcoMtEwtkN0hO5__zNfP5p5oBKmv_SE,1878
 triton/backends/amd/include/hip/hip_vector_types.h,sha256=6FcBMBkP3ZN1Enalpa9hV0VopxdBJvbUCuaxISgzbTY,1630
@@ -88,41 +88,49 @@
 triton/backends/amd/include/hip/amd_detail/device_library_decls.h,sha256=4clSpgf898UVjfZFVnDkcYi75A27crPsuFtLcs1s4KU,7457
 triton/backends/amd/lib/opencl.bc,sha256=92AGfuEI3ms6uxCLB75WCYYyFGUKcIU-8wxo4RhBuzI,2700232
 triton/backends/amd/lib/cuda2gcn.bc,sha256=UDl-zwwWB5Ad__lIlhReRQBx61m0nMORxdppdTxkjQo,41568
 triton/backends/amd/lib/ockl.bc,sha256=wQKCzkKukIHbu0lyjKUYlhndc7S27xto6L54J0Bn-C0,246124
 triton/backends/amd/lib/ocml.bc,sha256=UPNTXW0gCXUNB-c6orSYwb-mz9_mjUc7zny_vfFza44,205964
 triton/backends/intel/arch_parser.c,sha256=qGsQIjM0WU33SrS8zOb6yLOoaJce0Hh4VEjocs50fic,2634
 triton/backends/intel/driver.py,sha256=apukFbeNfm0nSS2PNHNA0fXpMSb4mRffRHLFAIwp8yI,15137
-triton/backends/intel/compiler.py,sha256=Xld9_l6F2z-pPKTF5EiAewlvFsl9quXc-PS495_NCTQ,9075
+triton/backends/intel/compiler.py,sha256=AzTWsntOpOSa4evM2QFSlSLDeQkuSVcArTZHg1QiiEk,8589
 triton/backends/intel/driver.c,sha256=ZUGO1t7iuuLMftZzVLOhxvwsC-MviFDs2rY7rq1XQzs,13891
 triton/backends/intel/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 triton/backends/intel/bin/spirv-dis,sha256=0I840dythPHQTD27JDvLZGJFSxiRwX7tkvOckC1NsP0,5104880
 triton/backends/intel/lib/libsycl-spir64-unknown-unknown.bc,sha256=xYAcoZ9pOKCF31tjtUP-i7CjdG6Q_xPvHI8zW0yiHks,1703916
 triton/_C/libtriton.so,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-triton/_C/__init__.py,sha256=BZiRgy76V6yG4eklr5w6mRSb2nDAt6RRxiVWertt_gc,1972
+triton/_C/libproton.so,sha256=J5JMsFvVP1yWDURDF6pvZL5tfVwIikItCSfaztRNo1g,10462160
+triton/_C/__init__.py,sha256=qWFsK7axTc5mBc1pVW84XhEI0vHzUcpsWsojvMTa_zc,1972
 triton/ops/matmul.py,sha256=epzb56ULAgUDy1JKazPnFqObLOf6F__73eXLInhnD8M,9278
 triton/ops/matmul_perf_model.py,sha256=E8LuqIrb-u_NCqSDD0r9hHNPkPKCTMTKJNAVOuZomaU,6697
 triton/ops/cross_entropy.py,sha256=Jr-iQ6oZQir8gh4WRmlPoh_CY4fM8x9c9dDsuavyFyQ,3451
 triton/ops/flash_attention.py,sha256=Vd2Ydo3VUdnR3-8h8uqQi1lJuG1NlEIoYTnDroH9G9k,18201
 triton/ops/__init__.py,sha256=Yo_IfcP54HxucFaQNc4aOtfOGryUcQZUDA4aONg6sHk,324
 triton/ops/blocksparse/softmax.py,sha256=2jfmu1Bn9XsM4PyBsSRaSi3-XK0bJABxwQ-XsTwo7fg,8243
 triton/ops/blocksparse/matmul.py,sha256=S29Wv0X47AUoCMfSw7A7-Lt6lUyGPzy63Q8pcD41O1w,15920
 triton/ops/blocksparse/__init__.py,sha256=6YEVQNzipgQCpoO_7B8H7ckaSW2Idt1244s7IyLWAwc,100
 triton/runtime/cache.py,sha256=Fmr6AgDubT7XPe9Lan6WE_czbSS7ZFZ__8qkdvaWkSE,9759
 triton/runtime/build.py,sha256=NtvpwIJ7OWViR-ZEFh6oAeaiUGDvi4cqMU7uwRMzDIU,3292
 triton/runtime/jit.py,sha256=-Izp7tsn_xwVZNxBflMw_vQ_MbJ0AtxdvMbVcZaBOZc,27693
 triton/runtime/driver.py,sha256=VZ-883Xri71R72lHB6usIpLo3gGLbZJkAlLP3ewWSpc,1509
-triton/runtime/interpreter.py,sha256=um0-jbT8Uc8dJbA6sfdQzdSzQUUndkMFTvGQ-kIxp3g,47640
+triton/runtime/interpreter.py,sha256=RkAE4o4DG3b_q2LXv1zMC1kDUM5cETvgurDg8NHD1RQ,47864
 triton/runtime/errors.py,sha256=oj73dn34qJbLhOjakakAuZPSv-laZyIYylJiJwREA8Y,787
 triton/runtime/autotuner.py,sha256=DLqSX1gMQ7vBte-eNQ2X6uT_DbUR85SVbVll9Ibt6Fk,13556
 triton/runtime/__init__.py,sha256=mKL5cqIBDUw2WO80NRCh4s1G8KYaqgM59TTAbTkPPjQ,621
 triton/tools/disasm.py,sha256=U58GRL7v14hu4-B_kWkciHaY9jVIkTKg7DtioH4LTHo,5080
 triton/tools/build_extern.py,sha256=jCr-2hu3nLGBIJhCGUQ1jAyzLttughjkiPGEwRFjLR0,13673
 triton/tools/compile.h,sha256=n9QKIFZTL4RSsiXtAxBP9XGSnxjyaevQQ9bBpwDsvAg,332
 triton/tools/compile.py,sha256=1HSZC_qB3ELb0OJmq6fv-FqClBmyzS3EMrtVgMC09C8,6467
 triton/tools/link.py,sha256=u7qtfZRLriZkAMEGNvj8YF-k1cthmLL7BwHYqBgT63E,11871
 triton/tools/compile.c,sha256=rjuAQ8b-2DTtbj29SgK1NxJI5BSU2P9ccp9wa5p8Iyc,2090
 triton/tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-triton_xpu-3.0.0b1.dist-info/top_level.txt,sha256=aIwyEGxBCqWM2O84X9652HjRy5duPG3fjW1wn1s0uxA,219
-triton_xpu-3.0.0b1.dist-info/WHEEL,sha256=MgZk2NznFDwoSBs76co6V39jIRdSDHJgMA0x7hBGfSc,149
-triton_xpu-3.0.0b1.dist-info/RECORD,,
-triton_xpu-3.0.0b1.dist-info/METADATA,sha256=QBAFslY5-l2L7OtOG9sk711aE2BmC0VIU6cZgPq6oD0,1426
+triton/profiler/flags.py,sha256=w8w851Xcm6uMGPzcEk1fZHnTGsbwQR6rlwcwgO3OByY,367
+triton/profiler/hook.py,sha256=8b2vR6sVWbuvWfm5GxoghRBa_wRd7dUbb7h5DEpxvm0,1061
+triton/profiler/viewer.py,sha256=DYzdbyEtvy0-ZyYVdq-7r8o9SVt05LLgfNkjMAPFlZc,8178
+triton/profiler/scope.py,sha256=LCynOCaS0YvOCcvcxzanPpO-X0nQrjPTqqZ8wteqi0o,2563
+triton/profiler/profile.py,sha256=Y81KrG-TnutvQnW0IF3zmqKUj9S1eZ3wNrgyWvw5Teo,4599
+triton/profiler/__init__.py,sha256=8MMGWMNsHxvgFva8l6o9lzUcAdGjpxiQouuTwJ4qkdQ,184
+triton_xpu-3.0.0b2.dist-info/top_level.txt,sha256=CMhcZwd1NMhEyBMOC8qvQ0YwJte-ZSlL748IPOWKbTs,235
+triton_xpu-3.0.0b2.dist-info/WHEEL,sha256=F5-Ql6i2p2wAEM4el9KC13r9bH3eovpktKfHbm4AtDo,149
+triton_xpu-3.0.0b2.dist-info/RECORD,,
+triton_xpu-3.0.0b2.dist-info/METADATA,sha256=qc96rVqfBcKgFt8Kb9oBWsz1Nky3M7WCGmMA4ibanDc,1454
+triton_xpu-3.0.0b2.dist-info/entry_points.txt,sha256=x5h_onixOxXIknHS4Xe1fQgq0lsCTiatIRITAzsXM5M,63
```

## Comparing `triton_xpu-3.0.0b1.dist-info/METADATA` & `triton_xpu-3.0.0b2.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triton-xpu
-Version: 3.0.0b1
+Version: 3.0.0b2
 Summary: A language and compiler for custom Deep Learning operations
 Home-page: https://github.com/openai/triton/
 Author: Philippe Tillet
 Author-email: phil@openai.com
 License: UNKNOWN
 Keywords: Compiler,Deep Learning
 Platform: UNKNOWN
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: filelock
+Requires-Dist: llnl-hatchet
 Provides-Extra: build
 Requires-Dist: cmake >=3.20 ; extra == 'build'
 Requires-Dist: importlib-metadata ; extra == 'build'
 Requires-Dist: lit ; extra == 'build'
 Provides-Extra: tests
 Requires-Dist: autopep8 ; extra == 'tests'
 Requires-Dist: flake8 ; extra == 'tests'
```

