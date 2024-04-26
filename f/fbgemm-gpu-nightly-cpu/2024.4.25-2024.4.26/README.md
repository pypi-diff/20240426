# Comparing `tmp/fbgemm_gpu_nightly_cpu-2024.4.25-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/fbgemm_gpu_nightly_cpu-2024.4.26-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,60 +1,60 @@
-Zip file size: 3149445 bytes, number of entries: 58
--rw-r--r--  2.0 unx      914 b- defN 24-Apr-25 12:54 fbgemm_gpu/__init__.py
--rw-r--r--  2.0 unx     3079 b- defN 24-Apr-25 12:54 fbgemm_gpu/batched_unary_embeddings_ops.py
--rw-r--r--  2.0 unx      789 b- defN 24-Apr-25 12:54 fbgemm_gpu/enums.py
--rwxr-xr-x  2.0 unx 10846712 b- defN 24-Apr-25 12:54 fbgemm_gpu/fbgemm_gpu_py.so
--rw-r--r--  2.0 unx     5663 b- defN 24-Apr-25 12:54 fbgemm_gpu/metrics.py
--rw-r--r--  2.0 unx     2362 b- defN 24-Apr-25 12:54 fbgemm_gpu/permute_pooled_embedding_modules.py
--rw-r--r--  2.0 unx     2752 b- defN 24-Apr-25 12:54 fbgemm_gpu/permute_pooled_embedding_modules_split.py
--rw-r--r--  2.0 unx     7885 b- defN 24-Apr-25 12:54 fbgemm_gpu/quantize_comm.py
--rw-r--r--  2.0 unx     4143 b- defN 24-Apr-25 12:54 fbgemm_gpu/quantize_utils.py
--rw-r--r--  2.0 unx     6947 b- defN 24-Apr-25 12:54 fbgemm_gpu/runtime_monitor.py
--rw-r--r--  2.0 unx    20486 b- defN 24-Apr-25 12:54 fbgemm_gpu/sparse_ops.py
--rw-r--r--  2.0 unx     5774 b- defN 24-Apr-25 12:54 fbgemm_gpu/split_embedding_configs.py
--rw-r--r--  2.0 unx     7058 b- defN 24-Apr-25 12:54 fbgemm_gpu/split_embedding_inference_converter.py
--rw-r--r--  2.0 unx      540 b- defN 24-Apr-25 12:54 fbgemm_gpu/split_embedding_optimizer_ops.py
--rw-r--r--  2.0 unx    26853 b- defN 24-Apr-25 12:54 fbgemm_gpu/split_embedding_utils.py
--rw-r--r--  2.0 unx     2339 b- defN 24-Apr-25 12:54 fbgemm_gpu/split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx     3493 b- defN 24-Apr-25 12:54 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
--rw-r--r--  2.0 unx    66800 b- defN 24-Apr-25 12:54 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
--rw-r--r--  2.0 unx    98158 b- defN 24-Apr-25 12:54 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
--rw-r--r--  2.0 unx    40680 b- defN 24-Apr-25 12:54 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx      925 b- defN 24-Apr-25 12:54 fbgemm_gpu/uvm.py
--rw-r--r--  2.0 unx      383 b- defN 24-Apr-25 12:54 fbgemm_gpu/docs/__init__.py
--rw-r--r--  2.0 unx      273 b- defN 24-Apr-25 12:54 fbgemm_gpu/docs/common.py
--rw-r--r--  2.0 unx     2377 b- defN 24-Apr-25 12:54 fbgemm_gpu/docs/examples.py
--rw-r--r--  2.0 unx     7381 b- defN 24-Apr-25 12:54 fbgemm_gpu/docs/jagged_tensor_ops.py
--rw-r--r--  2.0 unx     7708 b- defN 24-Apr-25 12:54 fbgemm_gpu/docs/table_batched_embedding_ops.py
--rw-r--r--  2.0 unx      264 b- defN 24-Apr-25 12:54 fbgemm_gpu/docs/version.py
--rw-r--r--  2.0 unx      869 b- defN 24-Apr-25 12:49 fbgemm_gpu/experimental/example/__init__.py
--rwxr-xr-x  2.0 unx    30688 b- defN 24-Apr-25 12:54 fbgemm_gpu/experimental/example/fbgemm_gpu_experimental_example_py.so
--rw-r--r--  2.0 unx      381 b- defN 24-Apr-25 12:49 fbgemm_gpu/experimental/example/utils.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
--rw-r--r--  2.0 unx     4180 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
--rw-r--r--  2.0 unx     4180 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py
--rw-r--r--  2.0 unx     3395 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
--rw-r--r--  2.0 unx     3395 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py
--rw-r--r--  2.0 unx     2147 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
--rw-r--r--  2.0 unx     3395 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
--rw-r--r--  2.0 unx     3395 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb_pt2.py
--rw-r--r--  2.0 unx     3144 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
--rw-r--r--  2.0 unx     3144 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd_pt2.py
--rw-r--r--  2.0 unx     2420 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
--rw-r--r--  2.0 unx     2420 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none_pt2.py
--rw-r--r--  2.0 unx     3100 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
--rw-r--r--  2.0 unx     3100 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam_pt2.py
--rw-r--r--  2.0 unx     3100 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
--rw-r--r--  2.0 unx     3100 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb_pt2.py
--rw-r--r--  2.0 unx     4512 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
--rw-r--r--  2.0 unx     4512 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py
--rw-r--r--  2.0 unx     3964 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     3964 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py
--rw-r--r--  2.0 unx     3762 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
--rw-r--r--  2.0 unx     3762 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py
--rw-r--r--  2.0 unx      649 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
--rw-r--r--  2.0 unx     6162 b- defN 24-Apr-25 12:52 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
--rw-r--r--  2.0 unx     2602 b- defN 24-Apr-25 12:54 fbgemm_gpu_nightly_cpu-2024.4.25.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 24-Apr-25 12:54 fbgemm_gpu_nightly_cpu-2024.4.25.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-25 12:54 fbgemm_gpu_nightly_cpu-2024.4.25.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6344 b- defN 24-Apr-25 12:54 fbgemm_gpu_nightly_cpu-2024.4.25.dist-info/RECORD
-58 files, 11294106 bytes uncompressed, 3138825 bytes compressed:  72.2%
+Zip file size: 3149446 bytes, number of entries: 58
+-rw-r--r--  2.0 unx      914 b- defN 24-Apr-26 12:57 fbgemm_gpu/__init__.py
+-rw-r--r--  2.0 unx     3079 b- defN 24-Apr-26 12:57 fbgemm_gpu/batched_unary_embeddings_ops.py
+-rw-r--r--  2.0 unx      789 b- defN 24-Apr-26 12:57 fbgemm_gpu/enums.py
+-rwxr-xr-x  2.0 unx 10846712 b- defN 24-Apr-26 12:57 fbgemm_gpu/fbgemm_gpu_py.so
+-rw-r--r--  2.0 unx     5663 b- defN 24-Apr-26 12:57 fbgemm_gpu/metrics.py
+-rw-r--r--  2.0 unx     2362 b- defN 24-Apr-26 12:57 fbgemm_gpu/permute_pooled_embedding_modules.py
+-rw-r--r--  2.0 unx     2752 b- defN 24-Apr-26 12:57 fbgemm_gpu/permute_pooled_embedding_modules_split.py
+-rw-r--r--  2.0 unx     7885 b- defN 24-Apr-26 12:57 fbgemm_gpu/quantize_comm.py
+-rw-r--r--  2.0 unx     4143 b- defN 24-Apr-26 12:57 fbgemm_gpu/quantize_utils.py
+-rw-r--r--  2.0 unx     6947 b- defN 24-Apr-26 12:57 fbgemm_gpu/runtime_monitor.py
+-rw-r--r--  2.0 unx    20486 b- defN 24-Apr-26 12:57 fbgemm_gpu/sparse_ops.py
+-rw-r--r--  2.0 unx     5774 b- defN 24-Apr-26 12:57 fbgemm_gpu/split_embedding_configs.py
+-rw-r--r--  2.0 unx     7058 b- defN 24-Apr-26 12:57 fbgemm_gpu/split_embedding_inference_converter.py
+-rw-r--r--  2.0 unx      540 b- defN 24-Apr-26 12:57 fbgemm_gpu/split_embedding_optimizer_ops.py
+-rw-r--r--  2.0 unx    26853 b- defN 24-Apr-26 12:57 fbgemm_gpu/split_embedding_utils.py
+-rw-r--r--  2.0 unx     2339 b- defN 24-Apr-26 12:57 fbgemm_gpu/split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx     3493 b- defN 24-Apr-26 12:57 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
+-rw-r--r--  2.0 unx    66800 b- defN 24-Apr-26 12:57 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
+-rw-r--r--  2.0 unx    98158 b- defN 24-Apr-26 12:57 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
+-rw-r--r--  2.0 unx    40680 b- defN 24-Apr-26 12:57 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx      925 b- defN 24-Apr-26 12:57 fbgemm_gpu/uvm.py
+-rw-r--r--  2.0 unx      383 b- defN 24-Apr-26 12:57 fbgemm_gpu/docs/__init__.py
+-rw-r--r--  2.0 unx      273 b- defN 24-Apr-26 12:57 fbgemm_gpu/docs/common.py
+-rw-r--r--  2.0 unx     2377 b- defN 24-Apr-26 12:57 fbgemm_gpu/docs/examples.py
+-rw-r--r--  2.0 unx     7381 b- defN 24-Apr-26 12:57 fbgemm_gpu/docs/jagged_tensor_ops.py
+-rw-r--r--  2.0 unx     7708 b- defN 24-Apr-26 12:57 fbgemm_gpu/docs/table_batched_embedding_ops.py
+-rw-r--r--  2.0 unx      264 b- defN 24-Apr-26 12:57 fbgemm_gpu/docs/version.py
+-rw-r--r--  2.0 unx      869 b- defN 24-Apr-26 12:52 fbgemm_gpu/experimental/example/__init__.py
+-rwxr-xr-x  2.0 unx    30688 b- defN 24-Apr-26 12:57 fbgemm_gpu/experimental/example/fbgemm_gpu_experimental_example_py.so
+-rw-r--r--  2.0 unx      381 b- defN 24-Apr-26 12:52 fbgemm_gpu/experimental/example/utils.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
+-rw-r--r--  2.0 unx     4180 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
+-rw-r--r--  2.0 unx     4180 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py
+-rw-r--r--  2.0 unx     2147 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb_pt2.py
+-rw-r--r--  2.0 unx     3144 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
+-rw-r--r--  2.0 unx     3144 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd_pt2.py
+-rw-r--r--  2.0 unx     2420 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
+-rw-r--r--  2.0 unx     2420 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none_pt2.py
+-rw-r--r--  2.0 unx     3100 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
+-rw-r--r--  2.0 unx     3100 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam_pt2.py
+-rw-r--r--  2.0 unx     3100 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
+-rw-r--r--  2.0 unx     3100 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb_pt2.py
+-rw-r--r--  2.0 unx     4512 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     4512 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py
+-rw-r--r--  2.0 unx     3964 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     3964 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py
+-rw-r--r--  2.0 unx     3762 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
+-rw-r--r--  2.0 unx     3762 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py
+-rw-r--r--  2.0 unx      649 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
+-rw-r--r--  2.0 unx     6162 b- defN 24-Apr-26 12:55 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     2602 b- defN 24-Apr-26 12:57 fbgemm_gpu_nightly_cpu-2024.4.26.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 24-Apr-26 12:57 fbgemm_gpu_nightly_cpu-2024.4.26.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-26 12:57 fbgemm_gpu_nightly_cpu-2024.4.26.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6344 b- defN 24-Apr-26 12:57 fbgemm_gpu_nightly_cpu-2024.4.26.dist-info/RECORD
+58 files, 11294106 bytes uncompressed, 3138826 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -156,20 +156,20 @@
 
 Filename: fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
 Comment: 
 
 Filename: fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.4.25.dist-info/METADATA
+Filename: fbgemm_gpu_nightly_cpu-2024.4.26.dist-info/METADATA
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.4.25.dist-info/WHEEL
+Filename: fbgemm_gpu_nightly_cpu-2024.4.26.dist-info/WHEEL
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.4.25.dist-info/top_level.txt
+Filename: fbgemm_gpu_nightly_cpu-2024.4.26.dist-info/top_level.txt
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.4.25.dist-info/RECORD
+Filename: fbgemm_gpu_nightly_cpu-2024.4.26.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fbgemm_gpu/fbgemm_gpu_py.so

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -1630511,15 +1630511,15 @@
 	js     8c1b90 <int_nbit_split_embedding_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0xe60>
 	cmpq   $0x0,0x8(%r13)
 	jle    8c1bb0 <int_nbit_split_embedding_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0xe80>
 	call   1b6df0 <at::detail::getCUDAHooks()@plt>
 	mov    0x18fd99(%rip),%rbx        
 	mov    %rax,%rdi
 	mov    (%rax),%rax
-	mov    0x60(%rax),%rax
+	mov    0x38(%rax),%rax
 	cmp    %rbx,%rax
 	jne    8c17f8 <int_nbit_split_embedding_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0xac8>
 	movb   $0x0,-0x634(%rbp)
 	mov    -0x620(%rbp),%rax
 	mov    0x18f099(%rip),%rcx        
 	mov    %rcx,(%rax)
 	cmp    $0x2,%r14b
@@ -1630873,22 +1630873,22 @@
 	call   *%rax
 	test   %al,%al
 	je     8c113a <int_nbit_split_embedding_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0x40a>
 	call   1b6e20 <at::globalContext()@plt>
 	call   1b6df0 <at::detail::getCUDAHooks()@plt>
 	mov    %rax,%rdi
 	mov    (%rax),%rax
-	mov    0x60(%rax),%rax
+	mov    0x38(%rax),%rax
 	cmp    %rbx,%rax
 	jne    8c2088 <int_nbit_split_embedding_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0x1358>
 	call   1b6e20 <at::globalContext()@plt>
 	call   1b6df0 <at::detail::getCUDAHooks()@plt>
 	mov    %rax,%rdi
 	mov    (%rax),%rax
-	mov    0x60(%rax),%rax
+	mov    0x38(%rax),%rax
 	cmp    %rbx,%rax
 	jne    8c2050 <int_nbit_split_embedding_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0x1320>
 	call   1b6e20 <at::globalContext()@plt>
 	call   1b5e50 <at::detail::getHIPHooks()@plt>
 	mov    %rax,%rdi
 	mov    (%rax),%rax
 	mov    0x20(%rax),%rax
@@ -1631266,15 +1631266,15 @@
 	call   *%rax
 	test   %al,%al
 	je     8c183c <int_nbit_split_embedding_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0xb0c>
 	call   1b6df0 <at::detail::getCUDAHooks()@plt>
 	movb   $0x0,-0x634(%rbp)
 	mov    %rax,%rdi
 	mov    (%rax),%rax
-	mov    0x120(%rax),%rax
+	mov    0xf8(%rax),%rax
 	cmp    0x19023e(%rip),%rax        
 	je     8c1141 <int_nbit_split_embedding_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0x411>
 	jmp    8c188a <int_nbit_split_embedding_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0xb5a>
 	nopl   (%rax)
 	call   *%rax
 	test   %al,%al
 	je     8c181f <int_nbit_split_embedding_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0xaef>
@@ -1632481,15 +1632481,15 @@
 	js     8c42b0 <int_nbit_split_embedding_nobag_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0xdd0>
 	cmpq   $0x0,(%rbx)
 	jle    8c42e0 <int_nbit_split_embedding_nobag_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0xe00>
 	call   1b6df0 <at::detail::getCUDAHooks()@plt>
 	mov    0x18d5f7(%rip),%r12        
 	mov    %rax,%rdi
 	mov    (%rax),%rax
-	mov    0x60(%rax),%rax
+	mov    0x38(%rax),%rax
 	cmp    %r12,%rax
 	jne    8c3f70 <int_nbit_split_embedding_nobag_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0xa90>
 	movb   $0x0,-0x6d0(%rbp)
 	mov    -0x6b8(%rbp),%rax
 	mov    0x18c8f7(%rip),%rsi        
 	mov    %rsi,(%rax)
 	cmp    $0x2,%r15b
@@ -1632830,22 +1632830,22 @@
 	call   *%rax
 	test   %al,%al
 	je     8c38dc <int_nbit_split_embedding_nobag_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0x3fc>
 	call   1b6e20 <at::globalContext()@plt>
 	call   1b6df0 <at::detail::getCUDAHooks()@plt>
 	mov    %rax,%rdi
 	mov    (%rax),%rax
-	mov    0x60(%rax),%rax
+	mov    0x38(%rax),%rax
 	cmp    %r12,%rax
 	jne    8c47b8 <int_nbit_split_embedding_nobag_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0x12d8>
 	call   1b6e20 <at::globalContext()@plt>
 	call   1b6df0 <at::detail::getCUDAHooks()@plt>
 	mov    %rax,%rdi
 	mov    (%rax),%rax
-	mov    0x60(%rax),%rax
+	mov    0x38(%rax),%rax
 	cmp    %r12,%rax
 	jne    8c4780 <int_nbit_split_embedding_nobag_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0x12a0>
 	call   1b6e20 <at::globalContext()@plt>
 	call   1b5e50 <at::detail::getHIPHooks()@plt>
 	mov    %rax,%rdi
 	mov    (%rax),%rax
 	mov    0x20(%rax),%rax
@@ -1633212,15 +1633212,15 @@
 	call   *%rax
 	test   %al,%al
 	je     8c3fb4 <int_nbit_split_embedding_nobag_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0xad4>
 	call   1b6df0 <at::detail::getCUDAHooks()@plt>
 	movb   $0x0,-0x6d0(%rbp)
 	mov    %rax,%rdi
 	mov    (%rax),%rax
-	mov    0x120(%rax),%rax
+	mov    0xf8(%rax),%rax
 	cmp    0x18db0e(%rip),%rax        
 	je     8c38e3 <int_nbit_split_embedding_nobag_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0x403>
 	jmp    8c4002 <int_nbit_split_embedding_nobag_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0xb22>
 	nopl   (%rax)
 	call   *%rax
 	test   %al,%al
 	je     8c3f97 <int_nbit_split_embedding_nobag_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0xab7>
@@ -1646865,15 +1646865,15 @@
 	js     8d51a0 <int_nbit_split_embedding_codegen_forward_weighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, at::Tensor, long, long, long)@@Base+0x2240>
 	cmpq   $0x0,0x8(%rbx)
 	jle    8d5220 <int_nbit_split_embedding_codegen_forward_weighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, at::Tensor, long, long, long)@@Base+0x22c0>
 	call   1b6df0 <at::detail::getCUDAHooks()@plt>
 	mov    0x17cd3f(%rip),%r13        
 	mov    %rax,%rdi
 	mov    (%rax),%rax
-	mov    0x60(%rax),%rax
+	mov    0x38(%rax),%rax
 	cmp    %r13,%rax
 	jne    8d4ca0 <int_nbit_split_embedding_codegen_forward_weighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, at::Tensor, long, long, long)@@Base+0x1d40>
 	movb   $0x0,-0x220(%rbp)
 	mov    -0x208(%rbp),%rax
 	mov    0x17c03f(%rip),%rcx        
 	mov    %rcx,(%rax)
 	cmp    $0x2,%r15b
@@ -1647417,22 +1647417,22 @@
 	call   *%rax
 	test   %al,%al
 	je     8d4194 <int_nbit_split_embedding_codegen_forward_weighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, at::Tensor, long, long, long)@@Base+0x1234>
 	call   1b6e20 <at::globalContext()@plt>
 	call   1b6df0 <at::detail::getCUDAHooks()@plt>
 	mov    %rax,%rdi
 	mov    (%rax),%rax
-	mov    0x60(%rax),%rax
+	mov    0x38(%rax),%rax
 	cmp    %r13,%rax
 	jne    8d5458 <int_nbit_split_embedding_codegen_forward_weighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, at::Tensor, long, long, long)@@Base+0x24f8>
 	call   1b6e20 <at::globalContext()@plt>
 	call   1b6df0 <at::detail::getCUDAHooks()@plt>
 	mov    %rax,%rdi
 	mov    (%rax),%rax
-	mov    0x60(%rax),%rax
+	mov    0x38(%rax),%rax
 	cmp    %r13,%rax
 	jne    8d5420 <int_nbit_split_embedding_codegen_forward_weighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, at::Tensor, long, long, long)@@Base+0x24c0>
 	call   1b6e20 <at::globalContext()@plt>
 	call   1b5e50 <at::detail::getHIPHooks()@plt>
 	mov    %rax,%rdi
 	mov    (%rax),%rax
 	mov    0x20(%rax),%rax
@@ -1647801,15 +1647801,15 @@
 	call   *%rax
 	test   %al,%al
 	je     8d4ce4 <int_nbit_split_embedding_codegen_forward_weighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, at::Tensor, long, long, long)@@Base+0x1d84>
 	call   1b6df0 <at::detail::getCUDAHooks()@plt>
 	movb   $0x0,-0x220(%rbp)
 	mov    %rax,%rdi
 	mov    (%rax),%rax
-	mov    0x120(%rax),%rax
+	mov    0xf8(%rax),%rax
 	cmp    0x17ce6e(%rip),%rax        
 	je     8d419b <int_nbit_split_embedding_codegen_forward_weighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, at::Tensor, long, long, long)@@Base+0x123b>
 	jmp    8d4d32 <int_nbit_split_embedding_codegen_forward_weighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, at::Tensor, long, long, long)@@Base+0x1dd2>
 	nopl   (%rax)
 	call   *%rax
 	test   %al,%al
 	je     8d4cc7 <int_nbit_split_embedding_codegen_forward_weighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, at::Tensor, long, long, long)@@Base+0x1d67>
```

## fbgemm_gpu/docs/version.py

```diff
@@ -2,8 +2,8 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-__version__: str = "2024.4.25"
+__version__: str = "2024.4.26"
```

## Comparing `fbgemm_gpu_nightly_cpu-2024.4.25.dist-info/METADATA` & `fbgemm_gpu_nightly_cpu-2024.4.26.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbgemm-gpu-nightly-cpu
-Version: 2024.4.25
+Version: 2024.4.26
 Home-page: https://github.com/pytorch/fbgemm
 Author: FBGEMM Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: PyTorch,Recommendation Models,High Performance Computing,GPU,CUDA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `fbgemm_gpu_nightly_cpu-2024.4.25.dist-info/RECORD` & `fbgemm_gpu_nightly_cpu-2024.4.26.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 fbgemm_gpu/__init__.py,sha256=ZPy0iaSSHb6-eT6lz8MSpr-5Ircj9SLmVpL0o0ejcNQ,914
 fbgemm_gpu/batched_unary_embeddings_ops.py,sha256=dpxZAueNsadJVuK7Dwo8GbOlho9r67Lfh8kesqRKJNI,3079
 fbgemm_gpu/enums.py,sha256=GVuzF5cFTLzttkvlH1SdcGrxrppMhDSbQj_Vm_4zmEo,789
-fbgemm_gpu/fbgemm_gpu_py.so,sha256=UpMRhj5Fad9jbBC12Yq4abWv1LbiwlyVPmTDFSpdBA4,10846712
+fbgemm_gpu/fbgemm_gpu_py.so,sha256=MkpJPVtnjMqFWMI8mnHGI3mbQIJYY-YZBVWETXOfOxY,10846712
 fbgemm_gpu/metrics.py,sha256=TsurFLJf0nJvPDN7urWb4LMQlf5RgdWPTTTDO7S4wtI,5663
 fbgemm_gpu/permute_pooled_embedding_modules.py,sha256=4mHJ2fo3SeG25iSwdm2YsM8q_oWsF1LxRguYmxSnuDI,2362
 fbgemm_gpu/permute_pooled_embedding_modules_split.py,sha256=cUrEbRIvLFW_3Zmh07QkN4S1Cfvvge6TYO1VXBFCpz8,2752
 fbgemm_gpu/quantize_comm.py,sha256=UZcVSC2JQ0oSkwsJQnjaZ2k8mm2p3hvVzpyg7X5xFXM,7885
 fbgemm_gpu/quantize_utils.py,sha256=-vwHIEkyStDo1TWoYfwmC5U6DvR6iRMHXyjFc9lO_p8,4143
 fbgemm_gpu/runtime_monitor.py,sha256=tIdxkJIWkJ8705btxs9NqzEXC7QprFh3sA8Q4LpvtJ8,6947
 fbgemm_gpu/sparse_ops.py,sha256=_yq67rG4sabvW5maMiM5IAucMhMWFXM99ABU7es2cm4,20486
@@ -20,15 +20,15 @@
 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py,sha256=S6qWfFzpqNIB8l9N3LAsYfaXSExg53f_b3fl47d1b1U,40680
 fbgemm_gpu/uvm.py,sha256=-cZunsuvnAKUEQptIwdYVar_3hUE99FbQUsyfBVeXPE,925
 fbgemm_gpu/docs/__init__.py,sha256=BbAfYbNZsBhO7L5Am4wyBLet4mTY2aXFucyGTxF9IlI,383
 fbgemm_gpu/docs/common.py,sha256=8ipXTwVb222X-aZ71O6n8fhxHCHPNhJEHMFiO7epcIs,273
 fbgemm_gpu/docs/examples.py,sha256=ZMN_6sL74LH_hrp2bF_hmg8gi29GhcgvwV3kCMjxkoE,2377
 fbgemm_gpu/docs/jagged_tensor_ops.py,sha256=Bsx-ZxvvdMv5CaldSvuw9GPR-HRcLbRR2IEXCOCm9r0,7381
 fbgemm_gpu/docs/table_batched_embedding_ops.py,sha256=h_EQOIMsdVlr-Pygul-fDGxx7JqLRjaBMI_z0PFrGAE,7708
-fbgemm_gpu/docs/version.py,sha256=4O_r24yq5FKgUoXIGPZbwwjKUa42qaGlSW4cuVhus_0,264
+fbgemm_gpu/docs/version.py,sha256=N7AIDmlepv3pKU7O_1d58W92UKJv5TqaobemNrtBNFk,264
 fbgemm_gpu/experimental/example/__init__.py,sha256=aGZXCUV-oXSrbESJnfRuI683DuLAIjFM-HmIWgwmCnw,869
 fbgemm_gpu/experimental/example/fbgemm_gpu_experimental_example_py.so,sha256=OM6Wogd4Ux-UqYPaW71uDCCkrH4ATBSXmvyIw1TvuMY,30688
 fbgemm_gpu/experimental/example/utils.py,sha256=nj4R0e58k3RR-XwMBowveLfC_sSYYYmocrJ2Wuf67uM,381
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py,sha256=lfob_IDNeAs2FjS2WCldKlw0gm_qUZdp043fngI8sGE,1466
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py,sha256=x17z36WrjIloP-pLVzyxpxjats7XjxJZv8OysT9JxD4,4180
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py,sha256=x17z36WrjIloP-pLVzyxpxjats7XjxJZv8OysT9JxD4,4180
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py,sha256=EBR6BEDV_SOuJM_yGq4IEfdL8umYkAmCWekcAwpHpNQ,3395
@@ -48,11 +48,11 @@
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py,sha256=Aljkdf4GB0zetL2j5YIhTZaOqiIMIlQ9iTDM421lbiM,4512
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py,sha256=Qr3xtASUsgNbPJD46__jyKkR3xy0n-n2IZSa5QPD-NA,3964
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py,sha256=Qr3xtASUsgNbPJD46__jyKkR3xy0n-n2IZSa5QPD-NA,3964
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py,sha256=fOgbq-u3VtbtKFqLTGQJiCwoHpa_xP-rBIvj98S78F4,3762
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py,sha256=fOgbq-u3VtbtKFqLTGQJiCwoHpa_xP-rBIvj98S78F4,3762
 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py,sha256=yiD3_bG5yT5VXLoGw4eeRKQ2Nj087DRq0qKCVPb52SY,649
 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py,sha256=OFw5PM2YDiKvr6T9ZW7BKiq58gB7txcKfuJkBUROxdI,6162
-fbgemm_gpu_nightly_cpu-2024.4.25.dist-info/METADATA,sha256=FWH-NnyPZaFm80bgiERsIUxVB2nw4gGDAg7HIB7zz14,2602
-fbgemm_gpu_nightly_cpu-2024.4.25.dist-info/WHEEL,sha256=AdAOsf8BL1uIBxiEcIdcPDjJWWb0G5USb4X4msVaesE,105
-fbgemm_gpu_nightly_cpu-2024.4.25.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
-fbgemm_gpu_nightly_cpu-2024.4.25.dist-info/RECORD,,
+fbgemm_gpu_nightly_cpu-2024.4.26.dist-info/METADATA,sha256=t-arsRDMW6ujHyegxFnXOj3nyeP7rDYL1A9W98MllDM,2602
+fbgemm_gpu_nightly_cpu-2024.4.26.dist-info/WHEEL,sha256=AdAOsf8BL1uIBxiEcIdcPDjJWWb0G5USb4X4msVaesE,105
+fbgemm_gpu_nightly_cpu-2024.4.26.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
+fbgemm_gpu_nightly_cpu-2024.4.26.dist-info/RECORD,,
```

