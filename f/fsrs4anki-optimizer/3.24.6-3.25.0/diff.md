# Comparing `tmp/fsrs4anki_optimizer-3.24.6.tar.gz` & `tmp/fsrs4anki_optimizer-3.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-3.24.6.tar", last modified: Sat Jun 17 13:25:42 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-3.25.0.tar", last modified: Sun Jun 18 15:19:45 2023, max compression
```

## Comparing `fsrs4anki_optimizer-3.24.6.tar` & `fsrs4anki_optimizer-3.25.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:25:42.478803 fsrs4anki_optimizer-3.24.6/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-17 13:25:42.478803 fsrs4anki_optimizer-3.24.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:25:42.478803 fsrs4anki_optimizer-3.24.6/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-17 13:25:33.000000 fsrs4anki_optimizer-3.24.6/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-17 13:25:33.000000 fsrs4anki_optimizer-3.24.6/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43667 2023-06-17 13:25:33.000000 fsrs4anki_optimizer-3.24.6/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:25:42.478803 fsrs4anki_optimizer-3.24.6/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-17 13:25:42.000000 fsrs4anki_optimizer-3.24.6/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-17 13:25:42.000000 fsrs4anki_optimizer-3.24.6/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 13:25:42.000000 fsrs4anki_optimizer-3.24.6/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-17 13:25:42.000000 fsrs4anki_optimizer-3.24.6/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-17 13:25:42.000000 fsrs4anki_optimizer-3.24.6/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-17 13:25:33.000000 fsrs4anki_optimizer-3.24.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 13:25:42.478803 fsrs4anki_optimizer-3.24.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-17 13:25:33.000000 fsrs4anki_optimizer-3.24.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:19:45.202244 fsrs4anki_optimizer-3.25.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-18 15:19:45.202244 fsrs4anki_optimizer-3.25.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:19:45.202244 fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-18 15:19:35.000000 fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-18 15:19:35.000000 fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43747 2023-06-18 15:19:35.000000 fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:19:45.202244 fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-18 15:19:45.000000 fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-18 15:19:45.000000 fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 15:19:45.000000 fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-18 15:19:45.000000 fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-18 15:19:45.000000 fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-18 15:19:35.000000 fsrs4anki_optimizer-3.25.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 15:19:45.202244 fsrs4anki_optimizer-3.25.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-18 15:19:35.000000 fsrs4anki_optimizer-3.25.0/setup.py
```

### Comparing `fsrs4anki_optimizer-3.24.6/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-3.24.6/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-3.25.0/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         self.batch_nums = len(self.batch_indices)
         # seed = int(torch.empty((), dtype=torch.int64).random_().item())
         seed = 2023
         self.generator = torch.Generator()
         self.generator.manual_seed(seed)
 
     def __iter__(self):
-        yield from [self.batch_indices[idx] for idx in torch.randperm(self.batch_nums, generator=self.generator).tolist()]
+        yield from (self.batch_indices[idx] for idx in torch.randperm(self.batch_nums, generator=self.generator).tolist())
 
     def __len__(self):
         return len(self.data_source)
 
 
 def collate_fn(batch):
     sequences, delta_ts, labels, seq_lens = zip(*batch)
@@ -561,15 +561,15 @@
         base = 1.01
         index_len = 664
         index_offset = 200
         d_range = 10
         d_offset = 1
         r_time = 8
         f_time = 25
-        max_time = 200000
+        max_time = 1e10
 
         type_block = dict()
         type_count = dict()
         type_time = dict()
         last_t = self.type_sequence[0]
         type_block[last_t] = 1
         type_count[last_t] = 1
@@ -586,15 +586,15 @@
         if 2 in type_count and 2 in type_block:
             f_time = round(type_time[2]/type_block[2]/1000 + r_time, 1)
 
         print(f"average time for failed cards: {f_time}s")
         print(f"average time for recalled cards: {r_time}s")
 
         def stability2index(stability):
-            return int(round(np.log(stability) / np.log(base)) + index_offset)
+            return (np.log(stability) / np.log(base)).round().astype(int) + index_offset
 
         def init_stability(d):
             return max(((d - self.w[2]) / self.w[3] + 2) * self.w[1] + self.w[0], np.power(base, -index_offset))
 
         def cal_next_recall_stability(s, r, d, response):
             if response == 1:
                 return s * (1 + np.exp(self.w[6]) * (11 - d) * np.power(s, self.w[7]) * (np.exp((1 - r) * self.w[8]) - 1))
@@ -610,31 +610,32 @@
             recall = percentage / 100
             time_list = np.zeros((d_range, index_len))
             time_list[:,:-1] = max_time
             for d in range(d_range, 0, -1):
                 s0 = init_stability(d)
                 s0_index = stability2index(s0)
                 diff = max_time
-                while diff > 0.1:
+                while diff > 1:
+                    total_time = time_list[d - 1].sum()
+                    s_indices = np.arange(index_len - 2, -1, -1)
+                    stabilities = stability_list[s_indices]
+                    intervals = np.maximum(1, np.round(stabilities * np.log(recall) / np.log(0.9)))
+                    p_recalls = np.power(0.9, intervals / stabilities)
+                    recall_s = cal_next_recall_stability(stabilities, p_recalls, d, 1)
+                    forget_d = np.minimum(d + d_offset, 10)
+                    forget_s = cal_next_recall_stability(stabilities, p_recalls, forget_d, 0)
+                    recall_s_indices = np.minimum(stability2index(recall_s), index_len - 1)
+                    forget_s_indices = np.clip(stability2index(forget_s), 0, index_len - 1)
+                    recall_times = time_list[d - 1][recall_s_indices] + r_time
+                    forget_times = time_list[forget_d - 1][forget_s_indices] + f_time
+                    exp_times = p_recalls * recall_times + (1.0 - p_recalls) * forget_times
+                    mask = exp_times < time_list[d - 1][s_indices]
+                    time_list[d - 1][s_indices[mask]] = exp_times[mask]
+                    diff = total_time - time_list[d - 1].sum()
                     s0_time = time_list[d - 1][s0_index]
-                    for s_index in range(index_len - 2, -1, -1):
-                        stability = stability_list[s_index];
-                        interval = max(1, round(stability * np.log(recall) / np.log(0.9)))
-                        p_recall = np.power(0.9, interval / stability)
-                        recall_s = cal_next_recall_stability(stability, p_recall, d, 1)
-                        forget_d = min(d + d_offset, 10)
-                        forget_s = cal_next_recall_stability(stability, p_recall, forget_d, 0)
-                        recall_s_index = min(stability2index(recall_s), index_len - 1)
-                        forget_s_index = min(max(stability2index(forget_s), 0), index_len - 1)
-                        recall_time = time_list[d - 1][recall_s_index] + r_time
-                        forget_time = time_list[forget_d - 1][forget_s_index] + f_time
-                        exp_time = p_recall * recall_time + (1.0 - p_recall) * forget_time
-                        if exp_time < time_list[d - 1][s_index]:
-                            time_list[d - 1][s_index] = exp_time
-                    diff = s0_time - time_list[d - 1][s0_index]
                 df.loc[0 if pd.isnull(df.index.max()) else df.index.max() + 1] = [recall, d, s0_time]
 
         df.sort_values(by=["difficulty", "retention"], inplace=True)
         df.to_csv("./expected_time.csv", index=False)
         print("expected_time.csv saved.")
 
         optimal_retention_list = np.zeros(10)
```

