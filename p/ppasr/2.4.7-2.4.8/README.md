# Comparing `tmp/ppasr-2.4.7-py3-none-any.whl.zip` & `tmp/ppasr-2.4.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 1648972 bytes, number of entries: 83
--rw-rw-rw-  2.0 fat      134 b- defN 24-Apr-27 06:48 ppasr/__init__.py
+Zip file size: 1649767 bytes, number of entries: 83
+-rw-rw-rw-  2.0 fat      134 b- defN 24-May-01 03:14 ppasr/__init__.py
 -rw-rw-rw-  2.0 fat    17895 b- defN 23-Jul-17 11:28 ppasr/predict.py
--rw-rw-rw-  2.0 fat    38580 b- defN 24-Apr-21 12:12 ppasr/trainer.py
+-rw-rw-rw-  2.0 fat    41804 b- defN 24-Apr-27 14:27 ppasr/trainer.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jul-12 12:38 ppasr/data_utils/__init__.py
 -rw-rw-rw-  2.0 fat    23844 b- defN 24-Apr-27 05:34 ppasr/data_utils/audio.py
 -rw-rw-rw-  2.0 fat     2377 b- defN 22-Oct-29 02:25 ppasr/data_utils/binary.py
 -rw-rw-rw-  2.0 fat     1584 b- defN 23-Apr-05 02:33 ppasr/data_utils/collate_fn.py
 -rw-rw-rw-  2.0 fat     5192 b- defN 23-Jan-30 11:56 ppasr/data_utils/normalizer.py
--rw-rw-rw-  2.0 fat     4244 b- defN 23-Jan-30 11:56 ppasr/data_utils/reader.py
+-rw-rw-rw-  2.0 fat     4565 b- defN 24-Apr-27 12:46 ppasr/data_utils/reader.py
 -rw-rw-rw-  2.0 fat     8477 b- defN 22-Aug-05 13:41 ppasr/data_utils/sampler.py
 -rw-rw-rw-  2.0 fat    15686 b- defN 23-Dec-08 11:32 ppasr/data_utils/utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jul-12 12:38 ppasr/data_utils/augmentor/__init__.py
 -rw-rw-rw-  2.0 fat     5787 b- defN 22-Nov-06 06:19 ppasr/data_utils/augmentor/augmentation.py
 -rw-rw-rw-  2.0 fat      965 b- defN 22-Jul-12 12:38 ppasr/data_utils/augmentor/base.py
 -rw-rw-rw-  2.0 fat     2570 b- defN 23-Apr-08 01:30 ppasr/data_utils/augmentor/noise_perturb.py
 -rw-rw-rw-  2.0 fat      977 b- defN 22-Sep-29 13:43 ppasr/data_utils/augmentor/resample.py
@@ -31,55 +31,55 @@
 -rw-rw-rw-  2.0 fat    11174 b- defN 23-Apr-01 04:48 ppasr/infer_utils/inference_predictor.py
 -rw-rw-rw-  2.0 fat     4696 b- defN 24-Feb-03 15:03 ppasr/infer_utils/pun_predictor.py
 -rw-rw-rw-  2.0 fat  1807522 b- defN 22-Oct-28 14:36 ppasr/infer_utils/silero_vad.onnx
 -rw-rw-rw-  2.0 fat     8614 b- defN 23-Jan-30 11:56 ppasr/infer_utils/vad_predictor.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jul-12 12:38 ppasr/model_utils/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-20 12:39 ppasr/model_utils/conformer/__init__.py
 -rw-rw-rw-  2.0 fat    12421 b- defN 23-Apr-01 02:49 ppasr/model_utils/conformer/attention.py
--rw-rw-rw-  2.0 fat     5829 b- defN 23-Feb-07 12:26 ppasr/model_utils/conformer/convolution.py
+-rw-rw-rw-  2.0 fat     5799 b- defN 24-Apr-29 14:50 ppasr/model_utils/conformer/convolution.py
 -rw-rw-rw-  2.0 fat     4738 b- defN 22-Nov-15 11:50 ppasr/model_utils/conformer/embedding.py
--rw-rw-rw-  2.0 fat    19705 b- defN 23-Jan-30 11:56 ppasr/model_utils/conformer/encoder.py
+-rw-rw-rw-  2.0 fat    19675 b- defN 24-Apr-29 14:50 ppasr/model_utils/conformer/encoder.py
 -rw-rw-rw-  2.0 fat     9338 b- defN 23-Jan-30 11:56 ppasr/model_utils/conformer/model.py
 -rw-rw-rw-  2.0 fat     1286 b- defN 22-Nov-16 04:10 ppasr/model_utils/conformer/positionwise.py
 -rw-rw-rw-  2.0 fat     8793 b- defN 22-Nov-16 04:10 ppasr/model_utils/conformer/subsampling.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jul-12 12:38 ppasr/model_utils/deepspeech2/__init__.py
 -rw-rw-rw-  2.0 fat      688 b- defN 22-Oct-20 12:39 ppasr/model_utils/deepspeech2/conv.py
 -rw-rw-rw-  2.0 fat     4644 b- defN 22-Oct-25 10:31 ppasr/model_utils/deepspeech2/encoder.py
 -rw-rw-rw-  2.0 fat     4329 b- defN 23-Jan-30 11:56 ppasr/model_utils/deepspeech2/model.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-30 11:56 ppasr/model_utils/efficient_conformer/__init__.py
 -rw-rw-rw-  2.0 fat     9054 b- defN 23-Apr-01 05:10 ppasr/model_utils/efficient_conformer/attention.py
--rw-rw-rw-  2.0 fat     5754 b- defN 23-Mar-10 14:43 ppasr/model_utils/efficient_conformer/convolution.py
--rw-rw-rw-  2.0 fat    25366 b- defN 23-Apr-01 04:48 ppasr/model_utils/efficient_conformer/encoder.py
+-rw-rw-rw-  2.0 fat     5724 b- defN 24-Apr-29 14:50 ppasr/model_utils/efficient_conformer/convolution.py
+-rw-rw-rw-  2.0 fat    25336 b- defN 24-Apr-29 14:50 ppasr/model_utils/efficient_conformer/encoder.py
 -rw-rw-rw-  2.0 fat     9409 b- defN 23-Apr-01 03:29 ppasr/model_utils/efficient_conformer/model.py
 -rw-rw-rw-  2.0 fat     2052 b- defN 23-Jan-30 11:56 ppasr/model_utils/efficient_conformer/subsampling.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-15 09:46 ppasr/model_utils/loss/__init__.py
--rw-rw-rw-  2.0 fat     2885 b- defN 23-Mar-15 13:56 ppasr/model_utils/loss/ctc.py
+-rw-rw-rw-  2.0 fat     2855 b- defN 24-Apr-29 14:50 ppasr/model_utils/loss/ctc.py
 -rw-rw-rw-  2.0 fat     3316 b- defN 22-Nov-15 09:53 ppasr/model_utils/loss/label_smoothing_loss.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-20 12:39 ppasr/model_utils/squeezeformer/__init__.py
 -rw-rw-rw-  2.0 fat     8318 b- defN 23-Jan-30 11:56 ppasr/model_utils/squeezeformer/attention.py
 -rw-rw-rw-  2.0 fat     2240 b- defN 22-Dec-03 10:03 ppasr/model_utils/squeezeformer/conv2d.py
--rw-rw-rw-  2.0 fat     6874 b- defN 23-Feb-15 10:43 ppasr/model_utils/squeezeformer/convolution.py
--rw-rw-rw-  2.0 fat    23943 b- defN 23-Feb-15 10:43 ppasr/model_utils/squeezeformer/encoder.py
+-rw-rw-rw-  2.0 fat     6844 b- defN 24-Apr-29 14:50 ppasr/model_utils/squeezeformer/convolution.py
+-rw-rw-rw-  2.0 fat    23913 b- defN 24-Apr-29 14:50 ppasr/model_utils/squeezeformer/encoder.py
 -rw-rw-rw-  2.0 fat     9759 b- defN 23-Jan-30 11:56 ppasr/model_utils/squeezeformer/model.py
 -rw-rw-rw-  2.0 fat     2497 b- defN 23-Jan-30 11:56 ppasr/model_utils/squeezeformer/positionwise.py
 -rw-rw-rw-  2.0 fat     2606 b- defN 23-Jan-30 11:56 ppasr/model_utils/squeezeformer/subsampling.py
 -rw-rw-rw-  2.0 fat     8788 b- defN 23-Jan-30 11:56 ppasr/model_utils/squeezeformer/time_reduction.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-15 09:53 ppasr/model_utils/transformer/__init__.py
--rw-rw-rw-  2.0 fat    17005 b- defN 22-Nov-16 04:10 ppasr/model_utils/transformer/decoder.py
+-rw-rw-rw-  2.0 fat    16948 b- defN 24-Apr-29 14:50 ppasr/model_utils/transformer/decoder.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-20 12:39 ppasr/model_utils/utils/__init__.py
 -rw-rw-rw-  2.0 fat     5120 b- defN 22-Oct-22 09:46 ppasr/model_utils/utils/base.py
 -rw-rw-rw-  2.0 fat      935 b- defN 22-Oct-20 12:39 ppasr/model_utils/utils/cmvn.py
 -rw-rw-rw-  2.0 fat     7642 b- defN 22-Oct-20 12:39 ppasr/model_utils/utils/common.py
 -rw-rw-rw-  2.0 fat     7536 b- defN 23-Jan-30 11:56 ppasr/model_utils/utils/mask.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-30 11:56 ppasr/optimizer/__init__.py
--rw-rw-rw-  2.0 fat    10523 b- defN 23-Jan-30 11:56 ppasr/optimizer/scheduler.py
+-rw-rw-rw-  2.0 fat    10493 b- defN 24-Apr-29 14:50 ppasr/optimizer/scheduler.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jul-12 12:38 ppasr/utils/__init__.py
 -rw-rw-rw-  2.0 fat     2844 b- defN 23-Jan-30 11:56 ppasr/utils/logger.py
 -rw-rw-rw-  2.0 fat      893 b- defN 22-Jul-12 12:38 ppasr/utils/metrics.py
 -rw-rw-rw-  2.0 fat    13549 b- defN 23-Jan-30 11:56 ppasr/utils/model_summary.py
 -rw-rw-rw-  2.0 fat     3910 b- defN 23-Feb-22 11:57 ppasr/utils/utils.py
--rw-rw-rw-  2.0 fat    11558 b- defN 24-Apr-27 06:48 ppasr-2.4.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    11142 b- defN 24-Apr-27 06:48 ppasr-2.4.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-27 06:48 ppasr-2.4.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-27 06:48 ppasr-2.4.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     7609 b- defN 24-Apr-27 06:48 ppasr-2.4.7.dist-info/RECORD
-83 files, 2288398 bytes uncompressed, 1636700 bytes compressed:  28.5%
+-rw-rw-rw-  2.0 fat    11558 b- defN 24-May-01 03:15 ppasr-2.4.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    11142 b- defN 24-May-01 03:15 ppasr-2.4.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-01 03:15 ppasr-2.4.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-01 03:15 ppasr-2.4.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     7609 b- defN 24-May-01 03:15 ppasr-2.4.8.dist-info/RECORD
+83 files, 2291646 bytes uncompressed, 1637495 bytes compressed:  28.6%
```

## zipnote {}

```diff
@@ -228,23 +228,23 @@
 
 Filename: ppasr/utils/model_summary.py
 Comment: 
 
 Filename: ppasr/utils/utils.py
 Comment: 
 
-Filename: ppasr-2.4.7.dist-info/LICENSE
+Filename: ppasr-2.4.8.dist-info/LICENSE
 Comment: 
 
-Filename: ppasr-2.4.7.dist-info/METADATA
+Filename: ppasr-2.4.8.dist-info/METADATA
 Comment: 
 
-Filename: ppasr-2.4.7.dist-info/WHEEL
+Filename: ppasr-2.4.8.dist-info/WHEEL
 Comment: 
 
-Filename: ppasr-2.4.7.dist-info/top_level.txt
+Filename: ppasr-2.4.8.dist-info/top_level.txt
 Comment: 
 
-Filename: ppasr-2.4.7.dist-info/RECORD
+Filename: ppasr-2.4.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ppasr/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "2.4.7"
+__version__ = "2.4.8"
 # 项目支持的模型
 SUPPORT_MODEL = ['squeezeformer', 'efficient_conformer', 'conformer', 'deepspeech2']
```

## ppasr/trainer.py

```diff
@@ -1,16 +1,18 @@
 import io
 import json
 import os
+import platform
 import shutil
 import time
 from collections import Counter
 from contextlib import nullcontext
 from datetime import timedelta
 
+import numpy as np
 import paddle
 import yaml
 from paddle.distributed import fleet
 from paddle.io import DataLoader
 from tqdm import tqdm
 from visualdl import LogWriter
 
@@ -55,14 +57,18 @@
         self.configs = dict_to_object(configs)
         self.local_rank = 0
         self.use_gpu = use_gpu
         assert self.configs.use_model in SUPPORT_MODEL, f'没有该模型：{self.configs.use_model}'
         self.model = None
         self.test_loader = None
         self.beam_search_decoder = None
+        if platform.system().lower() == 'windows':
+            self.configs.dataset_conf.num_workers = 0
+            self.configs.dataset_conf.prefetch_factor = 2
+            logger.warning('Windows系统不支持多线程读取数据，已自动关闭！')
         self.max_step, self.train_step = None, None
         self.train_loss, self.train_eta_sec = None, None
         self.eval_best_error_rate = None
         self.eval_loss, self.eval_error_result = None, None
         self.test_log_step, self.train_log_step = 0, 0
         self.stop_train, self.stop_eval = False, False
 
@@ -114,14 +120,59 @@
         self.test_loader = DataLoader(dataset=self.test_dataset,
                                       batch_size=self.configs.dataset_conf.batch_size,
                                       collate_fn=collate_fn,
                                       prefetch_factor=self.configs.dataset_conf.prefetch_factor,
                                       use_shared_memory=self.configs.dataset_conf.use_shared_memory,
                                       num_workers=self.configs.dataset_conf.num_workers)
 
+    # 提取特征保存文件
+    def extract_features(self, save_dir='dataset/features'):
+        for i, data_list_file in enumerate([self.configs.dataset_conf.train_manifest,
+                                            self.configs.dataset_conf.test_manifest]):
+            save_dir1 = os.path.join(save_dir, data_list_file.split('.')[-1])
+            os.makedirs(save_dir1, exist_ok=True)
+            test_dataset = PPASRDataset(preprocess_configs=self.configs.preprocess_conf,
+                                        data_manifest=data_list_file,
+                                        vocab_filepath=self.configs.dataset_conf.dataset_vocab,
+                                        manifest_type=self.configs.dataset_conf.manifest_type,
+                                        max_duration=-1)
+            save_dir_num = f'{int(time.time())}'
+            os.makedirs(os.path.join(str(save_dir1), save_dir_num), exist_ok=True)
+            all_feature, time_sum, index = None, 0, 0
+            save_data_list = data_list_file.replace('manifest', 'manifest_features')
+            with open(save_data_list, 'w', encoding='utf-8') as f:
+                for i in tqdm(range(len(test_dataset))):
+                    feature, _ = test_dataset[i]
+                    data_list = test_dataset.get_one_list(idx=i)
+                    time_sum += data_list['duration']
+                    if all_feature is None:
+                        index += 1
+                        all_feature = feature
+                        if index >= 1000:
+                            index = 0
+                            save_dir_num = f'{int(time.time())}'
+                            os.makedirs(os.path.join(str(save_dir1), save_dir_num), exist_ok=True)
+                        save_path = os.path.join(str(save_dir1), save_dir_num,
+                                                 f'{int(time.time() * 1000)}.npy').replace('\\', '/')
+                    else:
+                        all_feature = np.concatenate((all_feature, feature), axis=0)
+                    new_data_list = {"audio_filepath": save_path,
+                                     "duration": data_list['duration'],
+                                     "text": data_list['text'],
+                                     "start_frame": all_feature.shape[0] - feature.shape[0],
+                                     "end_frame": all_feature.shape[0]}
+                    f.write(f'{json.dumps(new_data_list, ensure_ascii=False)}\n')
+                    if time_sum > 600:
+                        np.save(save_path, all_feature)
+                        all_feature, time_sum = None, 0
+                if all_feature is not None:
+                    np.save(save_path, all_feature)
+                    print(save_path)
+            logger.info(f'[{data_list_file}]列表中的数据已提取特征完成，新列表为：[{save_data_list}]')
+
     def __setup_model(self, input_dim, vocab_size, is_train=False):
         from ppasr.model_utils.squeezeformer.model import SqueezeformerModel
         from ppasr.model_utils.conformer.model import ConformerModel
         from ppasr.model_utils.efficient_conformer.model import EfficientConformerModel
         from ppasr.model_utils.deepspeech2.model import DeepSpeech2Model
         # 获取模型
         if self.configs.use_model == 'squeezeformer':
```

## ppasr/data_utils/reader.py

```diff
@@ -46,45 +46,53 @@
             # 获取二进制的数据列表
             self.dataset_reader = DatasetReader(data_path=data_manifest,
                                                 min_duration=min_duration,
                                                 max_duration=max_duration)
             self.data_list = self.dataset_reader.get_keys()
 
     def __getitem__(self, idx):
-        # 获取数据列表
-        if self.manifest_type == 'txt':
-            data_list = self.data_list[idx]
-        elif self.manifest_type == 'binary':
-            data_list = self.dataset_reader.get_data(self.data_list[idx])
-        else:
-            raise Exception(f'没有该类型：{self.manifest_type}')
-        if 'start_time' not in data_list.keys():
-            # 分割音频路径和标签
-            audio_file, transcript = data_list["audio_filepath"], data_list["text"]
-            # 读取音频
-            audio_segment = AudioSegment.from_file(audio_file)
+        data_list = self.get_one_list(idx)
+        # 分割音频路径和标签
+        audio_file, transcript = data_list["audio_filepath"], data_list["text"]
+        # 如果后缀名为.npy的文件，那么直接读取
+        if audio_file.endswith('.npy'):
+            start_frame, end_frame = data_list["start_frame"], data_list["end_frame"]
+            feature = np.load(audio_file)
+            feature = feature[start_frame:end_frame, :]
         else:
-            # 分割音频路径和标签
-            audio_file, transcript = data_list["audio_filepath"], data_list["text"]
-            start_time, end_time = data_list["start_time"], data_list["end_time"]
-            # 分割读取音频
-            audio_segment = AudioSegment.slice_from_file(audio_file, start=start_time, end=end_time)
-        # 音频增强
-        self._augmentation_pipeline.transform_audio(audio_segment)
-        # 预处理，提取特征
-        feature = self._audio_featurizer.featurize(audio_segment)
+            if 'start_time' not in data_list.keys():
+                # 读取音频
+                audio_segment = AudioSegment.from_file(audio_file)
+            else:
+                start_time, end_time = data_list["start_time"], data_list["end_time"]
+                # 分割读取音频
+                audio_segment = AudioSegment.slice_from_file(audio_file, start=start_time, end=end_time)
+            # 音频增强
+            self._augmentation_pipeline.transform_audio(audio_segment)
+            # 预处理，提取特征
+            feature = self._audio_featurizer.featurize(audio_segment)
         transcript = self._text_featurizer.featurize(transcript)
         # 特征增强
         feature = self._augmentation_pipeline.transform_feature(feature)
         transcript = np.array(transcript, dtype=np.int32)
         return feature.astype(np.float32), transcript
 
     def __len__(self):
         return len(self.data_list)
 
+    def get_one_list(self, idx):
+        # 获取数据列表
+        if self.manifest_type == 'txt':
+            data_list = self.data_list[idx]
+        elif self.manifest_type == 'binary':
+            data_list = self.dataset_reader.get_data(self.data_list[idx])
+        else:
+            raise Exception(f'没有该类型：{self.manifest_type}')
+        return data_list
+
     @property
     def feature_dim(self):
         """返回音频特征大小
 
         :return: 词汇表大小
         :rtype: int
         """
```

## ppasr/model_utils/conformer/convolution.py

```diff
@@ -1,22 +1,23 @@
 from typing import Tuple
 
 import paddle
 from paddle import nn
-from typeguard import check_argument_types
+from typeguard import typechecked
 
 from ppasr.model_utils.utils.common import masked_fill
 from ppasr.model_utils.utils.base import Conv1D
 
 __all__ = ['ConvolutionModule']
 
 
 class ConvolutionModule(nn.Layer):
     """ConvolutionModule in Conformer model."""
 
+    @typechecked
     def __init__(self,
                  channels: int,
                  kernel_size: int = 15,
                  activation: nn.Layer = nn.ReLU(),
                  norm: str = "batch_norm",
                  causal: bool = False,
                  bias: bool = True):
@@ -25,15 +26,14 @@
             channels (int): The number of channels of conv layers.
             kernel_size (int): Kernel size of conv layers.
             activation (nn.Layer): Activation Layer.
             norm (str): Normalization type, 'batch_norm' or 'layer_norm'
             causal (bool): Whether use causal convolution or not
             bias (bool): Whether Conv with bias or not
         """
-        assert check_argument_types()
         super().__init__()
         self.pointwise_conv1 = Conv1D(channels,
                                       2 * channels,
                                       kernel_size=1,
                                       stride=1,
                                       padding=0,
                                       bias_attr=None
```

## ppasr/model_utils/conformer/encoder.py

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Tuple
 
 import paddle
 from paddle import nn
-from typeguard import check_argument_types
+from typeguard import typechecked
 
 from ppasr.model_utils.conformer.attention import MultiHeadedAttention
 from ppasr.model_utils.conformer.attention import RelPositionMultiHeadedAttention
 from ppasr.model_utils.utils.base import LayerNorm, Linear
 from ppasr.model_utils.conformer.convolution import ConvolutionModule
 from ppasr.model_utils.conformer.embedding import NoPositionalEncoding
 from ppasr.model_utils.conformer.embedding import PositionalEncoding
@@ -20,14 +20,15 @@
 from ppasr.model_utils.utils.mask import add_optional_chunk_mask
 from ppasr.model_utils.utils.mask import make_non_pad_mask
 
 
 class ConformerEncoder(nn.Layer):
     """Conformer encoder module."""
 
+    @typechecked
     def __init__(
             self,
             input_size: int,
             output_size: int = 256,
             attention_heads: int = 4,
             linear_units: int = 2048,
             num_blocks: int = 6,
@@ -84,15 +85,14 @@
             input_size to use_dynamic_chunk, see in BaseEncoder
             macaron_style (bool): Whether to use macaron style for positionwise layer.
             activation_type (str): Encoder activation function type.
             use_cnn_module (bool): Whether to use convolution module.
             cnn_module_kernel (int): Kernel size of convolution module.
             causal (bool): whether to use causal convolution or not.
         """
-        assert check_argument_types()
         super().__init__()
         self._output_size = output_size
 
         if pos_enc_layer_type == "abs_pos":
             pos_enc_class = PositionalEncoding
         elif pos_enc_layer_type == "rel_pos":
             pos_enc_class = RelPositionalEncoding
```

## ppasr/model_utils/efficient_conformer/convolution.py

```diff
@@ -1,23 +1,24 @@
 from typing import Tuple
 
 import paddle
 from paddle import nn
 from paddle.nn import initializer as I
-from typeguard import check_argument_types
+from typeguard import typechecked
 
 from ppasr.model_utils.utils.base import Conv1D, BatchNorm1D, LayerNorm
 from ppasr.model_utils.utils.common import masked_fill
 
 __all__ = ['ConvolutionModule']
 
 
 class ConvolutionModule(nn.Layer):
     """ConvolutionModule in Conformer model."""
 
+    @typechecked
     def __init__(self,
                  channels: int,
                  kernel_size: int = 15,
                  activation: nn.Layer = nn.ReLU(),
                  norm: str = "batch_norm",
                  causal: bool = False,
                  bias: bool = True,
@@ -25,15 +26,14 @@
         """Construct an ConvolutionModule object.
         Args:
             channels (int): The number of channels of conv layers.
             kernel_size (int): Kernel size of conv layers.
             causal (int): Whether use causal convolution or not
             stride (int): Stride Convolution, for efficient Conformer
         """
-        assert check_argument_types()
         super().__init__()
 
         self.pointwise_conv1 = Conv1D(channels,
                                       2 * channels,
                                       kernel_size=1,
                                       stride=1,
                                       padding=0,
```

## ppasr/model_utils/efficient_conformer/encoder.py

```diff
@@ -1,13 +1,13 @@
 from typing import Tuple, Union, Optional, List
 
 import paddle
 import paddle.nn as nn
 import paddle.nn.functional as F
-from typeguard import check_argument_types
+from typeguard import typechecked
 
 from ppasr.model_utils.conformer.attention import MultiHeadedAttention, RelPositionMultiHeadedAttention
 from ppasr.model_utils.conformer.embedding import PositionalEncoding, RelPositionalEncoding, NoPositionalEncoding
 from ppasr.model_utils.conformer.encoder import ConformerEncoderLayer
 from ppasr.model_utils.conformer.positionwise import PositionwiseFeedForward
 from ppasr.model_utils.conformer.subsampling import LinearNoSubsampling, Conv2dSubsampling4, Conv2dSubsampling6, \
     Conv2dSubsampling8
@@ -18,14 +18,15 @@
 from ppasr.model_utils.utils.common import get_activation
 from ppasr.model_utils.utils.mask import make_non_pad_mask, add_optional_chunk_mask
 
 
 class EfficientConformerEncoder(nn.Layer):
     """Conformer encoder module."""
 
+    @typechecked
     def __init__(
             self,
             input_size: int,
             output_size: int = 256,
             attention_heads: int = 4,
             linear_units: int = 2048,
             num_blocks: int = 6,
@@ -65,15 +66,14 @@
             causal (bool): whether to use causal convolution or not.
             stride_layer_idx (list): layer id with StrideConv, start from 0
             stride (list): stride size of each StrideConv in efficient conformer
             group_layer_idx (list): layer id with GroupedAttention, start from 0
             group_size (int): group size of every GroupedAttention layer
             stride_kernel (bool): default True. True: recompute cnn kernels with stride.
         """
-        assert check_argument_types()
         super().__init__()
         self._output_size = output_size
 
         if pos_enc_layer_type == "abs_pos":
             pos_enc_class = PositionalEncoding
         elif pos_enc_layer_type == "rel_pos":
             pos_enc_class = RelPositionalEncoding
```

## ppasr/model_utils/loss/ctc.py

```diff
@@ -1,30 +1,30 @@
 import paddle
 import paddle.nn.functional as F
-from typeguard import check_argument_types
+from typeguard import typechecked
 
 
 class CTCLoss(paddle.nn.Layer):
     """CTC module"""
 
+    @typechecked
     def __init__(
             self,
             odim: int,
             encoder_output_size: int,
             dropout_rate: float = 0.0,
             reduce: bool = True,
     ):
         """ Construct CTC module
         Args:
             odim: dimension of outputs
             encoder_output_size: number of encoder projection units
             dropout_rate: dropout rate (0.0 ~ 1.0)
             reduce: reduce the CTC loss into a scalar
         """
-        assert check_argument_types()
         super().__init__()
         eprojs = encoder_output_size
         self.dropout_rate = dropout_rate
         self.ctc_lo = paddle.nn.Linear(eprojs, odim)
 
         reduction_type = "sum" if reduce else "none"
         self.ctc_loss = paddle.nn.CTCLoss(reduction=reduction_type)
```

## ppasr/model_utils/squeezeformer/convolution.py

```diff
@@ -1,23 +1,24 @@
 from typing import Tuple
 
 import paddle
 from paddle import nn
 from paddle.nn import initializer as I
-from typeguard import check_argument_types
+from typeguard import typechecked
 
 from ppasr.model_utils.utils.base import Conv1D, BatchNorm1D, LayerNorm
 from ppasr.model_utils.utils.common import masked_fill
 
 __all__ = ['ConvolutionModule']
 
 
 class ConvolutionModule(nn.Layer):
     """ConvolutionModule in Conformer model."""
 
+    @typechecked
     def __init__(self,
                  channels: int,
                  kernel_size: int = 15,
                  activation: nn.Layer = nn.ReLU(),
                  norm: str = "batch_norm",
                  causal: bool = False,
                  bias: bool = True,
@@ -25,15 +26,14 @@
                  init_weights: bool = False):
         """Construct an ConvolutionModule object.
         Args:
             channels (int): The number of channels of conv layers.
             kernel_size (int): Kernel size of conv layers.
             causal (int): Whether use causal convolution or not
         """
-        assert check_argument_types()
         super().__init__()
         self.bias = bias
         self.channels = channels
         self.kernel_size = kernel_size
         self.adaptive_scale = adaptive_scale
         ada_scale = self.create_parameter([1, 1, channels], default_initializer=I.Constant(1.0))
         self.add_parameter('ada_scale', ada_scale)
```

## ppasr/model_utils/squeezeformer/encoder.py

```diff
@@ -1,12 +1,12 @@
 import paddle
 import paddle.nn as nn
 from typing import Tuple, Union, Optional, List
 
-from typeguard import check_argument_types
+from typeguard import typechecked
 
 from ppasr.model_utils.conformer.attention import MultiHeadedAttention
 from ppasr.model_utils.conformer.embedding import RelPositionalEncoding
 from ppasr.model_utils.squeezeformer.attention import RelPositionMultiHeadedAttention
 from ppasr.model_utils.squeezeformer.convolution import ConvolutionModule
 from ppasr.model_utils.squeezeformer.positionwise import PositionwiseFeedForward
 from ppasr.model_utils.squeezeformer.subsampling import DepthwiseConv2DSubsampling4
@@ -16,14 +16,15 @@
 from ppasr.model_utils.utils.common import get_activation
 from ppasr.model_utils.utils.mask import make_non_pad_mask, add_optional_chunk_mask
 
 __all__ = ["SqueezeformerEncoder"]
 
 
 class SqueezeformerEncoder(nn.Layer):
+    @typechecked
     def __init__(
             self,
             input_size: int,
             encoder_dim: int = 256,
             output_size: int = 256,
             attention_heads: int = 4,
             num_blocks: int = 12,
@@ -70,15 +71,14 @@
             cnn_module_kernel (int): Kernel size of CNN module.
             activation_type (str): Encoder activation function type.
             cnn_module_kernel (int): Kernel size of convolution module.
             adaptive_scale (bool): Whether to use adaptive scale.
             init_weights (bool): Whether to initialize weights.
             causal (bool): whether to use causal convolution or not.
         """
-        assert check_argument_types()
         super().__init__()
         self.global_cmvn = global_cmvn
         self.reduce_idx: Optional[Union[int, List[int]]] = [reduce_idx] \
             if type(reduce_idx) == int else reduce_idx
         self.recover_idx: Optional[Union[int, List[int]]] = [recover_idx] \
             if type(recover_idx) == int else recover_idx
         self.check_ascending_list()
```

## ppasr/model_utils/transformer/decoder.py

```diff
@@ -1,13 +1,13 @@
 from typing import List
 from typing import Optional, Tuple
 
 import paddle
 from paddle import nn
-from typeguard import check_argument_types
+from typeguard import typechecked
 
 from ppasr.model_utils.conformer.attention import MultiHeadedAttention
 from ppasr.model_utils.utils.base import Embedding, LayerNorm, Linear
 from ppasr.model_utils.conformer.embedding import PositionalEncoding
 from ppasr.model_utils.conformer.positionwise import PositionwiseFeedForward
 from ppasr.model_utils.utils.mask import (subsequent_mask, make_non_pad_mask)
 
@@ -30,14 +30,15 @@
             True: use layer_norm before each sub-block of a layer.
             False: use layer_norm after each sub-block of a layer.
         concat_after: whether to concat attention layer's input and output
             True: x -> x + linear(concat(x, att(x)))
             False: x -> x + att(x)
     """
 
+    @typechecked
     def __init__(self,
                  vocab_size: int,
                  encoder_output_size: int,
                  attention_heads: int = 4,
                  linear_units: int = 2048,
                  num_blocks: int = 6,
                  r_num_blocks: int = 0,
@@ -46,16 +47,14 @@
                  self_attention_dropout_rate: float = 0.0,
                  src_attention_dropout_rate: float = 0.0,
                  input_layer: str = "embed",
                  use_output_layer: bool = True,
                  normalize_before: bool = True,
                  concat_after: bool = False,
                  max_len: int = 5000):
-        assert check_argument_types()
-
         nn.Layer.__init__(self)
         self.left_decoder = TransformerDecoder(
             vocab_size, encoder_output_size, attention_heads, linear_units,
             num_blocks, dropout_rate, positional_dropout_rate,
             self_attention_dropout_rate, src_attention_dropout_rate,
             input_layer, use_output_layer, normalize_before, concat_after,
             max_len)
@@ -141,14 +140,15 @@
             True: use layer_norm before each sub-block of a layer.
             False: use layer_norm after each sub-block of a layer.
         concat_after: whether to concat attention layer's input and output
             True: x -> x + linear(concat(x, att(x)))
             False: x -> x + att(x)
     """
 
+    @typechecked
     def __init__(self,
                  vocab_size: int,
                  encoder_output_size: int,
                  attention_heads: int = 4,
                  linear_units: int = 2048,
                  num_blocks: int = 6,
                  dropout_rate: float = 0.1,
@@ -156,17 +156,14 @@
                  self_attention_dropout_rate: float = 0.0,
                  src_attention_dropout_rate: float = 0.0,
                  input_layer: str = "embed",
                  use_output_layer: bool = True,
                  normalize_before: bool = True,
                  concat_after: bool = False,
                  max_len: int = 5000):
-
-        assert check_argument_types()
-
         nn.Layer.__init__(self)
         self.selfattention_layer_type = 'selfattn'
         attention_dim = encoder_output_size
 
         if input_layer == "embed":
             self.embed = nn.Sequential(
                 Embedding(vocab_size, attention_dim),
```

## ppasr/optimizer/scheduler.py

```diff
@@ -1,12 +1,12 @@
 import math
 from typing import Union
 
 from paddle.optimizer.lr import LRScheduler
-from typeguard import check_argument_types
+from typeguard import typechecked
 
 
 class WarmupLR(LRScheduler):
     """The WarmupLR scheduler
     This scheduler is almost same as NoamLR Scheduler except for following
     difference:
     NoamLR:
@@ -14,17 +14,17 @@
              * min(step ** -0.5, step * warmup_step ** -1.5)
     WarmupLR:
         lr = optimizer.lr * warmup_step ** 0.5
              * min(step ** -0.5, step * warmup_step ** -1.5)
     Note that the maximum lr equals to optimizer.lr in this scheduler.
     """
 
+    @typechecked
     def __init__(self, learning_rate=1.0, warmup_steps: Union[int, float] = 25000,
                  min_lr=1e-5, last_epoch=-1, verbose=False):
-        assert check_argument_types()
         self.warmup_steps = warmup_steps
         self.min_lr = min_lr
         super().__init__(learning_rate, last_epoch, verbose)
 
     def __repr__(self):
         return f"{self.__class__.__name__}(warmup_steps={self.warmup_steps}, lr={self.base_lr}, " \
                f"min_lr={self.min_lr}, last_epoch={self.last_epoch})"
```

## Comparing `ppasr-2.4.7.dist-info/LICENSE` & `ppasr-2.4.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ppasr-2.4.7.dist-info/METADATA` & `ppasr-2.4.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppasr
-Version: 2.4.7
+Version: 2.4.8
 Summary: Automatic speech recognition toolkit on PaddlePaddle
 Home-page: https://github.com/yeyupiaoling/PPASR
 Download-URL: https://github.com/yeyupiaoling/PPASR.git
 Author: yeyupiaoling
 License: Apache License 2.0
 Keywords: asr,paddle
 Classifier: Intended Audience :: Developers
@@ -30,15 +30,15 @@
 Requires-Dist: resampy >=0.2.2
 Requires-Dist: zhconv >=1.4.2
 Requires-Dist: ijson >=3.1.4
 Requires-Dist: pyyaml >=5.4.1
 Requires-Dist: termcolor >=1.1.0
 Requires-Dist: scikit-learn >=1.0.2
 Requires-Dist: paddleaudio >=1.0.1
-Requires-Dist: typeguard ==2.13.3
+Requires-Dist: typeguard >=2.13.3
 Requires-Dist: onnxruntime >=1.11.1
 Requires-Dist: av >=10.0.0
 
 ![python version](https://img.shields.io/badge/python-3.8+-orange.svg)
 ![GitHub forks](https://img.shields.io/github/forks/yeyupiaoling/PPASR)
 ![GitHub Repo stars](https://img.shields.io/github/stars/yeyupiaoling/PPASR)
 ![GitHub](https://img.shields.io/github/license/yeyupiaoling/PPASR)
```

## Comparing `ppasr-2.4.7.dist-info/RECORD` & `ppasr-2.4.8.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-ppasr/__init__.py,sha256=l_HahMoHfGkdZw1mOdRz8Fr-YZbXbpaJO9UNJQ3Ogo8,134
+ppasr/__init__.py,sha256=mXSyH3F8FliyX8F8wG3MIc5sMopU-8YJJJSrrRjNECM,134
 ppasr/predict.py,sha256=5xUrdL6My1WBf4Kc8sx39KV3RN7KmI8oPks5MWq5aYc,17895
-ppasr/trainer.py,sha256=0oBSqnddzLCPTI0DcHS4Izs6WCKO2AGBbOMn5ZzXYFw,38580
+ppasr/trainer.py,sha256=xbbtXXWNT_jthFp2vCDTWfsTJTcmJmOGz-6mq5yqn90,41804
 ppasr/data_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ppasr/data_utils/audio.py,sha256=oGW1cbA_SmUVcfBV4ZNTKXwzTtBpFCYAOXLOtyJGxok,23844
 ppasr/data_utils/binary.py,sha256=qNXcZRcLcehLdGg4YwP5FBcLCpFp8Fd9YVSb5numyzs,2377
 ppasr/data_utils/collate_fn.py,sha256=tG5c5EjaCaz3WBQTqTk2gjsBUCZldRp-9mXBP76kfHs,1584
 ppasr/data_utils/normalizer.py,sha256=kPavVCRVk59p_ZHIfE6G20fTCrna5YxN4yOmTzTs67w,5192
-ppasr/data_utils/reader.py,sha256=Zl7po0c5i6ggodRZwgzL3jrjSC8YVx7CigwlFx5d-uU,4244
+ppasr/data_utils/reader.py,sha256=djt3RZ9CYbo2rDsBPicgcyZVwuDEjdrdZ31oyl0h4NY,4565
 ppasr/data_utils/sampler.py,sha256=NKql8qAqNGHrbrFrQ9vLwWssV7cA7P3Pb9Fc0nkUI1g,8477
 ppasr/data_utils/utils.py,sha256=ECfUz6UA7RfjhMOc6huKwi1rCbD9LQn-dfYFk8pboCk,15686
 ppasr/data_utils/augmentor/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ppasr/data_utils/augmentor/augmentation.py,sha256=Y-ZizFZFAsxHkXMjA8jUKKMWcQlRIOHCmHqKkHR9J7Q,5787
 ppasr/data_utils/augmentor/base.py,sha256=Qw5AsIjpqDkggVkVyfPGTI_IwnfSuIWViRdgo7g2ze0,965
 ppasr/data_utils/augmentor/noise_perturb.py,sha256=EB3Y59EEytiXXCg1ixWUS99hkQJwYGxh-Ykh1E4zaG0,2570
 ppasr/data_utils/augmentor/resample.py,sha256=ugt2468E_SNvy6moQloD9TT92MXyvrX2skWyoDx2FMg,977
@@ -30,54 +30,54 @@
 ppasr/infer_utils/inference_predictor.py,sha256=_zhrht-u367KaDcQpT3vD3iC2Yvr6kuHBc3IAVneaSg,11174
 ppasr/infer_utils/pun_predictor.py,sha256=uW-vuP-etmzLjs0u26XwSUW1GBVNZOFzGTRwDSnzSq8,4696
 ppasr/infer_utils/silero_vad.onnx,sha256=o16_Uv085fFGmyo2FY26dhvEe5c-ozgrMYbKFbH1ryg,1807522
 ppasr/infer_utils/vad_predictor.py,sha256=5lVpoKRNgSbwLpDLE2GJeYdxaUd7xXXSAyRMWqJ6OrU,8614
 ppasr/model_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ppasr/model_utils/conformer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ppasr/model_utils/conformer/attention.py,sha256=aBC0pjz55EzXANhWBe03YYkEw4Al2_bGNLtFH4Kgnsg,12421
-ppasr/model_utils/conformer/convolution.py,sha256=7PpLJG0HtdH-bV5_F3JqtCJ-Po5wnz8Iiq7DMoM5c0I,5829
+ppasr/model_utils/conformer/convolution.py,sha256=XF3dBYx5K5mhNrALHgOIcXF7qZ5V82K7GilOd6v6vjU,5799
 ppasr/model_utils/conformer/embedding.py,sha256=v4d5qwf2iuY0e5my834VzMglcChOyoG8Wg6mCBjlORs,4738
-ppasr/model_utils/conformer/encoder.py,sha256=2qSnfVPWDP2UZI166O5ITs6m6xaOKc0T3WU0RL5Y0zc,19705
+ppasr/model_utils/conformer/encoder.py,sha256=-baXu5bB4nAGgdsA95Szldg28IqVtg3aZ9CLDVjupvQ,19675
 ppasr/model_utils/conformer/model.py,sha256=FBMHFIVIICvSkcwJxrdSLiYrPU6p3RCwqnznWSPJ-P4,9338
 ppasr/model_utils/conformer/positionwise.py,sha256=soQN-T5z_Ai37l70svpqMauus9BJ2WN_WOwf-4xGqyw,1286
 ppasr/model_utils/conformer/subsampling.py,sha256=wggQ0hjTtuhVm9IBsQayR7s6JE46eJ4WgvYW6LsEuFg,8793
 ppasr/model_utils/deepspeech2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ppasr/model_utils/deepspeech2/conv.py,sha256=5qbXL6R8IZ8yxeoR3mzXakW1QDQf_TXMO15PR_BsBbk,688
 ppasr/model_utils/deepspeech2/encoder.py,sha256=-bXwD9iNGMx5VbC4rcTplZCDO9DjdukXrg44_ecnnxw,4644
 ppasr/model_utils/deepspeech2/model.py,sha256=89A0_WDdy3ngly8Q2wPZjlv5-okoPDSyp3HofEwJkiM,4329
 ppasr/model_utils/efficient_conformer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ppasr/model_utils/efficient_conformer/attention.py,sha256=ZCOFcesKJrJCKJmRd-e_Esbdhvr_j021jHv83HJ8iMs,9054
-ppasr/model_utils/efficient_conformer/convolution.py,sha256=AbgMVWca_KVEiFHXl80U4GKh282SoiLdep4tngnUeVg,5754
-ppasr/model_utils/efficient_conformer/encoder.py,sha256=AvxVZhfBI2jM67gNtHogOQq1M1j3RGwaykzMn1EHQ7o,25366
+ppasr/model_utils/efficient_conformer/convolution.py,sha256=hD_1yDnaS4Ovbi8IMjbGOUK2Nz6VYY3Om4WiSmI2aMY,5724
+ppasr/model_utils/efficient_conformer/encoder.py,sha256=wu_nK2-E6ziDXpvNvcuP0HSCf1zqDXz7R095fJTxAHc,25336
 ppasr/model_utils/efficient_conformer/model.py,sha256=V5wBMp1YX88dgdgqjACSJYDVvU92LSg5O00YkywtGcw,9409
 ppasr/model_utils/efficient_conformer/subsampling.py,sha256=LeGLdoB6TteE10lQtoNpxcnAVmiGtiHzt3CYnlpBu6Q,2052
 ppasr/model_utils/loss/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ppasr/model_utils/loss/ctc.py,sha256=6Sgqnds_IF3gqZ9wUVoAW36x0kCfoJ50BLd4teXEU_U,2885
+ppasr/model_utils/loss/ctc.py,sha256=BAVwgBM0LO9SOKBMOapHYEMJmIyzYZ3oN_ESQSIUKfU,2855
 ppasr/model_utils/loss/label_smoothing_loss.py,sha256=n2zTodVZHTyck3wDuuhtmnb2cxfUiVL0jmyTBsIhf9A,3316
 ppasr/model_utils/squeezeformer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ppasr/model_utils/squeezeformer/attention.py,sha256=nDm7g0lbWC8LN5DWTcpAJzGZ7yEyWpCh0OaVZ2Yg3iQ,8318
 ppasr/model_utils/squeezeformer/conv2d.py,sha256=hQutZmES9ZNZREDgzRVfpN3OuSiUVXYLqMvYrylEddY,2240
-ppasr/model_utils/squeezeformer/convolution.py,sha256=wwyGU-Xo9BiXsVL9t_SfSS532d-VulyQMT1wXPU57UM,6874
-ppasr/model_utils/squeezeformer/encoder.py,sha256=B25wHYdYVt4gNQxBfFCBmktAQxs85EyvrFbme8sWglw,23943
+ppasr/model_utils/squeezeformer/convolution.py,sha256=1VHsRxyrUYaqwmA1bZRAImt9al_6DZoOcDpsQfOFtpo,6844
+ppasr/model_utils/squeezeformer/encoder.py,sha256=LQgUjusvB4UsUx-adiipCTptC9tStpzmrirSj1PjJLU,23913
 ppasr/model_utils/squeezeformer/model.py,sha256=qSbb73kEpcYTwO5si7U-YdvEoOjJd7zYWtjSQm2P_yM,9759
 ppasr/model_utils/squeezeformer/positionwise.py,sha256=wUpNEkqIfImAqPzJBqow85XHxKl34_nCjUx8JcPS5Vk,2497
 ppasr/model_utils/squeezeformer/subsampling.py,sha256=fhESqDc86rBiqBeCZjSZ0BqKj70dMzz8-dRoJ1XL-zc,2606
 ppasr/model_utils/squeezeformer/time_reduction.py,sha256=PSqMbMRRNpC1m-_4utaPP-2gZdY0_GSl95gIQnxD7xY,8788
 ppasr/model_utils/transformer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ppasr/model_utils/transformer/decoder.py,sha256=3IL6IX-p6Qy4FHulTu-u0LY7aJBz6Izsub0ap3GlVMc,17005
+ppasr/model_utils/transformer/decoder.py,sha256=I8rmPV25Q8aHAHq-Nw_KOSH4uwXTtTo4m5VQ2NeCCAo,16948
 ppasr/model_utils/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ppasr/model_utils/utils/base.py,sha256=sSeLW6lO89IVQxLB8Dsy385QYqMpp1zyw2ly_BQBHIw,5120
 ppasr/model_utils/utils/cmvn.py,sha256=7QMk7Z_ITMsZbaTY1WCE3K5n6xLpaLUozIdY3Q9XfK4,935
 ppasr/model_utils/utils/common.py,sha256=ys_Rhblo1ZMSZRlvX9ethMW2NMWVx-Uu-pGasWSwmNM,7642
 ppasr/model_utils/utils/mask.py,sha256=xYmWHIsLDactAxupBlfaRLQ_HFSuszelQlqAlRplh7o,7536
 ppasr/optimizer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ppasr/optimizer/scheduler.py,sha256=Ki-0T0JZS2_LCJsTo9Xvb2dHrUuDz0mxh6sH9mb3j2M,10523
+ppasr/optimizer/scheduler.py,sha256=mKqCIpuk14b27RmKQy8nIKoG8ltbClACwqOjT5Nmlfo,10493
 ppasr/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ppasr/utils/logger.py,sha256=eHExExIfsMSQD7B0iCh0TSzx257JZIanKJCK7BWp23s,2844
 ppasr/utils/metrics.py,sha256=PGnCSSGnJH61xOzuM0iaNDLGwAllZh0ILPSCPRcGIAg,893
 ppasr/utils/model_summary.py,sha256=75MjURp-FJ8B3c0AdMhg1T-ePWb4IJPvtwk8HertJa8,13549
 ppasr/utils/utils.py,sha256=mfL-DzN8XEn6k_5E7FZ53hGBQKEqFotAgl8-Njrnhtc,3910
-ppasr-2.4.7.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-ppasr-2.4.7.dist-info/METADATA,sha256=CR4v9Gk1EawGbN2E4x7OCCyp-37polWjN84m9qIwi54,11142
-ppasr-2.4.7.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-ppasr-2.4.7.dist-info/top_level.txt,sha256=bW0NEVoj4d41szj8YJKhSn7D-K3AX86ipdtJLH_yXD4,6
-ppasr-2.4.7.dist-info/RECORD,,
+ppasr-2.4.8.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+ppasr-2.4.8.dist-info/METADATA,sha256=7bw7vjo_rb3NOhR-YGIzG5SBUekCOnhJm4g_GyhRVE8,11142
+ppasr-2.4.8.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+ppasr-2.4.8.dist-info/top_level.txt,sha256=bW0NEVoj4d41szj8YJKhSn7D-K3AX86ipdtJLH_yXD4,6
+ppasr-2.4.8.dist-info/RECORD,,
```

