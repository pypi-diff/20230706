# Comparing `tmp/BaseNN-0.1.6.tar.gz` & `tmp/BaseNN-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaseNN-0.1.6.tar", last modified: Wed May 31 09:49:51 2023, max compression
+gzip compressed data, was "dist/BaseNN-0.1.7.tar", last modified: Thu Jul  6 06:51:23 2023, max compression
```

## Comparing `BaseNN-0.1.6.tar` & `BaseNN-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-31 09:49:51.000000 BaseNN-0.1.6/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-31 09:49:51.000000 BaseNN-0.1.6/BaseNN/
--rw-rw-r--   0 user      (1001) user      (1001)    38906 2023-05-31 09:49:11.000000 BaseNN-0.1.6/BaseNN/BaseNN.py
--rw-rw-r--   0 user      (1001) user      (1001)      270 2023-05-24 09:07:14.000000 BaseNN-0.1.6/BaseNN/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-31 09:49:51.000000 BaseNN-0.1.6/BaseNN/examples/
--rw-rw-r--   0 user      (1001) user      (1001)    22901 2023-05-29 09:42:57.000000 BaseNN-0.1.6/BaseNN/examples/BaseNN_demo.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-26 07:13:38.000000 BaseNN-0.1.6/BaseNN/examples/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     3059 2023-04-13 07:47:30.000000 BaseNN-0.1.6/BaseNN/examples/pkl2pth.py
--rw-r--r--   0 user      (1001) user      (1001)     4409 2023-05-22 08:15:12.000000 BaseNN-0.1.6/BaseNN/load_data.py
--rw-rw-r--   0 user      (1001) user      (1001)     1256 2023-05-31 09:49:28.000000 BaseNN-0.1.6/BaseNN/version.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-31 09:49:51.000000 BaseNN-0.1.6/BaseNN.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-31 09:49:51.000000 BaseNN-0.1.6/BaseNN.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      375 2023-05-31 09:49:51.000000 BaseNN-0.1.6/BaseNN.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-05-31 09:49:51.000000 BaseNN-0.1.6/BaseNN.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       49 2023-05-31 09:49:51.000000 BaseNN-0.1.6/BaseNN.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1001) user      (1001)       80 2023-05-31 09:49:51.000000 BaseNN-0.1.6/BaseNN.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        7 2023-05-31 09:49:51.000000 BaseNN-0.1.6/BaseNN.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-18 03:21:26.000000 BaseNN-0.1.6/BaseNN.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)      346 2023-05-31 09:49:51.000000 BaseNN-0.1.6/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-05-31 09:49:51.000000 BaseNN-0.1.6/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     3827 2023-05-31 09:49:24.000000 BaseNN-0.1.6/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-07-06 06:51:23.000000 BaseNN-0.1.7/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-07-06 06:51:23.000000 BaseNN-0.1.7/BaseNN/
+-rw-rw-r--   0 user      (1001) user      (1001)    39047 2023-07-06 06:50:46.000000 BaseNN-0.1.7/BaseNN/BaseNN.py
+-rw-rw-r--   0 user      (1001) user      (1001)      270 2023-05-24 09:07:14.000000 BaseNN-0.1.7/BaseNN/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-07-06 06:51:23.000000 BaseNN-0.1.7/BaseNN/examples/
+-rw-rw-r--   0 user      (1001) user      (1001)    24607 2023-07-06 06:49:25.000000 BaseNN-0.1.7/BaseNN/examples/BaseNN_demo.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-26 07:13:38.000000 BaseNN-0.1.7/BaseNN/examples/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)     3059 2023-04-13 07:47:30.000000 BaseNN-0.1.7/BaseNN/examples/pkl2pth.py
+-rw-r--r--   0 user      (1001) user      (1001)     4409 2023-05-22 08:15:12.000000 BaseNN-0.1.7/BaseNN/load_data.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1256 2023-07-06 06:29:56.000000 BaseNN-0.1.7/BaseNN/version.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-07-06 06:51:23.000000 BaseNN-0.1.7/BaseNN.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      346 2023-07-06 06:51:23.000000 BaseNN-0.1.7/BaseNN.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      375 2023-07-06 06:51:23.000000 BaseNN-0.1.7/BaseNN.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-07-06 06:51:23.000000 BaseNN-0.1.7/BaseNN.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       49 2023-07-06 06:51:23.000000 BaseNN-0.1.7/BaseNN.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       80 2023-07-06 06:51:23.000000 BaseNN-0.1.7/BaseNN.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        7 2023-07-06 06:51:23.000000 BaseNN-0.1.7/BaseNN.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-18 03:21:26.000000 BaseNN-0.1.7/BaseNN.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)      346 2023-07-06 06:51:23.000000 BaseNN-0.1.7/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-07-06 06:51:23.000000 BaseNN-0.1.7/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     3827 2023-07-06 06:29:37.000000 BaseNN-0.1.7/setup.py
```

### Comparing `BaseNN-0.1.6/BaseNN/BaseNN.py` & `BaseNN-0.1.7/BaseNN/BaseNN.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,16 +120,14 @@
         self.rnn = False
         self.color = None # 若载入图片数据集，该变量表示灰度/RGB等颜色通道信息
         self.transform = None # 若载入图片数据集，该变量记录数据预处理操作
         if save_fold != None:
             self.save_fold = save_fold
         self.device = torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')
 
- 
-
     def add(self, layer=None, activation=None, optimizer=None, **kw):
         self.layers_num += 1
         self.layers.append(layer)
         if layer is not None and isinstance(layer,str):
             layer = layer.lower()
         if layer == 'linear':
             self.model.add_module('reshape', Reshape(self.batchsize))
@@ -418,45 +416,30 @@
 
             return self.dataloader
 
     def load_npz_data(self, data_path, batch_size=32, shuffle=True, classes=None,train_val_ratio=1.0):
         from .load_data import NpzDataset
         dataset = NpzDataset(data_path)
         self.dataset_size = int(len(dataset))
+        print(self.dataset_size)
         self.img_classes = classes
-
+        self.word2idx = dataset.word2idx
         # print(self.dataset_size)
         # self.dataloader = DataLoader(dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
         if 0 < train_val_ratio < 1:
             train_size =  int(train_val_ratio * self.dataset_size)
             val_size =  self.dataset_size - train_size
 
             train_dataset, val_dataset = torch.utils.data.random_split(dataset, [train_size, val_size])
             self.dataloader = DataLoader(train_dataset,batch_size=batch_size, shuffle=shuffle,num_workers=0)
             self.val_dataloader = DataLoader(val_dataset,batch_size=batch_size, shuffle=shuffle,num_workers=0)
         else:
             self.dataloader = DataLoader(dataset,batch_size=batch_size, shuffle=shuffle,num_workers=0)
         return self.dataloader
 
-    # def load_dataset(self, data_path, batch_size=32,shuffle=True,batch_mode=False,label_column=-1,transform=None,color="RGB",**kw ):
-        # from .load_data import ImageFolderDataset
-        # from torch.utils.data import DataLoader
-
-        # if data_type == 'tabular':
-        #     dataset = ""
-        # elif data_type =="image_folder":
-        #     dataset = ImageFolderDataset(data_path, transform=transform,color=color, batch_mode=batch_mode)
-        # elif data_type == "custom":
-        #     dataset = ""
-        # else:
-        #     raise ValueError(f"Unsupported data_type: {data_type}")
-        # self.dataset_size = len(dataset)
-        # self.dataloader = DataLoader(dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
-        # return self.dataloader
-
     def load_dataset(self, x, y, **kw):
         if kw:
             if 'word2idx'  in kw:
                 print("载入词表")
                 self.word2idx = kw['word2idx']
                 self.idx2word = {v:k for k, v in self.word2idx.items()}
                 self.x = torch.from_numpy(x)
@@ -517,39 +500,39 @@
                 self.model.load_state_dict(torch.load(checkpoint)['state_dict'])
                         
             self.model.to(self.device)
 
             # 设置优化器
             optimizer = torch.optim.Adam(self.model.parameters(), lr = lr)
             # scheduler = torch.optim.lr_scheduler.CosineAnnealingLR(optimizer, T_max=150, eta_min=0)
-            scheduler = torch.optim.lr_sheduler.ReduceLROnPlateau(optimizer, mode='min', factor=0.1, patience=10,verbose=False, threshold=0.0001, threshold_mode='rel', cooldown=0, min_lr=0, eps=1e-08)
+            # scheduler = torch.optim.lr_sheduler.ReduceLROnPlateau(optimizer, mode='min', factor=0.1, patience=10,verbose=False, threshold=0.0001, threshold_mode='rel', cooldown=0, min_lr=0, eps=1e-08)
             # 设置损失函数
             criterion = torch.nn.CrossEntropyLoss()
 
             # 定义训练过程
             for epoch in range(epochs):
                 for batch_idx, (batch_x, batch_y) in enumerate(self.dataloader,0):
 
                     batch_x = batch_x.long().transpose(1, 0).contiguous()
                     batch_y = batch_y.long().transpose(1, 0).contiguous()
-
+                    # print(batch_x.shape, batch_y.shape)
                     batch_x = batch_x.to(self.device)
                     batch_y = batch_y.to(self.device)
                     output, _ = self.model(batch_x)
                     loss = criterion(output, batch_y.view(-1))
 
-                    if batch_idx % 900 == 0:
-                        print('Train Epoch: {} [{}/{} ({:.0f}%)]\tLoss: {:.6f}'.format(
+                    # if batch_idx % 900 == 0:
+                    print('Train Epoch: {} [{}/{} ({:.0f}%)]\tLoss: {:.6f}'.format(
                             epoch+1, batch_idx * len(batch_x[1]), len(self.dataloader.dataset),
                             100. * batch_idx / len(self.dataloader), loss.item()))
 
                     optimizer.zero_grad()
                     loss.backward()
                     optimizer.step()
-                    scheduler.step()
+                    # scheduler.step()
 
             # 保存模型
             print("保存模型中...")
 
             info = {
                 'meta':{
                     'tool':'BaseNN', 
@@ -582,15 +565,15 @@
                 print("保存模型{}成功！".format(filename))
 
         else: # 针对图像任务
             if checkpoint:
                 if not os.path.exists(checkpoint):
                     print("未找到{}文件！".format(checkpoint))
                     return 
-                self.model = torch.load(checkpoint)['state_dict']
+                self.model = torch.load(checkpoint,map_location=torch.device('cpu'))['state_dict']
             # import torch.utils.data as Data
             # dataset = Data.TensorDataset(self.x, self.y)
             # total = self.x.shape[0]
             # self.loader = Data.DataLoader(
             #     dataset=dataset,
             #     batch_size=int(total / batch_num),
             #     shuffle=True,
@@ -699,19 +682,19 @@
             torch.save(info,model_path)
             # torch.save([self.img_classes, self.model], model_path)
             print("保存模型{}成功！".format(model_path))
             return log
 
     def inference(self, data, show=False, checkpoint=None,hidden=None, label=False):
         if checkpoint is not None:
-            self.rnn = torch.load(checkpoint)['para']['rnn']
+            self.rnn = torch.load(checkpoint,map_location=torch.device('cpu'))['para']['rnn']
         if checkpoint:
-            self.model = torch.load(checkpoint)['state_dict']
+            self.model = torch.load(checkpoint,map_location=torch.device('cpu'))['state_dict']
             try:
-                self.img_classes = torch.load(checkpoint)['meta']['CLASSES']
+                self.img_classes = torch.load(checkpoint,map_location=torch.device('cpu'))['meta']['CLASSES']
             except:
                 pass
         if self.rnn:
             self.word2idx = torch.load(checkpoint)['meta']['word2idx']
             self.ix2word = {v:k for k, v in self.word2idx.items()}
             config = torch.load(checkpoint)['para']['config']
             self.model =  lstm(len(self.word2idx),config['para']['ed'],config['para']['hd'],config['para']['nl'])
@@ -732,24 +715,26 @@
                         data  = Variable(torch.tensor(np.array(x)).to(torch.float32)).to(self.device)
                     else: # 有标签
                         x = np.loadtxt(data, dtype=float, delimiter=',',skiprows=1)
                         data = x[:, :-1]
                         data  = Variable(torch.tensor(np.array(data)).to(torch.float32)).to(self.device)
                 elif file_type.lower() in ["jpg", "png", "jpeg"]:  # 推理图片
                     # img = cv2.imread(data)
-                    color = torch.load(checkpoint)['meta']['color']
+                    color = torch.load(checkpoint,map_location=torch.device('cpu'))['meta']['color']
                     if color == "grayscale":
                         img = cv2.imread(data,cv2.IMREAD_GRAYSCALE)
                         img = np.expand_dims(img, 2)                 
                     else:
                         img = cv2.imread(data)
                     # img = np.array(Image.open(data))
-                    transform = torch.load(checkpoint)['meta']['transform']
+                    transform = torch.load(checkpoint,map_location=torch.device('cpu'))['meta']['transform']
+                    print(img.shape,"+++")
                     if transform is not None:
                         img = np.array(transform(Image.fromarray(img)))
+                        print(img.shape)
                     data = torch.from_numpy(img).unsqueeze(0).permute(0,3,1,2).to(torch.float32).to(self.device) 
 
                     # if len(img.shape) == 2:
                     #     # 灰度，加两维度（sample，channel）
                     #     data = torch.from_numpy(img).unsqueeze(0).unsqueeze(0).to(torch.float32).to(self.device) 
                     # elif len(img.shape) == 3:
                     #     # 灰度/RGB，加一维度（sample）
@@ -761,25 +746,25 @@
                     img_list = []
                     dir_list = os.listdir(data)
                     # print(dir_list)
                     # 将顺序读取的文件保存到该list中
                     for item in dir_list:
                         img_path = os.path.join(data,item)
                         # img = np.array(Image.open(img_path))
-                        color = torch.load(checkpoint)['meta']['color']
+                        color = torch.load(checkpoint,map_location=torch.device('cpu'))['meta']['color']
                         if color == "grayscale":
                             img = cv2.imread(img_path,cv2.IMREAD_GRAYSCALE)
                             img = np.expand_dims(img, 2)                 
 
                         else:
                             img = cv2.imread(img_path)
                         # if len(img.shape) == 2:
                         #     # 灰度，加1维度（channel）
                         #     img = np.expand_dims(img, 0)                 
-                        transform = torch.load(checkpoint)['meta']['transform']
+                        transform = torch.load(checkpoint,map_location=torch.device('cpu'))['meta']['transform']
                         if transform is not None:
                             img = np.array(transform(Image.fromarray(img)))
                         img_list.append(img)
                     
                     data = torch.from_numpy(np.array(img_list)).permute(0,3,1,2).to(torch.float32).to(self.device) 
                     # x = np.expand_dims(x, axis=1)
             elif isinstance(data, DataLoader):  # 推理dataloader
@@ -795,18 +780,23 @@
                 res = res.cpu().detach().numpy()
                 if show:
                     print("推理结果为：",res)
                 self. res = res
                 return res
 
             else:  # 推理numpy数组
-                data  = Variable(torch.tensor(np.array(data)).to(torch.float32)).to(self.device)
+                transform = torch.load(checkpoint,map_location=torch.device('cpu'))['meta']['transform']
+                if transform is not None:
+                    data = np.array(transform(Image.fromarray(data)))
+                # data  = Variable(torch.tensor(np.array(data)).to(torch.float32)).to(self.device)
+                data = torch.from_numpy(data).unsqueeze(0).permute(0,3,1,2).to(torch.float32).to(self.device) 
+
             # print(data.shape)
             # data  = Variable(torch.tensor(np.array(data)))
-
+            self.model = self.model.to(self.device)
             self.model.eval()
             with torch.no_grad():
                 res = self.model(data)
             res = res.cpu().detach().numpy()
             if show:
                 print("推理结果为：",res)
             self. res = res
@@ -814,15 +804,15 @@
     
     def _inference(self, data, show=False, checkpoint=None,hidden=None):
         data = data.to(self.device)
 
         if checkpoint and self.device== torch.device('cpu'):
             self.model.load_state_dict(torch.load(checkpoint,map_location=torch.device('cpu'))[1])
         elif checkpoint:
-            sta = torch.load(checkpoint)['state_dict']
+            sta = torch.load(checkpoint,map_location=torch.device('cpu'))['state_dict']
             self.model.load_state_dict(sta)
 
         output, hidden = self.model(data, hidden)
         return output, hidden
     
     def print_model(self):
         # print('模型共{}层'.format(self.layers_num))
@@ -832,15 +822,15 @@
         print("保存模型中...")
         torch.save(self.model, model_path)
         print("保存模型{}成功！".format(model_path))
     
     def load(self,model_path):
         print("载入模型中...")
         # self.model = torch.load(model_path)
-        self.model = torch.load(model_path)['state_dict']
+        self.model = torch.load(model_path,map_location=torch.device('cpu'))['state_dict']
 
         print("载入模型{}成功！".format(model_path))
 
     def print_result(self, result=None):
         res_idx = self.res.argmax(axis=1)
         res = {}
         for i,idx in enumerate(res_idx):
```

### Comparing `BaseNN-0.1.6/BaseNN/examples/BaseNN_demo.py` & `BaseNN-0.1.7/BaseNN/examples/BaseNN_demo.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # import torch
 import numpy as np
 import cv2
 import os
 
 def cal_accuracy(y, pred_y):
     res = pred_y.argmax(axis=1)
+    print(res, y)
     tp = np.array(y)==np.array(res)
     acc = np.sum(tp)/ y.shape[0]
     return acc
 
 def read_data(path):
     data = []
     label = []
@@ -354,35 +355,38 @@
     result = model.inference(data=a, checkpoint="new_mn_ckpt/basenn.pth")
     model.print_result()
 
 def load_image_data_cd():
     from torchvision.transforms import transforms
     model = nn()
     # model.set_seed(123465)
-    tran = transforms.Resize([128,128])
-    classes = {0:"cat", 1:"dog"}
-    d = model.load_img_data("/home/user/桌面/BaseNN004/dataset/cls/cats_dogs_dataset/CatsDogs (1)/CatsDogs/training_set",
-                             color="RGB",batch_size=1000, transform=tran,classes=classes)
-    # # for x, y in d:
-    # #     print(x.shape)
-    model.add('Conv2D', size=(3, 6),kernel_size=( 5, 5), activation='ReLU') # 60000 * 3456(6 * 24 * 24)
-    model.add('AvgPool', kernel_size=(2,2)) # 60000 * 864(6 * 12 * 12)
-    model.add('Conv2D', size=(6, 16), kernel_size=(5, 5), activation='ReLU') # 60000 * 1024(16 * 8 * 8)
-    model.add('AvgPool', kernel_size=(2,2)) # 60000 * 256(16 * 4 * 4)
-    model.add('Linear', size=(13456, 120), activation='ReLU')  # 60000 * 256
-    model.add('Linear', size=(120, 84), activation='ReLU') 
-    model.add('Linear', size=(84, 10), activation='Softmax')
-    model.add(optimizer='SGD')
-    model.save_fold = 'new_cd_ckpt'
-    model.train(lr=0.01, epochs=10) # 直接训练
+    # tran = transforms.Resize([128,128])
+    # classes = {0:"cat", 1:"dog"}
+    # d = model.load_img_data("/home/user/桌面/BaseNN004/dataset/cls/cats_dogs_dataset/CatsDogs (1)/CatsDogs/training_set",
+    #                          color="RGB",batch_size=1000, transform=tran,classes=classes)
+    # # # for x, y in d:
+    # # #     print(x.shape)
+    # model.add('Conv2D', size=(3, 6),kernel_size=( 5, 5), activation='ReLU') # 60000 * 3456(6 * 24 * 24)
+    # model.add('AvgPool', kernel_size=(2,2)) # 60000 * 864(6 * 12 * 12)
+    # model.add('Conv2D', size=(6, 16), kernel_size=(5, 5), activation='ReLU') # 60000 * 1024(16 * 8 * 8)
+    # model.add('AvgPool', kernel_size=(2,2)) # 60000 * 256(16 * 4 * 4)
+    # model.add('Linear', size=(13456, 120), activation='ReLU')  # 60000 * 256
+    # model.add('Linear', size=(120, 84), activation='ReLU') 
+    # model.add('Linear', size=(84, 10), activation='Softmax')
+    # model.add(optimizer='SGD')
+    # model.save_fold = 'new_cd_ckpt'
+    # model.train(lr=0.01, epochs=10) # 直接训练
     # test_x, y = read_data("../../dataset/cls/mnist/val_set")
     # print(y[1000:1100])
     a = "/home/user/桌面/BaseNN004/dataset/cls/cats_dogs_dataset/CatsDogs (1)/CatsDogs/val_set/dog"
     b = "/home/user/桌面/BaseNN004/dataset/cls/cats_dogs_dataset/CatsDogs (1)/CatsDogs/val_set/dog/dog0.jpg"
-    result = model.inference(data=b, checkpoint="new_cd_ckpt/basenn.pth")
+    from PIL import Image
+    im = Image.open(b)
+    bb = np.array(im)
+    result = model.inference(data=bb, checkpoint="new_cd_ckpt/basenn.pth")
     model.print_result()
 
 def load_tab_data_iris():
     import time
     model = nn()
     # 训练数据
     train_path = '../../dataset/iris/iris_training.csv'
@@ -442,33 +446,81 @@
     model.train(lr=0.01, epochs=10,loss="BCELoss",metrics=[])
 
     res = model.inference(test_x, checkpoint="action_ckpt2/basenn.pth")
     print(test_y)
     print(res)
     model.print_result()
 
+def load_npz_data_tang():
+    # 读取数据
+    # datas = np.load('tang.npz',allow_pickle=True)
+    # data = datas['data'] 
+    # # print("第一条数据：",data[0]) # 观察第一条数据
+    # word2ix = datas['word2ix'].item() # 汉字对应的索引
+    # print(data.shape)
+    # # print(datas["word2idx"])
+    # x, y = data[:,:-1], data[:, 1:]
+
+    # np.savez("tangccc.npz", data=x, label=y, word2idx=word2ix)
+
+    # print("词表:",word2ix) 
+    # ix2word = datas['ix2word'].item() # 索引对应的汉字
+
+    model = nn()
+    # model.load_dataset(x, y, word2idx=word2ix) # 载入数据
+    model.load_npz_data('tangccc.npz', batch_size=128)
+    model.add('em_LSTM', size=(128,256),num_layers=2) 
+    model.save_fold = '111ckpt'
+    model.train(lr=0.005, epochs=3,checkpoint='111ckpt/basenn.pth')
+
+def tang_infer():
+    from BaseNN import nn
+    model = nn()
+
+    input = '长'
+    checkpoint = '111ckpt/basenn.pth'
+    output, hidden = model.inference(data=input,checkpoint=checkpoint) # output是多维向量，接下来转化为汉字
+    print("output: ",output)
+    index = np.argmax(output) # 找到概率最大的字的索引
+    w = model.ix2word[index] # 根据索引从词表中找到字
+    print("word:",w)
+
+def txt2npz():
+    with open("tang.txt","r",encoding='utf-8') as f:
+        data = f.readlines()
+        data = [i.rstrip('\n') for i in data]
+        word2ix = {}
+        index = 1
+        for line in data:
+            for word in line:
+                pass
+        print(type(data),data)
+
 if __name__=="__main__":
+    # load_npz_data_action()
+    # load_npz_data_tang()
+    # tang_infer()
+    # txt2npz()
     # action_demo()
     # user_defined_demo()
     # data_define_demo()
     # normal_train_demo()
     # pth_info('iris_ckpt/basenn.pth')
     # only_infer_demo()
     # continue_train_demo()
     # iris_train_test()
 
     # mnist_train()
     # pth_info('mn_ckpt/basenn.pth')
-    # mnist_test(True)
+    # mnist_test(False)
 
     # infer_9_demo()
     # visual_feature_demo()
     # extract_feature_demo()
 
     # lstm_train_demo()
     # pth_info('model_lstm.pth')
     # lstm_infer_demo()
 
     # load_image_data_mn()
-    # load_image_data_cd()
-    load_tab_data_iris()
-    # load_npz_data_action()
+    load_image_data_cd()
+    # load_tab_data_iris()
```

### Comparing `BaseNN-0.1.6/BaseNN/examples/pkl2pth.py` & `BaseNN-0.1.7/BaseNN/examples/pkl2pth.py`

 * *Files identical despite different names*

### Comparing `BaseNN-0.1.6/BaseNN/load_data.py` & `BaseNN-0.1.7/BaseNN/load_data.py`

 * *Files identical despite different names*

### Comparing `BaseNN-0.1.6/BaseNN/version.py` & `BaseNN-0.1.7/BaseNN/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-__version__='0.1.6'
+__version__='0.1.7'
 __path__=os.path.abspath(os.getcwd())
 
 def parse_version_info(version_str):
     version_info = []
     for x in version_str.split('.'):
         if x.isdigit():
             version_info.append(int(x))
```

### Comparing `BaseNN-0.1.6/setup.py` & `BaseNN-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     packages = list(gen_packages_items())
     return packages
 
 
 setup(
     name='BaseNN',
-    version='0.1.6',
+    version='0.1.7',
     description='BaseNN can easily build neural networks layer by layer and deeply explore the neural network principle.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
     include_package_data=True,
```

