# Comparing `tmp/Pyara-0.1.29.tar.gz` & `tmp/Pyara-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Pyara-0.1.29.tar", last modified: Sat Jun 17 15:12:06 2023, max compression
+gzip compressed data, was "dist\Pyara-0.2.0.tar", last modified: Sun Jun 18 11:03:38 2023, max compression
```

## Comparing `Pyara-0.1.29.tar` & `Pyara-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 15:12:06.000000 Pyara-0.1.29/
--rw-rw-rw-   0        0        0     1098 2023-06-05 08:31:19.000000 Pyara-0.1.29/LICENSE
--rw-rw-rw-   0        0        0       73 2023-06-16 10:56:25.000000 Pyara-0.1.29/MANIFEST.in
--rw-rw-rw-   0        0        0      539 2023-06-17 15:12:06.000000 Pyara-0.1.29/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-17 15:12:06.000000 Pyara-0.1.29/Pyara.egg-info/
--rw-rw-rw-   0        0        0      539 2023-06-17 15:12:06.000000 Pyara-0.1.29/Pyara.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2023-06-17 15:12:06.000000 Pyara-0.1.29/Pyara.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 15:12:06.000000 Pyara-0.1.29/Pyara.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-21 09:07:37.000000 Pyara-0.1.29/Pyara.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       57 2023-06-17 15:12:06.000000 Pyara-0.1.29/Pyara.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-17 15:12:06.000000 Pyara-0.1.29/Pyara.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       48 2023-04-10 18:25:02.000000 Pyara-0.1.29/README.md
--rw-rw-rw-   0        0        0      950 2023-06-11 12:54:48.000000 Pyara-0.1.29/instruct.txt
--rw-rw-rw-   0        0        0    92204 2023-03-28 18:31:37.000000 Pyara-0.1.29/mozila11_1.wav
--rw-rw-rw-   0        0        0   164396 2023-03-28 18:37:21.000000 Pyara-0.1.29/mozila11_2.wav
-drwxrwxrwx   0        0        0        0 2023-06-17 15:12:06.000000 Pyara-0.1.29/pyara/
-drwxrwxrwx   0        0        0        0 2023-06-17 15:12:06.000000 Pyara-0.1.29/pyara/Model/
--rw-rw-rw-   0        0        0  1075221 2023-04-03 12:30:41.000000 Pyara-0.1.29/pyara/Model/Model_weights.bin
--rw-rw-rw-   0        0        0        0 2023-06-11 12:49:19.000000 Pyara-0.1.29/pyara/Model/__init__.py
--rw-rw-rw-   0        0        0     4177 2023-06-17 15:00:11.000000 Pyara-0.1.29/pyara/Model/model.py
--rw-rw-rw-   0        0        0      350 2023-06-14 09:04:25.000000 Pyara-0.1.29/pyara/__init__.py
--rw-rw-rw-   0        0        0     6412 2023-06-14 08:53:51.000000 Pyara-0.1.29/pyara/audio_prepare.py
--rw-rw-rw-   0        0        0     1029 2023-05-21 08:36:42.000000 Pyara-0.1.29/pyara/config.py
--rw-rw-rw-   0        0        0      836 2023-06-14 08:53:51.000000 Pyara-0.1.29/pyara/main.py
--rw-rw-rw-   0        0        0   184364 2023-03-28 18:31:37.000000 Pyara-0.1.29/pyara/mozila11_0.wav
--rw-rw-rw-   0        0        0       28 2023-06-14 09:11:56.000000 Pyara-0.1.29/pyara/some.txt
--rw-rw-rw-   0        0        0      108 2023-06-05 08:20:17.000000 Pyara-0.1.29/pyproject.toml
--rw-rw-rw-   0        0        0      276 2023-05-28 20:41:04.000000 Pyara-0.1.29/requirements.txt
--rw-rw-rw-   0        0        0      131 2023-05-30 08:51:00.000000 Pyara-0.1.29/requirements_dev.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 15:12:06.000000 Pyara-0.1.29/setup.cfg
--rw-rw-rw-   0        0        0     1180 2023-06-17 15:12:05.000000 Pyara-0.1.29/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 11:03:38.000000 Pyara-0.2.0/
+-rw-rw-rw-   0        0        0     1098 2023-06-05 08:31:19.000000 Pyara-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       73 2023-06-16 10:56:25.000000 Pyara-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      538 2023-06-18 11:03:38.000000 Pyara-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-18 11:03:38.000000 Pyara-0.2.0/Pyara.egg-info/
+-rw-rw-rw-   0        0        0      538 2023-06-18 11:03:38.000000 Pyara-0.2.0/Pyara.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2023-06-18 11:03:38.000000 Pyara-0.2.0/Pyara.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 11:03:38.000000 Pyara-0.2.0/Pyara.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-21 09:07:37.000000 Pyara-0.2.0/Pyara.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       57 2023-06-18 11:03:38.000000 Pyara-0.2.0/Pyara.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-18 11:03:38.000000 Pyara-0.2.0/Pyara.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       48 2023-04-10 18:25:02.000000 Pyara-0.2.0/README.md
+-rw-rw-rw-   0        0        0      950 2023-06-11 12:54:48.000000 Pyara-0.2.0/instruct.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 11:03:38.000000 Pyara-0.2.0/pyara/
+drwxrwxrwx   0        0        0        0 2023-06-18 11:03:38.000000 Pyara-0.2.0/pyara/Model/
+-rw-rw-rw-   0        0        0  1075221 2023-04-03 12:30:41.000000 Pyara-0.2.0/pyara/Model/Model_weights.bin
+-rw-rw-rw-   0        0        0        0 2023-06-11 12:49:19.000000 Pyara-0.2.0/pyara/Model/__init__.py
+-rw-rw-rw-   0        0        0     5305 2023-06-18 10:59:22.000000 Pyara-0.2.0/pyara/Model/model.py
+-rw-rw-rw-   0        0        0      318 2023-06-18 11:02:30.000000 Pyara-0.2.0/pyara/__init__.py
+-rw-rw-rw-   0        0        0     6543 2023-06-18 10:59:22.000000 Pyara-0.2.0/pyara/audio_prepare.py
+-rw-rw-rw-   0        0        0     1029 2023-05-21 08:36:42.000000 Pyara-0.2.0/pyara/config.py
+-rw-rw-rw-   0        0        0      692 2023-06-18 11:03:24.000000 Pyara-0.2.0/pyara/main.py
+-rw-rw-rw-   0        0        0      108 2023-06-05 08:20:17.000000 Pyara-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      276 2023-05-28 20:41:04.000000 Pyara-0.2.0/requirements.txt
+-rw-rw-rw-   0        0        0      131 2023-05-30 08:51:00.000000 Pyara-0.2.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 11:03:38.000000 Pyara-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1179 2023-06-18 11:03:24.000000 Pyara-0.2.0/setup.py
```

### Comparing `Pyara-0.1.29/LICENSE` & `Pyara-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.29/PKG-INFO` & `Pyara-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyara
-Version: 0.1.29
+Version: 0.2.0
 Summary: Library for audio classification
 Home-page: https://github.com/Millcool/Pyara.git
 Author: Ilya Mironov
 Author-email: ilyamironov210202@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Pyara-0.1.29/Pyara.egg-info/PKG-INFO` & `Pyara-0.2.0/Pyara.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyara
-Version: 0.1.29
+Version: 0.2.0
 Summary: Library for audio classification
 Home-page: https://github.com/Millcool/Pyara.git
 Author: Ilya Mironov
 Author-email: ilyamironov210202@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Pyara-0.1.29/instruct.txt` & `Pyara-0.2.0/instruct.txt`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.29/pyara/Model/Model_weights.bin` & `Pyara-0.2.0/pyara/Model/Model_weights.bin`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.29/pyara/Model/model.py` & `Pyara-0.2.0/pyara/Model/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,22 @@
 import torch
 from torch import nn
 import os
 from pyara.config import CFG
 
 
 class ResNetBlock(nn.Module):
-    """Class for ResNet Block description"""
+    """
+    Class representing a ResNet Block.
+
+    Args:
+        in_depth (int): Number of input channels.
+        depth (int): Number of output channels.
+        first (bool, optional): Whether it's the first block in the network. Defaults to False.
+    """
 
     def __init__(self, in_depth, depth, first=False):
         super(ResNetBlock,
               self).__init__()
         self.first = first
         self.conv1 = nn.Conv2d(in_depth, depth,
                                kernel_size=3,
@@ -30,15 +37,23 @@
                                 kernel_size=3,
                                 stride=3,
                                 padding=1)
         if not self.first:
             self.pre_bn = nn.BatchNorm2d(in_depth)
 
     def forward(self, signal):
-        """Forward method of model"""
+        """
+        Forward pass of the ResNet Block.
+
+        Args:
+            signal (torch.Tensor): Input tensor.
+
+        Returns:
+            torch.Tensor: Output tensor.
+        """
 
         # x is (B x d_in x T)
         prev = signal
         prev_mp = self.conv11(signal)
         if not self.first:
             out = self.pre_bn(signal)
             out = self.lrelu(out)
@@ -52,15 +67,34 @@
         out = self.conv2(out)
         # out is (B x depth x T/2)
         out = out + prev_mp
         return out
 
 
 class MFCCModel(nn.Module):
-    """Class for model description"""
+    """
+    Class representing a MFCC Model.
+
+    Copy code
+    Attributes:
+        conv1 (nn.Conv2d): Convolutional layer 1.
+        block1-9 (ResNetBlock): ResNet blocks 1-9.
+        mp (nn.MaxPool2d): Max pooling layer.
+        lrelu (nn.LeakyReLU): LeakyReLU activation function.
+        bn (nn.BatchNorm2d): Batch normalization layer.
+        dropout (nn.Dropout): Dropout layer.
+        logsoftmax (nn.LogSoftmax): LogSoftmax activation function.
+        fc1 (nn.Linear): Fully connected layer 1.
+        fc2 (nn.Linear): Fully connected layer 2.
+        model_name (str): Name of the model.
+
+    Methods:
+        forward(signal): Performs a forward pass of the model.
+
+    """
 
     def __init__(self):
         super(MFCCModel, self).__init__()
         self.conv1 = nn.Conv2d(1, 32,
                                kernel_size=3,
                                stride=1,
                                padding=1)
@@ -79,15 +113,23 @@
         self.dropout = nn.Dropout(0.5)
         self.logsoftmax = nn.LogSoftmax(dim=1)
         self.fc1 = nn.Linear(32, 128)
         self.fc2 = nn.Linear(128, 2)
         self.model_name = 'CNN_model_ResNet'
 
     def forward(self, signal):
-        """Forward method of MFCCModel"""
+        """
+           Forward pass of the MFCC Model.
+
+           Args:
+               signal (torch.Tensor): Input tensor.
+
+           Returns:
+               torch.Tensor: Output tensor.
+        """
 
         batch_size = signal.size(0)
         signal = signal.unsqueeze(dim=1)
         out = self.conv1(signal)
         out = self.block1(out)
         out = self.block2(out)
         out = self.block3(out)
@@ -111,18 +153,16 @@
         return out
 
 
 def model_eval():
     """Function for model Evaluation"""
 
     model = MFCCModel()
-    import os
-
-    module_path = os.path.dirname(__file__)  # Путь к текущему модулю (mylibrary.py)
+    module_path = os.path.dirname(__file__)
     weights_path = os.path.join(module_path,  'Model_weights.bin')
 
     model.load_state_dict(torch.load(weights_path,
                                      map_location=torch.device('cpu')))
     model.eval()
     model.to(CFG.device)
-    print(' Model Evaluated ! DONE !')
+    print('Model Evaluated!')
     return model
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Pyara-0.1.29/pyara/audio_prepare.py` & `Pyara-0.2.0/pyara/audio_prepare.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 """Module for audio prepare"""
 
 import torch
 import torchaudio
 
 from pyara.config import CFG
 
+
 # TODO __all__ во всех файлах чтобы в import опадали только написанные функции
 
-def cut_if_necessary(signal):
+def cut_if_necessary(signal, width=CFG.width):
     """cuts the audio signal to CFG.width samples """
 
-    if signal.shape[2] > CFG.width:
-        signal = signal[:, :, 0:CFG.width]
+    if signal.shape[2] > width:
+        signal = signal[:, :, 0:width]
     return signal
 
 
-def right_pad_if_necessary(signal):
+def right_pad_if_necessary(signal, width=CFG.width):
     """
      Выполняет дополнение последнего измерения входного сигнала вправо, если необходимо.
 
      Параметры:
      - signal (torch.Tensor): Тензор сигнала, представляющий многомерные данные.
                               Должен быть трехмерным тензором
                               с размерностью [batch_size, num_channels, signal_length].
 
      Возвращает:
      - torch.Tensor: Дополненный сигнал с выполненным дополнением последнего измерения вправо.
 
      """
     length_signal = signal.shape[2]
-    if length_signal < CFG.width:
-        num_missing_samples = CFG.width - length_signal
+    if length_signal < width:
+        num_missing_samples = width - length_signal
         last_dim_padding = (0, num_missing_samples)
         signal = torch.nn.functional.pad(signal, last_dim_padding)
     return signal
 
 
-def prepare_signal(voice_path):
+def prepare_signal(voice_path, width= CFG.width):
     """
       Подготавливает аудиосигнал для обработки.
 
       Аргументы:
       - voice_path (str): Путь к аудиофайлу.
 
       Возвращает:
@@ -70,20 +71,22 @@
       """
     signal, sample_rate = torchaudio.load(voice_path)
     signal = signal.mean(dim=0)
     signal = signal.unsqueeze(dim=0)
 
     signal = MFCC_spectrogram(signal)
 
-    signal = cut_if_necessary(signal)
-    signal = right_pad_if_necessary(signal)
+#TODO сделать зависимость от args, kwargs
+    signal = cut_if_necessary(signal, width)
+    signal = right_pad_if_necessary(signal, width)
 
     signal = signal.repeat(3, 1, 1)
     signal = signal.unsqueeze(dim=0)
     signal = signal.to(CFG.device)
+    print(f'Audio signal prepared !')
     return signal
 
 
 def prediction(model, signal):
     """
     Функция prediction выполняет предсказание с использованием заданной модели для входного сигнала.
 
@@ -115,15 +118,14 @@
     print(prediction)  # Выводит: 1
     ```
     """
     model = model.to(CFG.device)
     signal = signal.squeeze()
     with torch.no_grad():
         output = model(signal)
-        print(output)
         out = output.argmax(dim=-1).cpu().numpy()
     if out[0] == 1:
         return 1
     elif out[0] == 0:
         return 0
 
     return 0
```

### Comparing `Pyara-0.1.29/pyara/config.py` & `Pyara-0.2.0/pyara/config.py`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.29/setup.py` & `Pyara-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
                 'torchaudio>=0.13.1',
                 'soundfile==0.12.1',
                 'numpy'
                 ]
 
 # Создаст библиотеку для загрузки на PyPI
 setup(name='Pyara',
-      version='0.1.29',
+      version='0.2.0',
       url='https://github.com/Millcool/Pyara.git',
       license='MIT',
       author='Ilya Mironov',
       author_email='ilyamironov210202@gmail.com',
       description='Library for audio classification',
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

