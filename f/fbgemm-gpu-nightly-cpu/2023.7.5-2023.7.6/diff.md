# Comparing `tmp/fbgemm_gpu_nightly_cpu-2023.7.5-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/fbgemm_gpu_nightly_cpu-2023.7.6-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,43 +1,43 @@
 Zip file size: 3198123 bytes, number of entries: 41
--rw-r--r--  2.0 unx      567 b- defN 23-Jul-05 13:03 fbgemm_gpu/__init__.py
--rw-r--r--  2.0 unx    14920 b- defN 23-Jul-05 13:03 fbgemm_gpu/_fbgemm_gpu_docs.py
--rw-r--r--  2.0 unx     2747 b- defN 23-Jul-05 13:03 fbgemm_gpu/batched_unary_embeddings_ops.py
--rw-r--r--  2.0 unx      818 b- defN 23-Jul-05 13:03 fbgemm_gpu/enums.py
--rwxr-xr-x  2.0 unx 10709064 b- defN 23-Jul-05 13:03 fbgemm_gpu/fbgemm_gpu_py.so
--rw-r--r--  2.0 unx     5648 b- defN 23-Jul-05 13:03 fbgemm_gpu/metrics.py
--rw-r--r--  2.0 unx     2339 b- defN 23-Jul-05 13:03 fbgemm_gpu/permute_pooled_embedding_modules.py
--rw-r--r--  2.0 unx     2737 b- defN 23-Jul-05 13:03 fbgemm_gpu/permute_pooled_embedding_modules_split.py
--rw-r--r--  2.0 unx     7682 b- defN 23-Jul-05 13:03 fbgemm_gpu/quantize_comm.py
--rw-r--r--  2.0 unx     4005 b- defN 23-Jul-05 13:03 fbgemm_gpu/quantize_utils.py
--rw-r--r--  2.0 unx     5745 b- defN 23-Jul-05 13:03 fbgemm_gpu/split_embedding_configs.py
--rw-r--r--  2.0 unx     6661 b- defN 23-Jul-05 13:03 fbgemm_gpu/split_embedding_inference_converter.py
--rw-r--r--  2.0 unx      525 b- defN 23-Jul-05 13:03 fbgemm_gpu/split_embedding_optimizer_ops.py
--rw-r--r--  2.0 unx    19751 b- defN 23-Jul-05 13:03 fbgemm_gpu/split_embedding_utils.py
--rw-r--r--  2.0 unx     2170 b- defN 23-Jul-05 13:03 fbgemm_gpu/split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx     3433 b- defN 23-Jul-05 13:03 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
--rw-r--r--  2.0 unx    61087 b- defN 23-Jul-05 13:03 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
--rw-r--r--  2.0 unx    80868 b- defN 23-Jul-05 13:03 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
--rw-r--r--  2.0 unx    39550 b- defN 23-Jul-05 13:03 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx      910 b- defN 23-Jul-05 13:03 fbgemm_gpu/uvm.py
--rw-r--r--  2.0 unx     1603 b- defN 23-Jul-05 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
--rw-r--r--  2.0 unx     4717 b- defN 23-Jul-05 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
--rw-r--r--  2.0 unx     3354 b- defN 23-Jul-05 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
--rw-r--r--  2.0 unx     3112 b- defN 23-Jul-05 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_weight_decay.py
--rw-r--r--  2.0 unx     1906 b- defN 23-Jul-05 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
--rw-r--r--  2.0 unx     3354 b- defN 23-Jul-05 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
--rw-r--r--  2.0 unx     3062 b- defN 23-Jul-05 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
--rw-r--r--  2.0 unx     2617 b- defN 23-Jul-05 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
--rw-r--r--  2.0 unx     3370 b- defN 23-Jul-05 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
--rw-r--r--  2.0 unx     3370 b- defN 23-Jul-05 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
--rw-r--r--  2.0 unx     5005 b- defN 23-Jul-05 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
--rw-r--r--  2.0 unx     7014 b- defN 23-Jul-05 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     3105 b- defN 23-Jul-05 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py
--rw-r--r--  2.0 unx     4961 b- defN 23-Jul-05 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
--rw-r--r--  2.0 unx     4250 b- defN 23-Jul-05 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
--rw-r--r--  2.0 unx      635 b- defN 23-Jul-05 12:57 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
--rw-r--r--  2.0 unx     6136 b- defN 23-Jul-05 13:01 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
--rw-r--r--  2.0 unx     2933 b- defN 23-Jul-05 13:03 fbgemm_gpu_nightly_cpu-2023.7.5.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 23-Jul-05 13:03 fbgemm_gpu_nightly_cpu-2023.7.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-05 13:03 fbgemm_gpu_nightly_cpu-2023.7.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4530 b- defN 23-Jul-05 13:03 fbgemm_gpu_nightly_cpu-2023.7.5.dist-info/RECORD
-41 files, 11040377 bytes uncompressed, 3190493 bytes compressed:  71.1%
+-rw-r--r--  2.0 unx      567 b- defN 23-Jul-06 13:03 fbgemm_gpu/__init__.py
+-rw-r--r--  2.0 unx    14920 b- defN 23-Jul-06 13:03 fbgemm_gpu/_fbgemm_gpu_docs.py
+-rw-r--r--  2.0 unx     2747 b- defN 23-Jul-06 13:03 fbgemm_gpu/batched_unary_embeddings_ops.py
+-rw-r--r--  2.0 unx      818 b- defN 23-Jul-06 13:03 fbgemm_gpu/enums.py
+-rwxr-xr-x  2.0 unx 10709064 b- defN 23-Jul-06 13:03 fbgemm_gpu/fbgemm_gpu_py.so
+-rw-r--r--  2.0 unx     5648 b- defN 23-Jul-06 13:03 fbgemm_gpu/metrics.py
+-rw-r--r--  2.0 unx     2339 b- defN 23-Jul-06 13:03 fbgemm_gpu/permute_pooled_embedding_modules.py
+-rw-r--r--  2.0 unx     2737 b- defN 23-Jul-06 13:03 fbgemm_gpu/permute_pooled_embedding_modules_split.py
+-rw-r--r--  2.0 unx     7682 b- defN 23-Jul-06 13:03 fbgemm_gpu/quantize_comm.py
+-rw-r--r--  2.0 unx     4005 b- defN 23-Jul-06 13:03 fbgemm_gpu/quantize_utils.py
+-rw-r--r--  2.0 unx     5745 b- defN 23-Jul-06 13:03 fbgemm_gpu/split_embedding_configs.py
+-rw-r--r--  2.0 unx     6661 b- defN 23-Jul-06 13:03 fbgemm_gpu/split_embedding_inference_converter.py
+-rw-r--r--  2.0 unx      525 b- defN 23-Jul-06 13:03 fbgemm_gpu/split_embedding_optimizer_ops.py
+-rw-r--r--  2.0 unx    19751 b- defN 23-Jul-06 13:03 fbgemm_gpu/split_embedding_utils.py
+-rw-r--r--  2.0 unx     2170 b- defN 23-Jul-06 13:03 fbgemm_gpu/split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx     3433 b- defN 23-Jul-06 13:03 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
+-rw-r--r--  2.0 unx    61087 b- defN 23-Jul-06 13:03 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
+-rw-r--r--  2.0 unx    80872 b- defN 23-Jul-06 13:03 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
+-rw-r--r--  2.0 unx    39550 b- defN 23-Jul-06 13:03 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx      910 b- defN 23-Jul-06 13:03 fbgemm_gpu/uvm.py
+-rw-r--r--  2.0 unx     1603 b- defN 23-Jul-06 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
+-rw-r--r--  2.0 unx     4717 b- defN 23-Jul-06 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
+-rw-r--r--  2.0 unx     3354 b- defN 23-Jul-06 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
+-rw-r--r--  2.0 unx     3112 b- defN 23-Jul-06 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_weight_decay.py
+-rw-r--r--  2.0 unx     1906 b- defN 23-Jul-06 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
+-rw-r--r--  2.0 unx     3354 b- defN 23-Jul-06 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
+-rw-r--r--  2.0 unx     3062 b- defN 23-Jul-06 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
+-rw-r--r--  2.0 unx     2617 b- defN 23-Jul-06 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
+-rw-r--r--  2.0 unx     3370 b- defN 23-Jul-06 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
+-rw-r--r--  2.0 unx     3370 b- defN 23-Jul-06 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
+-rw-r--r--  2.0 unx     5005 b- defN 23-Jul-06 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     7014 b- defN 23-Jul-06 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     3105 b- defN 23-Jul-06 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py
+-rw-r--r--  2.0 unx     4961 b- defN 23-Jul-06 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
+-rw-r--r--  2.0 unx     4250 b- defN 23-Jul-06 13:01 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
+-rw-r--r--  2.0 unx      635 b- defN 23-Jul-06 12:57 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
+-rw-r--r--  2.0 unx     6136 b- defN 23-Jul-06 13:01 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     2933 b- defN 23-Jul-06 13:03 fbgemm_gpu_nightly_cpu-2023.7.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 23-Jul-06 13:03 fbgemm_gpu_nightly_cpu-2023.7.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-06 13:03 fbgemm_gpu_nightly_cpu-2023.7.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4530 b- defN 23-Jul-06 13:03 fbgemm_gpu_nightly_cpu-2023.7.6.dist-info/RECORD
+41 files, 11040381 bytes uncompressed, 3190493 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -105,20 +105,20 @@
 
 Filename: fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
 Comment: 
 
 Filename: fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.7.5.dist-info/METADATA
+Filename: fbgemm_gpu_nightly_cpu-2023.7.6.dist-info/METADATA
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.7.5.dist-info/WHEEL
+Filename: fbgemm_gpu_nightly_cpu-2023.7.6.dist-info/WHEEL
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.7.5.dist-info/top_level.txt
+Filename: fbgemm_gpu_nightly_cpu-2023.7.6.dist-info/top_level.txt
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.7.5.dist-info/RECORD
+Filename: fbgemm_gpu_nightly_cpu-2023.7.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fbgemm_gpu/split_table_batched_embeddings_ops_training.py

```diff
@@ -428,15 +428,15 @@
 
         self.register_buffer(
             "D_offsets",
             torch.tensor(D_offsets, device=self.current_device, dtype=torch.int32),
         )
         hash_size_cumsum = [0] + list(accumulate(rows))
         self.total_hash_size: int = int(hash_size_cumsum[-1])
-        if hash_size_cumsum == 0:
+        if self.total_hash_size == 0:
             self.total_hash_size_bits: int = 0
         else:
             self.total_hash_size_bits: int = int(log2(float(self.total_hash_size)) + 1)
         # The last element is to easily access # of rows of each table by
         # hash_size_cumsum[t + 1] - hash_size_cumsum[t]
         hash_size_cumsum = [hash_size_cumsum[t] for t in self.feature_table_map] + [
             self.total_hash_size
```

## Comparing `fbgemm_gpu_nightly_cpu-2023.7.5.dist-info/METADATA` & `fbgemm_gpu_nightly_cpu-2023.7.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbgemm-gpu-nightly-cpu
-Version: 2023.7.5
+Version: 2023.7.6
 Home-page: https://github.com/pytorch/fbgemm
 Author: FBGEMM Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: PyTorch,Recommendation Models,High Performance Computing,GPU,CUDA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `fbgemm_gpu_nightly_cpu-2023.7.5.dist-info/RECORD` & `fbgemm_gpu_nightly_cpu-2023.7.6.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 fbgemm_gpu/split_embedding_configs.py,sha256=Y3fJLHh4ffO6v_iKGc2MbBQTu8yFIMExEG_VYNW7rzI,5745
 fbgemm_gpu/split_embedding_inference_converter.py,sha256=z1NugAsdcLO4nVFa_DJlOZHahmEdrBELi15ywFdaP3U,6661
 fbgemm_gpu/split_embedding_optimizer_ops.py,sha256=QrJ6qz5pzlojnj08te9opHCDjRPK_PnogL8mERXxlz8,525
 fbgemm_gpu/split_embedding_utils.py,sha256=CqK8zqBRMNp9D4xJWgZGR8mG1L5u4rdcXQMwV6sMTBs,19751
 fbgemm_gpu/split_table_batched_embeddings_ops.py,sha256=-MRQ-fyb9ySHuYaMnYoLZjPTBK-tcEEvQtK-EwZansg,2170
 fbgemm_gpu/split_table_batched_embeddings_ops_common.py,sha256=khzh06VsBtrmnfcxBRfSQ_4_eKTCSma7bjeP5TENHaY,3433
 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py,sha256=hZ7Y9ThJMxzhWaRtRnHQeuea_R0IT8lqSfMAkrKa0Bo,61087
-fbgemm_gpu/split_table_batched_embeddings_ops_training.py,sha256=joEtv-gCa9yoJtYFhKqdtLWuzPLzWqpuHBB6fThFheo,80868
+fbgemm_gpu/split_table_batched_embeddings_ops_training.py,sha256=ys2ckjXyDyofrY876P4Wys72R8Cd3gmUGaUBWcPdSAo,80872
 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py,sha256=PEyotgA2wKfUqvhcsw229VE5fn260treZjWSPdEmEnU,39550
 fbgemm_gpu/uvm.py,sha256=GproyMKA3fxW_bgaiEp3pduf7Q8Pj5Iv1_7OBVB_3to,910
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py,sha256=iN_8ecRtNU72t89OO-JtvRrIdQqMdOfdNF-zXK_RUSM,1603
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py,sha256=d20G6PLB0hJ9EEHzrhxbN8mn06JOpgKaHdEsJgHZCtQ,4717
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py,sha256=a3sRw9P4-iJHJTU9m6DwA8Pg9rxAKRcJN6ZWBkk3lo8,3354
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_weight_decay.py,sha256=IY8PwBueq_QzO7TXVp9Cl6tnIoFYivDTwa3GNyu08vk,3112
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py,sha256=5R-T38PIvVHh1WVHqU_RdbEOr8Q8FX2jMMnpZ1Ddysg,1906
@@ -31,11 +31,11 @@
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py,sha256=XRgP_N9mHwg5RLpDhtDIcogDHqY5Gw2C04QH4-W0Tk4,5005
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py,sha256=C69JVjrCdRnkCGZq_KYJ1WXuj24z4nPWCpsezICsoXI,7014
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py,sha256=OUATcloIxrOdnU_S0gcwiJbP95mtLX93hlYyqhNcdSc,3105
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py,sha256=UV7PGpsmOjbsPprmk3z-xTnkrEl4JkWl216o-V3T4YI,4961
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py,sha256=7E-kNXqHV4_P0Cl6Zq8cRpKZFaHMAtS6x8r4Yq1PLJo,4250
 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py,sha256=I6xnQ0vv6PZCxMsR87fWvb1Qtkp7ehx1b-9-La1vW2U,635
 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py,sha256=soARoBsdOnNNZdCIkVmryPHtKyhbcFLqHOTveG-hk6s,6136
-fbgemm_gpu_nightly_cpu-2023.7.5.dist-info/METADATA,sha256=3_0-cS-lr5ZCMxMsYIBepGqARO1ErXI8bzj6OGsjZak,2933
-fbgemm_gpu_nightly_cpu-2023.7.5.dist-info/WHEEL,sha256=uNTrmykJsfnOiRowEmEAgdbSsr7BScgAFZq1d9YxSqA,105
-fbgemm_gpu_nightly_cpu-2023.7.5.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
-fbgemm_gpu_nightly_cpu-2023.7.5.dist-info/RECORD,,
+fbgemm_gpu_nightly_cpu-2023.7.6.dist-info/METADATA,sha256=smZqxbTOckckUHafNoyW4GAUzY7CzubSwia5Dl43hZ4,2933
+fbgemm_gpu_nightly_cpu-2023.7.6.dist-info/WHEEL,sha256=uNTrmykJsfnOiRowEmEAgdbSsr7BScgAFZq1d9YxSqA,105
+fbgemm_gpu_nightly_cpu-2023.7.6.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
+fbgemm_gpu_nightly_cpu-2023.7.6.dist-info/RECORD,,
```

