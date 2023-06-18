# Comparing `tmp/HandGestureRec-0.1.5.tar.gz` & `tmp/HandGestureRec-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HandGestureRec-0.1.5.tar", last modified: Thu Jun 15 19:48:08 2023, max compression
+gzip compressed data, was "HandGestureRec-0.1.6.tar", last modified: Sat Jun 17 19:41:35 2023, max compression
```

## Comparing `HandGestureRec-0.1.5.tar` & `HandGestureRec-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ahmadbodayr   (501) staff       (20)        0 2023-06-15 19:48:08.590620 HandGestureRec-0.1.5/
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1069 2023-06-13 20:47:04.000000 HandGestureRec-0.1.5/LICENSE
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2926 2023-06-15 19:48:08.590474 HandGestureRec-0.1.5/PKG-INFO
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2601 2023-06-15 19:26:27.000000 HandGestureRec-0.1.5/README.md
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)       38 2023-06-15 19:48:08.590656 HandGestureRec-0.1.5/setup.cfg
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1175 2023-06-15 19:46:33.000000 HandGestureRec-0.1.5/setup.py
-drwxr-xr-x   0 ahmadbodayr   (501) staff       (20)        0 2023-06-15 19:48:08.589584 HandGestureRec-0.1.5/src/
-drwxr-xr-x   0 ahmadbodayr   (501) staff       (20)        0 2023-06-15 19:48:08.590302 HandGestureRec-0.1.5/src/HandGestureRec.egg-info/
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2926 2023-06-15 19:48:08.000000 HandGestureRec-0.1.5/src/HandGestureRec.egg-info/PKG-INFO
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)      412 2023-06-15 19:48:08.000000 HandGestureRec-0.1.5/src/HandGestureRec.egg-info/SOURCES.txt
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)        1 2023-06-15 19:48:08.000000 HandGestureRec-0.1.5/src/HandGestureRec.egg-info/dependency_links.txt
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)       48 2023-06-15 19:48:08.000000 HandGestureRec-0.1.5/src/HandGestureRec.egg-info/entry_points.txt
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)       67 2023-06-15 19:48:08.000000 HandGestureRec-0.1.5/src/HandGestureRec.egg-info/requires.txt
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)       83 2023-06-15 19:48:08.000000 HandGestureRec-0.1.5/src/HandGestureRec.egg-info/top_level.txt
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)    11233 2023-06-13 18:28:48.000000 HandGestureRec-0.1.5/src/MLScript.py
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     3457 2023-06-15 19:43:15.000000 HandGestureRec-0.1.5/src/main.py
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2797 2023-06-15 19:43:15.000000 HandGestureRec-0.1.5/src/mainView.py
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1582 2023-06-15 19:43:15.000000 HandGestureRec-0.1.5/src/modelTestingView.py
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     4213 2023-06-15 19:43:15.000000 HandGestureRec-0.1.5/src/myDataSetsView.py
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1303 2023-06-15 19:43:15.000000 HandGestureRec-0.1.5/src/myGesturesView.py
--rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2555 2023-06-15 19:43:15.000000 HandGestureRec-0.1.5/src/myModelsView.py
+drwxr-xr-x   0 ahmadbodayr   (501) staff       (20)        0 2023-06-17 19:41:35.989649 HandGestureRec-0.1.6/
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1069 2023-06-13 20:47:04.000000 HandGestureRec-0.1.6/LICENSE
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2984 2023-06-17 19:41:35.989505 HandGestureRec-0.1.6/PKG-INFO
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2659 2023-06-17 19:40:44.000000 HandGestureRec-0.1.6/README.md
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)       38 2023-06-17 19:41:35.989690 HandGestureRec-0.1.6/setup.cfg
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1175 2023-06-17 19:37:34.000000 HandGestureRec-0.1.6/setup.py
+drwxr-xr-x   0 ahmadbodayr   (501) staff       (20)        0 2023-06-17 19:41:35.988161 HandGestureRec-0.1.6/src/
+drwxr-xr-x   0 ahmadbodayr   (501) staff       (20)        0 2023-06-17 19:41:35.989326 HandGestureRec-0.1.6/src/HandGestureRec.egg-info/
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2984 2023-06-17 19:41:35.000000 HandGestureRec-0.1.6/src/HandGestureRec.egg-info/PKG-INFO
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)      412 2023-06-17 19:41:35.000000 HandGestureRec-0.1.6/src/HandGestureRec.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)        1 2023-06-17 19:41:35.000000 HandGestureRec-0.1.6/src/HandGestureRec.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)       48 2023-06-17 19:41:35.000000 HandGestureRec-0.1.6/src/HandGestureRec.egg-info/entry_points.txt
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)       67 2023-06-17 19:41:35.000000 HandGestureRec-0.1.6/src/HandGestureRec.egg-info/requires.txt
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)       83 2023-06-17 19:41:35.000000 HandGestureRec-0.1.6/src/HandGestureRec.egg-info/top_level.txt
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)    11687 2023-06-17 19:35:44.000000 HandGestureRec-0.1.6/src/MLScript.py
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     3457 2023-06-15 19:43:15.000000 HandGestureRec-0.1.6/src/main.py
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     2797 2023-06-16 18:11:02.000000 HandGestureRec-0.1.6/src/mainView.py
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1582 2023-06-16 18:11:02.000000 HandGestureRec-0.1.6/src/modelTestingView.py
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     5007 2023-06-16 18:11:02.000000 HandGestureRec-0.1.6/src/myDataSetsView.py
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     1935 2023-06-16 18:11:02.000000 HandGestureRec-0.1.6/src/myGesturesView.py
+-rw-r--r--   0 ahmadbodayr   (501) staff       (20)     3159 2023-06-16 18:11:02.000000 HandGestureRec-0.1.6/src/myModelsView.py
```

### Comparing `HandGestureRec-0.1.5/LICENSE` & `HandGestureRec-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `HandGestureRec-0.1.5/PKG-INFO` & `HandGestureRec-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: HandGestureRec
-Version: 0.1.5
+Version: 0.1.6
 Summary: Dynamic hand gesture detection library using ML.
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HandGestureRec
 # Short Summary:
- ## The library is open source  https://github.com/AhmadBodayr/HandGestureRec 
-This is a dynamic hand gesture detection library, the user can interact with the library using a GUI built using Tkinter.
+The library is an open source dynamic hand gesture recognition built using python with a Tkinter GUI and ML. using Tensorflow, Keras Api for TF, OpneCV for camera access and MediaPipe for hand landmarks detection https://github.com/AhmadBodayr/HandGestureRec
 ## Implementation: 
 The library uses the webcam as the sensor and it gives the user access to the webcam using opencv, then the handlandmarks are collected using MediaPipe.
 ## GUI:
 The GUI is the main way for the user to interact with the toolkit. It is written in Tkinter for python wich is the default GUI library for Python. The GUI is simple and easy to use.
 ## The Backend:
 It is comprised of:
 ### Data Collection:
```

### Comparing `HandGestureRec-0.1.5/README.md` & `HandGestureRec-0.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # HandGestureRec
 # Short Summary:
- ## The library is open source  https://github.com/AhmadBodayr/HandGestureRec 
-This is a dynamic hand gesture detection library, the user can interact with the library using a GUI built using Tkinter.
+The library is an open source dynamic hand gesture recognition built using python with a Tkinter GUI and ML. using Tensorflow, Keras Api for TF, OpneCV for camera access and MediaPipe for hand landmarks detection https://github.com/AhmadBodayr/HandGestureRec
 ## Implementation: 
 The library uses the webcam as the sensor and it gives the user access to the webcam using opencv, then the handlandmarks are collected using MediaPipe.
 ## GUI:
 The GUI is the main way for the user to interact with the toolkit. It is written in Tkinter for python wich is the default GUI library for Python. The GUI is simple and easy to use.
 ## The Backend:
 It is comprised of:
 ### Data Collection:
```

### Comparing `HandGestureRec-0.1.5/setup.py` & `HandGestureRec-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     else:
         tfversion = "tensorflow"
         
 setup(
     long_description=long_description, 
     long_description_content_type="text/markdown",
     name='HandGestureRec',
-    version='0.1.5',
+    version='0.1.6',
     description='Dynamic hand gesture detection library using ML.',
     packages=find_packages(),
     py_modules=[
         "main",
         "MLScript",
         "mainView",
         "modelTestingView",
```

### Comparing `HandGestureRec-0.1.5/src/HandGestureRec.egg-info/PKG-INFO` & `HandGestureRec-0.1.6/src/HandGestureRec.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: HandGestureRec
-Version: 0.1.5
+Version: 0.1.6
 Summary: Dynamic hand gesture detection library using ML.
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HandGestureRec
 # Short Summary:
- ## The library is open source  https://github.com/AhmadBodayr/HandGestureRec 
-This is a dynamic hand gesture detection library, the user can interact with the library using a GUI built using Tkinter.
+The library is an open source dynamic hand gesture recognition built using python with a Tkinter GUI and ML. using Tensorflow, Keras Api for TF, OpneCV for camera access and MediaPipe for hand landmarks detection https://github.com/AhmadBodayr/HandGestureRec
 ## Implementation: 
 The library uses the webcam as the sensor and it gives the user access to the webcam using opencv, then the handlandmarks are collected using MediaPipe.
 ## GUI:
 The GUI is the main way for the user to interact with the toolkit. It is written in Tkinter for python wich is the default GUI library for Python. The GUI is simple and easy to use.
 ## The Backend:
 It is comprised of:
 ### Data Collection:
```

### Comparing `HandGestureRec-0.1.5/src/MLScript.py` & `HandGestureRec-0.1.6/src/MLScript.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 from tensorflow.keras.utils import to_categorical
 from tensorflow.keras.callbacks import EarlyStopping
 from tensorflow.keras.optimizers.legacy import Adam
 from tensorflow.keras.utils import plot_model
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import multilabel_confusion_matrix, accuracy_score
 
+baseCounter = 0
+
 learning_rate = .001
 adam = Adam(learning_rate)
 # Setting up the learning rate
 # learning_rate = 0.0001 
 # adam = adam(learning_rate)
 
 possible = False
@@ -68,25 +70,37 @@
 
 # Videos are going to be 30 frames in length
 sequence_length = 30
 
 action = ""
 X = np.array([])
 y = np.array([])
-
 mp_holistic = mp.solutions.holistic 
 mp_drawing = mp.solutions.drawing_utils
 mp_holistic = mp.solutions.holistic
 
 # Get the absolute path of the directory containing this script
 script_dir = os.path.dirname(os.path.abspath(__file__))
 
 # Construct the path to the holistic model file
 model_path = os.path.join(script_dir, 'models', 'holistic.pb')
 
+
+# Early stopping class
+class earlyStop(tf.keras.callbacks.Callback):
+    def on_epoch_end(self, epoch, logs=None):
+        global baseCounter
+        if logs.get("categorical_accuracy") > 0.9:
+            if baseCounter == 3:
+                self.model.stop_training = True
+            else:
+                baseCounter += 1
+        else:
+            baseCounter = 0
+
 # definning gesture /////////////////
 def define_gestures(gesture):
     global action
     global result_mapa
     global result_helper
     action = gesture
     print("Gesture defined successfully")
@@ -148,24 +162,25 @@
     for sequence in range(no_sequences):
         try: 
             os.makedirs(os.path.join(DATA_PATH, action, str(sequence)))
         except:
             pass     
     print("Folders created successfully")
 
-# The camera loop for data gathering ------------------------------------
+# The camera loop for data gathering
 def data_collection_cam_loop():
     global action
     global sequences
     global sequence_length
     global DATA_PATH
+    sequence_length = 30
     print("Started Collecting data")
     cap = cv2.VideoCapture(0)
     # Set mediapipe model 
-    with mp_holistic.Holistic(min_detection_confidence=0.5, min_tracking_confidence=0.5) as holistic:
+    with mp_holistic.Holistic(min_detection_confidence=0.5, min_tracking_confidence=0.8) as holistic:
         for sequence in range(no_sequences):
             for frame_num in range(sequence_length):
                 # Read feed
                 ret, frame = cap.read()
                 # Make detections
                 image, results = mediapipe_detection(frame, holistic)
                 # Draw landmarks
@@ -193,30 +208,31 @@
                     break
     cap.release()
     cv2.destroyAllWindows()
     cv2.waitKey(1)
 
 
 
-# Building the input data and label and making the   ///////////////////////////////
+# Building the input data and labels
 def build_data_and_labels(selectedSet):
     global DATA_PATH2
     global sequences
     global sequence_length
     global labels
     global possible
     global X
-    global y
+    global y   
     global actions
     # Building the data and labels
     temp = []
     for entry in os.scandir(os.path.join(DATA_PATH2, selectedSet)):
         if entry.is_dir():
             temp.append(entry.name)
     actions = np.array(temp)
+    actions.sort()
     label_map = {label:num for num, label in enumerate(actions)}
     for action in actions:
         for sequence in os.listdir(os.path.join(DATA_PATH2, selectedSet, action)):
             if sequence != '.DS_Store':
                 sequence_int = int(sequence)
                 window = []
                 for frame_num in range(sequence_length):
@@ -224,63 +240,64 @@
                     window.append(res)
                 window = np.array(window)
                 sequences.append(window)
                 labels.append(label_map[action])
     # Setting up the data and labels
     X = np.array(sequences)
     y = to_categorical(labels).astype(int)
-    # Making the train/test split
     possible = True
     print(" Training and testing tesnsors are ready!!!")
 
 # Building the ML model
 def build_ML_model(modelName):
     global possible
     global X
-    global y 
+    global y
     global DATA_PATH3   
     global model
     global adam
+    global baseCounter
     global actions
     if possible == False:
         print("Error: Cant build the model yet, data not ready")
         return
-    
+    baseCounter = 0
     model = Sequential()
     model.add(LSTM(64, return_sequences=True, activation='relu'))
     model.add(LSTM(128, return_sequences=True, activation='relu'))
     model.add(LSTM(64, return_sequences=False, activation='relu'))
     model.add(Dense(64, activation='relu'))
     model.add(Dense(32, activation='relu'))
     model.add(Dense(actions.shape[0], activation='softmax'))
-    # Compiling the model
-    model.compile(optimizer=adam ,loss='categorical_crossentropy', metrics=['accuracy'])
+    # Compilling the model
+    model.compile(optimizer=adam, loss='categorical_crossentropy', metrics=['categorical_accuracy'])
     # Fitting the model
-    model.fit(X, y, epochs=50)
+    model.fit(X, y, epochs=500, callbacks=[earlyStop()])
+    # Saving the model
     model.save(os.path.join(DATA_PATH3, modelName))
     print("Model finished training successfully!")
 
 def realtime_testing(modelName):
+    # actions dont forget
     global sequence_length
     global DATA_PATH3
     temp = []
     for entry in os.scandir(os.path.join(DATA_PATH2, modelName)):
         if entry.is_dir():
             temp.append(entry.name)
     newActions = np.array(temp)
-    
-
+    newActions.sort()
     loadedModel = tf.keras.models.load_model(os.path.join(DATA_PATH3, modelName))
     # The sequence of frames
     sequence = []
     # The prediction thresh hold 
-    threshold = .75
+    threshold = .90
     # Screen video capture and realtime detection
     cap = cv2.VideoCapture(0)
-    with mp_holistic.Holistic(min_detection_confidence=0.5, min_tracking_confidence=0.5) as holistic:
+    with mp_holistic.Holistic(min_detection_confidence=0.5, min_tracking_confidence=0.8) as holistic:
         while cap.isOpened():
             # Read feed
             ret, frame = cap.read()
             # Make detections
             image, results = mediapipe_detection(frame, holistic)
             # Draw landmarks
             draw_landmarks(image, results)
```

### Comparing `HandGestureRec-0.1.5/src/main.py` & `HandGestureRec-0.1.6/src/main.py`

 * *Files identical despite different names*

### Comparing `HandGestureRec-0.1.5/src/mainView.py` & `HandGestureRec-0.1.6/src/mainView.py`

 * *Files identical despite different names*

### Comparing `HandGestureRec-0.1.5/src/modelTestingView.py` & `HandGestureRec-0.1.6/src/modelTestingView.py`

 * *Files identical despite different names*

### Comparing `HandGestureRec-0.1.5/src/myDataSetsView.py` & `HandGestureRec-0.1.6/src/myDataSetsView.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from tkinter import *
 import MLScript
 import shutil
 import mainView
 import os
 class MyDataSetsView(tk.Frame):
     back_button = None
-    
     definedGesturesBox = None
     selectedGesturesBox = None
     dataSetsBox = None
+    deleteDataset_button = None
     gestures_label = None
     dataSets_label = None
     addSelected_button = None
     delete_button = None
     createDataSet_button = None
     dataSetName_entry = None
 
@@ -43,19 +43,21 @@
         self.selectedGestures_label.pack()
         self.selectedGesturesBox.pack()
         self.name_label = tk.Label(self, text="Enter Your DataSet Name: ")
         self.name_label.pack(side=tk.LEFT)
         self.dataSetName_entry = tk.Entry(self)
         self.dataSetName_entry.pack(side=tk.LEFT)
         self.addSelected_button = tk.Button(self, text="Add Selected", font=("Arial",15), command=self.add_selected_items)
+        self.deleteDataset_button = tk.Button(self, text="Delete Dataset", font=("Arial",15), command=self.deleteDataset)
         self.back_button = tk.Button(self, text="Back", font=("Arial",15), command=self.backToMainView)
         self.createDataSet_button = tk.Button(self, text="create Dataset", font=("Arial",15), command=self.createDataSet)
         self.delete_button = tk.Button(self, text="Remove All", font=("Arial",15), command=self.emptySet)
         self.createDataSet_button.pack(side=tk.LEFT, pady=20)
         self.delete_button.pack(side=tk.LEFT, pady=20)
+        self.deleteDataset_button.pack(side=tk.LEFT, pady=20)
         self.addSelected_button.pack(side=tk.LEFT, pady=20)
         self.back_button.pack(side=tk.RIGHT)
         
        
 
     def backToMainView(self):
         self.pack_forget()
@@ -84,14 +86,26 @@
                 if os.path.isdir(src_dir):
                     shutil.copytree(src_dir, dest_dir)
                 else:
                     shutil.copy(src_dir, dest_dir)
             self.dataSetsBox.insert(tk.END, self.dataSetName_entry.get())
             self.dataSetName_entry.delete(0, tk.END)
             self.selectedGesturesBox.delete(0, tk.END) 
+    
+    def deleteDataset(self):
+        selected_index = self.dataSetsBox.curselection()
+        if selected_index:
+            modelName = self.dataSetsBox.get(selected_index)
+            self.dataSetsBox.delete(selected_index)
+            folder_to_delete1 = os.path.join(MLScript.DATA_PATH2, modelName)
+            folder_to_delete2 = os.path.join(MLScript.DATA_PATH3, modelName)
+            if os.path.exists(folder_to_delete1):
+                shutil.rmtree(folder_to_delete1)
+            if os.path.exists(folder_to_delete2):
+                shutil.rmtree(folder_to_delete2)
```

### Comparing `HandGestureRec-0.1.5/src/myModelsView.py` & `HandGestureRec-0.1.6/src/myModelsView.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 from tkinter import *
 import MLScript
 import shutil
 import mainView
 import os
 class MyModelsView(tk.Frame):
     back_button = None
+    deleteModel_button = None
     modelsBox = None
     dataSetsBox = None
     models_label = None
     dataSets_label = None
     createModel_button = None
     modelName_entry = None
 
     def __init__(self, parent):
         super().__init__(parent)
         self.parent = parent
         self.howTo = tk.Label(self, text="To create a model, select a predefined dataset then press create model", pady=10)
         self.howTo.pack()
         self.back_button = tk.Button(self, text="Back", font=("Arial",15), command=self.backToMainView)
+        self.deleteModel_button = tk.Button(self, text="Delete Model", font=("Arial",15), command=self.deleteModel)
         self.back_button.pack(side=tk.BOTTOM)
+        self.deleteModel_button.pack(side=tk.BOTTOM, pady=20)
         self.dataSetsBox = Listbox(self, selectmode=tk.SINGLE)
         self.modelsBox= Listbox(self)
         sets = os.listdir(MLScript.DATA_PATH2)
         models = os.listdir(MLScript.DATA_PATH3)
         self.dataSets_label = tk.Label(self, text="Defined DataSets")
         self.dataSets_label.pack()    
         folders = [item for item in sets if os.path.isdir(os.path.join(MLScript.DATA_PATH2, item))]
@@ -53,14 +56,23 @@
             self.creationInProgress_label = tk.Label(self, text="Creating your model this might take a few minutes !", font=("Arial", 25, "bold"), pady=10)
             self.creationInProgress_label.pack()
             selectedSet = self.dataSetsBox.get(selected_index)
             MLScript.build_data_and_labels(selectedSet)
             MLScript.build_ML_model(selectedSet)
             self.creationInProgress_label.pack_forget()
             self.modelsBox.insert(tk.END, selectedSet)
+    
+    def deleteModel(self):
+        selected_index = self.modelsBox.curselection()
+        if selected_index:
+            modelName = self.modelsBox.get(selected_index)
+            self.modelsBox.delete(selected_index)
+            folder_to_delete = os.path.join(MLScript.DATA_PATH3, modelName)
+            if os.path.exists(folder_to_delete):
+                shutil.rmtree(folder_to_delete)
```

