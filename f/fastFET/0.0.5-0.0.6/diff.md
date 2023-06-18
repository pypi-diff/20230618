# Comparing `tmp/fastFET-0.0.5.tar.gz` & `tmp/fastFET-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastFET-0.0.5.tar", last modified: Tue Mar 21 03:56:04 2023, max compression
+gzip compressed data, was "fastFET-0.0.6.tar", last modified: Sun Jun 18 13:47:46 2023, max compression
```

## Comparing `fastFET-0.0.5.tar` & `fastFET-0.0.6.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 hlei0     (1000) hlei0     (1000)        0 2023-03-21 03:56:04.790329 fastFET-0.0.5/
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)      187 2023-03-21 03:42:39.000000 fastFET-0.0.5/MANIFEST.in
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)    13262 2023-03-21 03:56:04.790329 fastFET-0.0.5/PKG-INFO
-drwxr-xr-x   0 hlei0     (1000) hlei0     (1000)        0 2023-03-21 03:56:04.750329 fastFET-0.0.5/fastFET/
-drwxr-xr-x   0 hlei0     (1000) hlei0     (1000)        0 2023-03-21 03:56:04.760329 fastFET-0.0.5/fastFET/BGPMAGNET/
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)     3102 2023-03-21 03:31:43.000000 fastFET-0.0.5/fastFET/BGPMAGNET/ProcessHandler.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)     3586 2023-03-21 03:31:44.000000 fastFET-0.0.5/fastFET/BGPMAGNET/README.md
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)        0 2023-03-21 03:31:43.000000 fastFET-0.0.5/fastFET/BGPMAGNET/__init__.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)     6482 2023-03-21 03:31:44.000000 fastFET-0.0.5/fastFET/BGPMAGNET/base.py
-drwxr-xr-x   0 hlei0     (1000) hlei0     (1000)        0 2023-03-21 03:56:04.780329 fastFET-0.0.5/fastFET/BGPMAGNET/bgpparser/
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)        0 2023-03-21 03:31:44.000000 fastFET-0.0.5/fastFET/BGPMAGNET/bgpparser/__init__.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)     8211 2023-03-21 03:31:45.000000 fastFET-0.0.5/fastFET/BGPMAGNET/bgpparser/base.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)    12848 2023-03-21 03:31:45.000000 fastFET-0.0.5/fastFET/BGPMAGNET/bgpparser/dump_form.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)    29349 2023-03-21 03:31:46.000000 fastFET-0.0.5/fastFET/BGPMAGNET/bgpparser/init.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)    12332 2023-03-21 03:31:46.000000 fastFET-0.0.5/fastFET/BGPMAGNET/bgpparser/params.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)     2260 2023-03-21 03:31:46.000000 fastFET-0.0.5/fastFET/BGPMAGNET/bgpparser/parse.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)     5934 2023-03-21 03:31:46.000000 fastFET-0.0.5/fastFET/BGPMAGNET/bgpparser/parse_Process.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)     3183 2023-03-21 03:31:46.000000 fastFET-0.0.5/fastFET/BGPMAGNET/bgpparser/read_Process.py
-drwxr-xr-x   0 hlei0     (1000) hlei0     (1000)        0 2023-03-21 03:56:04.790329 fastFET-0.0.5/fastFET/BGPMAGNET/config/
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)      943 2023-03-21 03:31:46.000000 fastFET-0.0.5/fastFET/BGPMAGNET/config/collector_list.ini
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)       69 2023-03-21 03:31:46.000000 fastFET-0.0.5/fastFET/BGPMAGNET/config/parseMRT.ini
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)     1276 2023-03-21 03:31:44.000000 fastFET-0.0.5/fastFET/BGPMAGNET/dataGetter.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)      588 2023-03-21 03:31:44.000000 fastFET-0.0.5/fastFET/BGPMAGNET/download.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)     1575 2023-03-21 03:31:44.000000 fastFET-0.0.5/fastFET/BGPMAGNET/params.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)     1292 2023-03-21 03:31:44.000000 fastFET-0.0.5/fastFET/BGPMAGNET/parse.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)      955 2023-03-21 03:31:44.000000 fastFET-0.0.5/fastFET/BGPMAGNET/tools.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)    43916 2023-03-21 03:31:43.000000 fastFET-0.0.5/fastFET/FET.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)     7300 2023-03-21 03:31:43.000000 fastFET-0.0.5/fastFET/MultiProcess.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)    13039 2023-03-21 03:31:43.000000 fastFET-0.0.5/fastFET/README.md
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)     5027 2023-03-21 03:31:43.000000 fastFET-0.0.5/fastFET/RIPEStatAPI.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)       22 2023-03-21 03:31:43.000000 fastFET-0.0.5/fastFET/__init__.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)    55623 2023-03-21 03:31:43.000000 fastFET-0.0.5/fastFET/bgpToolKit.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)    19462 2023-03-21 03:31:43.000000 fastFET-0.0.5/fastFET/collectData.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)       63 2023-03-21 03:31:43.000000 fastFET-0.0.5/fastFET/event_list.csv
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)    42416 2023-03-21 03:31:43.000000 fastFET-0.0.5/fastFET/featGraph.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)    38994 2023-03-21 03:31:43.000000 fastFET-0.0.5/fastFET/featTradition.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)    10970 2023-03-21 03:31:43.000000 fastFET-0.0.5/fastFET/featTree.py
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)     1428 2023-03-21 03:31:43.000000 fastFET-0.0.5/fastFET/logConfig.json
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)    18822 2023-03-21 03:31:43.000000 fastFET-0.0.5/fastFET/utils.py
-drwxr-xr-x   0 hlei0     (1000) hlei0     (1000)        0 2023-03-21 03:56:04.750329 fastFET-0.0.5/fastFET.egg-info/
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)    13262 2023-03-21 03:56:04.000000 fastFET-0.0.5/fastFET.egg-info/PKG-INFO
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)     1128 2023-03-21 03:56:04.000000 fastFET-0.0.5/fastFET.egg-info/SOURCES.txt
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)        1 2023-03-21 03:56:04.000000 fastFET-0.0.5/fastFET.egg-info/dependency_links.txt
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)      197 2023-03-21 03:56:04.000000 fastFET-0.0.5/fastFET.egg-info/requires.txt
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)        8 2023-03-21 03:56:04.000000 fastFET-0.0.5/fastFET.egg-info/top_level.txt
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)      212 2023-03-21 03:42:39.000000 fastFET-0.0.5/requirements.txt
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)       38 2023-03-21 03:56:04.790329 fastFET-0.0.5/setup.cfg
--rw-r--r--   0 hlei0     (1000) hlei0     (1000)     1392 2023-03-21 03:47:11.000000 fastFET-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:47:46.819051 fastFET-0.0.6/
+-rw-rw-rw-   0        0        0      192 2023-06-18 09:39:49.000000 fastFET-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    13408 2023-06-18 13:47:46.818051 fastFET-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-18 13:47:46.731056 fastFET-0.0.6/fastFET/
+drwxrwxrwx   0        0        0        0 2023-06-18 13:47:46.759049 fastFET-0.0.6/fastFET/BGPMAGNET/
+-rw-rw-rw-   0        0        0     3102 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/BGPMAGNET/ProcessHandler.py
+-rw-rw-rw-   0        0        0     3586 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/BGPMAGNET/README.md
+-rw-rw-rw-   0        0        0        0 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/BGPMAGNET/__init__.py
+-rw-rw-rw-   0        0        0     6482 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/BGPMAGNET/base.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:47:46.811050 fastFET-0.0.6/fastFET/BGPMAGNET/bgpparser/
+-rw-rw-rw-   0        0        0        0 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/BGPMAGNET/bgpparser/__init__.py
+-rw-rw-rw-   0        0        0     8211 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/BGPMAGNET/bgpparser/base.py
+-rw-rw-rw-   0        0        0    12848 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/BGPMAGNET/bgpparser/dump_form.py
+-rw-rw-rw-   0        0        0    29349 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/BGPMAGNET/bgpparser/init.py
+-rw-rw-rw-   0        0        0    12332 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/BGPMAGNET/bgpparser/params.py
+-rw-rw-rw-   0        0        0     2260 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/BGPMAGNET/bgpparser/parse.py
+-rw-rw-rw-   0        0        0     5934 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/BGPMAGNET/bgpparser/parse_Process.py
+-rw-rw-rw-   0        0        0     3183 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/BGPMAGNET/bgpparser/read_Process.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:47:46.816049 fastFET-0.0.6/fastFET/BGPMAGNET/config/
+-rw-rw-rw-   0        0        0      943 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/BGPMAGNET/config/collector_list.ini
+-rw-rw-rw-   0        0        0       69 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/BGPMAGNET/config/parseMRT.ini
+-rw-rw-rw-   0        0        0     1276 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/BGPMAGNET/dataGetter.py
+-rw-rw-rw-   0        0        0      588 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/BGPMAGNET/download.py
+-rw-rw-rw-   0        0        0     1575 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/BGPMAGNET/params.py
+-rw-rw-rw-   0        0        0     1292 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/BGPMAGNET/parse.py
+-rw-rw-rw-   0        0        0      955 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/BGPMAGNET/tools.py
+-rw-rw-rw-   0        0        0    27585 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/FET.py
+-rw-rw-rw-   0        0        0     4796 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/MultiProcess.py
+-rw-rw-rw-   0        0        0    12942 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/README.md
+-rw-rw-rw-   0        0        0     5957 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/RIPEStatAPI.py
+-rw-rw-rw-   0        0        0       22 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/__init__.py
+-rw-rw-rw-   0        0        0    63942 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/bgpToolKit.py
+-rw-rw-rw-   0        0        0    16650 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/collectData.py
+-rw-rw-rw-   0        0        0     5917 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/drawing.py
+-rw-rw-rw-   0        0        0       63 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/event_list.csv
+-rw-rw-rw-   0        0        0    30606 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/featGraph.py
+-rw-rw-rw-   0        0        0    20347 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/featTradition.py
+-rw-rw-rw-   0        0        0     8606 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/featTree.py
+-rw-rw-rw-   0        0        0     1428 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/logConfig.json
+-rw-rw-rw-   0        0        0    14772 2023-06-18 09:34:59.000000 fastFET-0.0.6/fastFET/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:47:46.743050 fastFET-0.0.6/fastFET.egg-info/
+-rw-rw-rw-   0        0        0    13408 2023-06-18 13:47:46.000000 fastFET-0.0.6/fastFET.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1147 2023-06-18 13:47:46.000000 fastFET-0.0.6/fastFET.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 13:47:46.000000 fastFET-0.0.6/fastFET.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-06-18 13:47:46.000000 fastFET-0.0.6/fastFET.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-18 13:47:46.000000 fastFET-0.0.6/fastFET.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      221 2023-06-18 09:43:38.000000 fastFET-0.0.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 13:47:46.820050 fastFET-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1436 2023-06-18 13:46:54.000000 fastFET-0.0.6/setup.py
```

### Comparing `fastFET-0.0.5/PKG-INFO` & `fastFET-0.0.6/fastFET/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,264 +1,245 @@
-Metadata-Version: 2.1
-Name: fastFET
-Version: 0.0.5
-Summary: A fast feature extrating tool for BGP Dataset Collection.
-Home-page: https://github.com/JamesRay0713/fastFET
-Author: James Ray
-Author-email: hl1670704310@icloud.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-
-##
-logger.info( utils.logMemUsage(10, inspect.stack()[0][3] ))     # 调试锚点：随删
-##
-
-持续优化的问题：
-- 计算ED那里，对比测试多进程的情况。
-- 自定义多进程模块中，等待睡眠为1s是否合理。
-- 做一个对比各个特征计算时间的函数。
-- 构建函数：输入一个或多个新特征，能把采集结果追加到已有的DF.csv。这要涉及到`自定义特征采集函数`的API
-- 关于每slot如何构建全局拓扑图：还是要结合pl.DF来加速计算，避免逐条消息更新。
-- requirement的预安装，特别是bgpdump
-- 针对异常类型的特征设计：子前缀劫持、路径劫持、路由泄露等，连接其他框架？
-
-require add:
-    - pyarrow
-
-# BGP特征提取工具 
-
-## 组织结构
-
-### 1. 库路径
-
-```
-fastFET  
-    ├── BGPMAGNET/      BGP原始数据下载工具(by倪泽栋)  
-    ├── collectData.py  主模块：数据收集，包括下载、解析   
-    ├── event_list.csv　要采集的事件列表  
-    ├── featGraph.py    图特征采集功能集合   
-    ├── featTradition.py传统特征采集功能集合  
-    ├── featTree.py     特征树，集成所有特征及其pl.Expr  
-    ├── FET.py          主模块：特征采集  
-    ├── logConfig.json  日志配置  
-    ├── utils.py        工具集合   
-    ├── MultiProcess.py 多进程工具   
-    ├── README.md  
-    └── requirements.txt
-``` 
-
-### 2. cwd 默认路径
-```
-cwd  
-├── Dataset  
-│   ├── features/               特征提取最终数据  
-│   │　　└── date_event_monitor.csv  
-│   ├── MOAS/                   提取过程中属于multi-origin-AS的消息  
-│   ├── raw_cmpres              原始数据下载存放路径    
-│   │   ├── rrc00/    
-│   │   └── routeviews./    
-│   └── raw_parsed              原始数据解析存放路径    
-│       └── 事件名  
-│           └── 采集器名/  
-└── log                         日志路径    
-    ├── errors.log  
-    └── info.log 
-```
-
-## 使用方法
-
-创建特征提取工具对象`fet`, 指定特征集合, 添加目标事件信息, 开始提取特征。
-```python
-from fastFET import FET
-ev= FET.EventEditor()
-ev.addEvents([])
-fet= FET.FET()
-fet.setCustomFeats([])
-feat_path= fet.run()
-```
-- 先利用 EventEditor 的 addEvents 方法添加此次要采集特征的事件信息。
-    - 格式：事件名；起始时间；结束时间（可缺省）；采集器（可多个，用`,`相隔）
-    - 举例：`GoogleLeak,2017/08/25 05:00:00,2017/08/25 06:00:00,rrc06,rrc05`
-- 后利用 `fet` 对象实现特征采集操作。
-    1. 初始化对象: `fet= FET.FET()`, 参数见注释, 其中 `slot` 为特征采集的时间尺度, 默认1分钟。
-        
-    2. 自定义此次采集所需的特征集合: `fet.setCustomFeats([...])`
-        - 有3种自定义特征的方法：全量采集；按类别采集；按单个特征采集 (详见该方法的注释)
-        - 若想查看该工具现已集成的特征列表：`feats= fet.getAllFeats()`
-
-    3. 正式采集特征: `fet.run()`
-        - 参数: 当`fet`对象仅仅只从大量 rib 表采集图特征时`only_rib`才为`True`, 此时自定义的特征集合仅限于图特征
-        - 返回: 特征存放路径
-
-## 框架解释
-- RIPE NCC和RouteViews的`.gz`和`.bz2`原始数据经并行下载和 `bgpdump`工具转码得到的`.txt`文件，根据事件和采集器名分别存入 `./Dataset/raw_parsed/event_name/monitor_name/`
-- 利用 `polars` 数据分析工具高效提取BGP特征，按事件名存入 `./Dataset/features/date__event__collector.csv`。
-- 顺便收集了事件中出现的MOAS消息，存入`./Dataset/MOAS/`
-
-
-## 输出字段说明
-- 共139字段，含序列号，日期，136个特征，及标签。
-
-类别 | 字段 | 解释
-|---|---|--- 
-\- | time_bin | 时间序列号
-\- | date | 日期
-volume | v_total | 消息总数
-\- | v_A | 宣告消息总数
-\- | v_W | 撤销消息总数
-\- | v_IGP | 属于IGP的消息总数
-\- | v_EGP | 属于EGP的消息总数
-\- | v_ICMP | 属于IMCOMPLETE的消息总数
-\- | v_peer | 不同peer的数量
-\- | v_pfx_t_cnt | 不同prefix的数量
-\- | v_pfx_t_avg | 不同prefix出现过的平均次数
-\- | v_pfx_t_max | 不同prefix出现过的最大次数
-\- | v_pfx_A_cnt | 属宣告的不同prefix的数量
-\- | v_pfx_A_avg | 属宣告的不同prefix出现过的平均次数
-\- | v_pfx_A_max | 属宣告的不同prefix出现过的最大次数
-\- | v_pfx_W_cnt | 属撤销的不同prefix的数量
-\- | v_pfx_W_avg | 属撤销的不同prefix出现过的平均次数
-\- | v_pfx_W_max | 属撤销的不同prefix出现过的最大次数
-\- | v_pp_t_cnt | 不同peer-prefix对的数量
-\- | v_pp_t_avg | 不同peer-prefix对出现过的平均次数
-\- | v_pp_t_max | 不同peer-prefix对出现过的最大次数
-\- | v_pp_A_cnt | 属宣告的不同peer-prefix对的数量
-\- | v_pp_A_avg | 属宣告的不同peer-prefix对出现过的平均次数
-\- | v_pp_A_max | 属宣告的不同peer-prefix对出现过的最大次数
-\- | v_pp_W_cnt | 属撤销的不同peer-prefix对的数量
-\- | v_pp_W_avg | 属撤销的不同peer-prefix对出现过的平均次数
-\- | v_pp_W_max | 属撤销的不同peer-prefix对出现过的最大次数
-\- | v_oriAS_t_cnt | 源AS的数量
-\- | v_oriAS_t_avg | 源AS的平均出现次数
-\- | v_oriAS_t_max | 源AS的最大出现次数
-\- | v_oriAS_peer_cnt | 不同peer-originAS对的数量
-\- | v_oriAS_peer_avg | 不同peer-originAS对出现过的平均次数
-\- | v_oriAS_peer_max | 不同peer-originAS对出现过的最大次数
-\- | v_oriAS_pfx_cnt | 不同prefix-originAS对的数量
-\- | v_oriAS_pfx_avg | 不同prefix-originAS对出现过的平均次数
-\- | v_oriAS_pfx_max | 不同prefix-originAS对出现过的最大次数
-\- | v_oriAS_pp_cnt | 不同peer-prefix-originAS对的数量
-\- | v_oriAS_pp_avg | 不同peer-prefix-originAS对出现过的平均次数
-\- | v_oriAS_pp_max | 不同peer-prefix-originAS对出现过的最大次数
-path | path_len_max | 最大路径长度
-\- | path_len_avg | 平均路径长度
-\- | path_unq_len_max | 去重后的最大路径长度
-\- | path_unq_len_avg | 去重后的平均路径长度
-AS | As_total_cnt | 出现过的AS的数量
-\- | As_total_avg | 不同AS出现过的平均次数
-\- | As_total_max | 不同AS出现过的最大次数
-\- | AS_rare_avg | 所有消息的路径中含有稀有AS的总共数量
-\- | AS_rare_sum | 一条消息的路径中含有稀有AS的最大数量
-dynamic | is_WA | 属于撤销后宣告的消息数
-\- | is_AW | 属于宣告后撤销的消息数
-\- | is_WAW | 属于撤销-宣告-撤销的消息数
-\- | is_longer_path | 路径变长的消息数
-\- | is_shorter_path | 路径变短的消息数
-\- | is_longer_unq_path | 去重后路径变长的消息数
-\- | is_shorter_unq_path | 去重后路径变短的消息数
-\- | is_new | 属于全新宣告的消息数
-\- | is_dup_ann | 属于重复宣告的消息数（仅prefix重复）
-\- | is_AWnA | 属于宣告-撤销多次-宣告的消息数
-\- | is_imp_wd | 属于隐式撤销的消息数（重复宣告，但其他属性变化）
-\- | is_WnA | 属于撤销多次-宣告的消息数
-\- | is_AWn | 属于宣告-多次撤销的消息数
-\- | is_AnW | 属于多次宣告-撤销的消息数
-\- | is_WAn | 属于撤销-多次宣告的消息数
-\- | is_dup_wd | 属于重复撤销的消息数
-\- | is_dup | 属于重复宣告的消息数（完全重复）
-\- | is_flap | 属于宣告-撤销-宣告，且属性完全不变的消息数
-\- | is_NADA | 属于宣告-撤销-宣告，但属性有变化的消息数
-\- | is_imp_wd_spath | 属于路径属性不变的隐式撤销的消息数
-\- | is_imp_wd_dpath | 属于路径属性变化的隐式撤销的消息数
-\- | type_0 | 针对同一prefix，源AS改变了的消息数(MOAS)
-\- | type_1 | 针对同一prefix，path中第2个AS改变了的消息数
-\- | type_2 | 针对同一prefix，path中第3个AS改变了的消息数
-\- | type_3 | 针对同一prefix，path中第4个AS改变了的消息数
-\- | ED_max | 同一peer-prefix下，最大的编辑距离值的消息数
-\- | ED_avg | 同一peer-prefix下，平均的编辑距离值的消息数
-\- | ED_0 | 同一peer-prefix下，编辑距离为0的消息数
-\- | ED_1 ~ ED_10 | 同一peer-prefix下，编辑距离为1~10的消息数
-ratio | ratio_firstOrder | 最活跃的宣告前缀/宣告总数（即 `v_pfx_A_max / v_A`）
-\- | ratio_ann | 宣告量占更新消息总量之比（即`v_A / v_total`）
-\- | ratio_wd | 撤销量占更新消息总量之比（即`v_W / v_total`）
-\- | ratio_origin0 | IGP占宣告量之比（即`v_IGP / v_A`）
-\- | ratio_origin1 | EGP占宣告量之比（即`v_EGP / v_A`）
-\- | ratio_origin2 | IMCOMPLETE占宣告量之比（即`v_ICMP / v_A`）
-\- | ratio_dup_ann | 完全重复宣告占宣告量之比（即`is_dup_ann / v_A`）
-\- | ratio_flap | 属性完全不变的宣-撤-宣占宣告量之比（即`is_flap / v_A`）
-\- | ratio_NADA | 属性有变化的宣-撤-宣占宣告量之比（即`is_NADA / v_A`）
-\- | ratio_imp_wd | 隐式撤销占宣告量之比（即`is_imp_wd / v_A`）
-\- | ratio_imp_wd2 | 隐式撤销占隐式撤销+撤销之比（即`is_imp_wd / (is_imp_wd+ v_W)`）
-\- | ratio_exp_wd | 真正撤销占隐式撤销+撤销之比（即`v_W / (is_imp_wd+ v_W)`）
-\- | ratio_imp_wd_dpath | 路径属性不同的隐式撤销占隐式撤销之比（即`is_imp_wd_dpath / is_imp_wd`）
-\- | ratio_imp_wd_spath | 路径属性相同的隐式撤销占隐式撤销之比（即`is_imp_wd_spath / is_imp_wd`）
-\- | ratio_new | 全新宣告占宣告量之比（即`is_new / v_A`）
-\- | ratio_wd_dups | 重复撤销占撤销量之比（即`is_dup_wd / v_W`）
-\- | ratio_longer_path | 更长路径宣告占宣告量之比（即`is_longer_path / v_A`）
-\- | ratio_shorter_path | 更短路径宣告占宣告量之比（即`is_shorter_path / v_A`）
-\- | ratio_longer_path2 | 更长路径宣告占更长/短宣告量之比（即`is_longer_path / (is_longer_path+ is_shorter_path)`）
-\- | ratio_shorter_path2 | 更短路径宣告占更长/短宣告量之比（即`is_shorter_path / (is_longer_path+ is_shorter_path)`）
-node_level_graph | nd_degree_centrality | 节点平均度中心性
-\- | nd_node_clique_number | 节点平均最大集团数
-\- | nd_number_of_cliques | 节点平均集团数
-\- | nd_closeness_centrality | 节点平均紧密中心性
-\- | nd_betweenness_centrality | 节点平均中介中心性
-\- | nd_local_efficiency | 节点平均局部效率
-\- | nd_harmonic_centrality | 节点平均谐波中心度
-\- | nd_eigenvector_centrality | 节点平均特征向量中心度
-\- | nd_pagerank | 节点平均重要度排名
-\- | nd_clustering | 节点平均聚类中心性
-\- | nd_triangles | 节点平均三角形数量
-\- | nd_eccentricity | 节点平均偏心率
-\- | nd_average_shortest_pth_length | 节点平均最短路径长度
-\- | nd_load_centrality | 节点平均负载中心性
-\- | nd_degree | 节点平均度数
-\- | nd_square_clustering | 节点平均平方聚类系数
-\- | nd_average_neighbor_degree | 节点平均邻居度数
-AS_level_graph | gp_nb_of_nodes | 总节点数
-\- | gp_nb_of_edges | 总边数
-\- | gp_diameter | 最大偏心率
-\- | gp_assortativity | 同配性
-\- | gp_largest_eigenvalue | 最大特征值
-\- | gp_algebraic_connectivity | 代数连通度
-\- | gp_effective_graph_resistance | 有效图阻抗
-\- | gp_symmetry_ratio | 对称率
-\- | gp_natural_connectivity | 自然连通度
-\- | gp_node_connectivity | 节点连通度
-\- | gp_edge_connectivity | 边连通度
-\- | gp_weighted_spectrum_3 | 三方加权频谱
-\- | gp_weighted_spectrum_4 | 四方加权频谱
-\- | gp_percolation_limit | 渗透极限
-\- | gp_nb_spanning_trees | 生成树数量
-\- | label	|	异常类型标签
-
-
-
-
-## 特征补充
-
-字段            |  说明
- ----           |  ----
-ConcentratRatio |  前三个最活跃的宣告前缀/宣告总数（即 `vol_ann_pfx_max / v_A`）
-
-
-## 其他注意事项 
-
-1. BGP RAW DATA: 采集时间间隔不统一，如rrc00中20030723.0745之前为15min（且时刻不固定），之后为5min（时刻固定）。
-2. MRT文件解析后，path 字段可能存在`{}`形式，如下: 
-    - 58057 6939 4635 4788 38044 23736
-    - 58057 6939 4635 4788 38044 {23736}
-    - 58057 6939 1299 2603 2603 2603 6509 {271,7860,8111,53904}
-3. `stat.ripe.net`的API获取的路由，path字段可能存在`[]`形式。
-3. `Route-Views`中的MRT文件名格式不严谨，经常出现无规律的时间戳。
-
-
-# 发现：
-- 劫持震荡：
-当`is_MOAS`很大，而`vol_oriAS_peer_pfx`或`vol_oriAS_pfx`很小时，说明存在一个prefix反复被多个AS宣告的情况。
-- outage类型难溯源
-
+
+持续优化的问题：
+- 计算ED那里，对比测试多进程的情况。
+- 自定义多进程模块中，等待睡眠为1s是否合理。
+- 做一个对比各个特征计算时间的函数。
+- 构建函数：输入一个或多个新特征，能把采集结果追加到已有的DF.csv。这要涉及到`自定义特征采集函数`的API
+- 关于每slot如何构建全局拓扑图：还是要结合pl.DF来加速计算，避免逐条消息更新。
+- requirement的预安装，特别是bgpdump
+- 针对异常类型的特征设计：子前缀劫持、路径劫持、路由泄露等，连接其他框架？
+
+require add:
+    - pyarrow
+
+# BGP特征提取工具 
+
+## 组织结构
+
+### 1. 库路径
+
+```
+fastFET  
+    ├── BGPMAGNET/      BGP原始数据下载工具(by倪泽栋)  
+    ├── collectData.py  主模块：数据收集，包括下载、解析   
+    ├── event_list.csv　要采集的事件列表  
+    ├── featGraph.py    图特征采集功能集合   
+    ├── featTradition.py传统特征采集功能集合  
+    ├── featTree.py     特征树，集成所有特征及其pl.Expr  
+    ├── FET.py          主模块：特征采集  
+    ├── logConfig.json  日志配置  
+    ├── utils.py        工具集合   
+    ├── MultiProcess.py 多进程工具   
+    ├── README.md  
+    └── requirements.txt
+``` 
+
+### 2. cwd 默认路径
+```
+cwd  
+├── Dataset  
+│   ├── features/               特征提取最终数据  
+│   │　　└── date_event_monitor.csv  
+│   ├── MOAS/                   提取过程中属于multi-origin-AS的消息  
+│   ├── raw_cmpres              原始数据下载存放路径    
+│   │   ├── rrc00/    
+│   │   └── routeviews./    
+│   └── raw_parsed              原始数据解析存放路径    
+│       └── 事件名  
+│           └── 采集器名/  
+└── log                         日志路径    
+    ├── errors.log  
+    └── info.log 
+```
+
+## 使用方法
+
+创建特征提取工具对象`fet`, 指定特征集合, 添加目标事件信息, 开始提取特征。
+```python
+from fastFET import FET
+ev= FET.EventEditor()
+ev.addEvents([])
+fet= FET.FET()
+fet.setCustomFeats([])
+feat_path= fet.run()
+```
+- 先利用 EventEditor 的 addEvents 方法添加此次要采集特征的事件信息。
+    - 格式：事件名；起始时间；结束时间（可缺省）；采集器（可多个，用`,`相隔）
+    - 举例：`GoogleLeak,2017/08/25 05:00:00,2017/08/25 06:00:00,rrc06,rrc05`
+- 后利用 `fet` 对象实现特征采集操作。
+    1. 初始化对象: `fet= FET.FET()`, 参数见注释, 其中 `slot` 为特征采集的时间尺度, 默认1分钟。
+        
+    2. 自定义此次采集所需的特征集合: `fet.setCustomFeats([...])`
+        - 有3种自定义特征的方法：全量采集；按类别采集；按单个特征采集 (详见该方法的注释)
+        - 若想查看该工具现已集成的特征列表：`feats= fet.getAllFeats()`
+
+    3. 正式采集特征: `fet.run()`
+        - 参数: 当`fet`对象仅仅只从大量 rib 表采集图特征时`only_rib`才为`True`, 此时自定义的特征集合仅限于图特征
+        - 返回: 特征存放路径
+
+## 框架解释
+- RIPE NCC和RouteViews的`.gz`和`.bz2`原始数据经并行下载和 `bgpdump`工具转码得到的`.txt`文件，根据事件和采集器名分别存入 `./Dataset/raw_parsed/event_name/monitor_name/`
+- 利用 `polars` 数据分析工具高效提取BGP特征，按事件名存入 `./Dataset/features/date__event__collector.csv`。
+- 顺便收集了事件中出现的MOAS消息，存入`./Dataset/MOAS/`
+
+
+## 输出字段说明
+- 共139字段，含序列号，日期，136个特征，及标签。
+
+类别 | 字段 | 解释
+|---|---|--- 
+\- | time_bin | 时间序列号
+\- | date | 日期
+volume | v_total | 消息总数
+\- | v_A | 宣告消息总数
+\- | v_W | 撤销消息总数
+\- | v_IGP | 属于IGP的消息总数
+\- | v_EGP | 属于EGP的消息总数
+\- | v_ICMP | 属于IMCOMPLETE的消息总数
+\- | v_peer | 不同peer的数量
+\- | v_pfx_t_cnt | 不同prefix的数量
+\- | v_pfx_t_avg | 不同prefix出现过的平均次数
+\- | v_pfx_t_max | 不同prefix出现过的最大次数
+\- | v_pfx_A_cnt | 属宣告的不同prefix的数量
+\- | v_pfx_A_avg | 属宣告的不同prefix出现过的平均次数
+\- | v_pfx_A_max | 属宣告的不同prefix出现过的最大次数
+\- | v_pfx_W_cnt | 属撤销的不同prefix的数量
+\- | v_pfx_W_avg | 属撤销的不同prefix出现过的平均次数
+\- | v_pfx_W_max | 属撤销的不同prefix出现过的最大次数
+\- | v_pp_t_cnt | 不同peer-prefix对的数量
+\- | v_pp_t_avg | 不同peer-prefix对出现过的平均次数
+\- | v_pp_t_max | 不同peer-prefix对出现过的最大次数
+\- | v_pp_A_cnt | 属宣告的不同peer-prefix对的数量
+\- | v_pp_A_avg | 属宣告的不同peer-prefix对出现过的平均次数
+\- | v_pp_A_max | 属宣告的不同peer-prefix对出现过的最大次数
+\- | v_pp_W_cnt | 属撤销的不同peer-prefix对的数量
+\- | v_pp_W_avg | 属撤销的不同peer-prefix对出现过的平均次数
+\- | v_pp_W_max | 属撤销的不同peer-prefix对出现过的最大次数
+\- | v_oriAS_t_cnt | 源AS的数量
+\- | v_oriAS_t_avg | 源AS的平均出现次数
+\- | v_oriAS_t_max | 源AS的最大出现次数
+\- | v_oriAS_peer_cnt | 不同peer-originAS对的数量
+\- | v_oriAS_peer_avg | 不同peer-originAS对出现过的平均次数
+\- | v_oriAS_peer_max | 不同peer-originAS对出现过的最大次数
+\- | v_oriAS_pfx_cnt | 不同prefix-originAS对的数量
+\- | v_oriAS_pfx_avg | 不同prefix-originAS对出现过的平均次数
+\- | v_oriAS_pfx_max | 不同prefix-originAS对出现过的最大次数
+\- | v_oriAS_pp_cnt | 不同peer-prefix-originAS对的数量
+\- | v_oriAS_pp_avg | 不同peer-prefix-originAS对出现过的平均次数
+\- | v_oriAS_pp_max | 不同peer-prefix-originAS对出现过的最大次数
+path | path_len_max | 最大路径长度
+\- | path_len_avg | 平均路径长度
+\- | path_unq_len_max | 去重后的最大路径长度
+\- | path_unq_len_avg | 去重后的平均路径长度
+AS | As_total_cnt | 出现过的AS的数量
+\- | As_total_avg | 不同AS出现过的平均次数
+\- | As_total_max | 不同AS出现过的最大次数
+\- | AS_rare_avg | 所有消息的路径中含有稀有AS的总共数量
+\- | AS_rare_sum | 一条消息的路径中含有稀有AS的最大数量
+dynamic | is_WA | 属于撤销后宣告的消息数
+\- | is_AW | 属于宣告后撤销的消息数
+\- | is_WAW | 属于撤销-宣告-撤销的消息数
+\- | is_longer_path | 路径变长的消息数
+\- | is_shorter_path | 路径变短的消息数
+\- | is_longer_unq_path | 去重后路径变长的消息数
+\- | is_shorter_unq_path | 去重后路径变短的消息数
+\- | is_new | 属于全新宣告的消息数
+\- | is_dup_ann | 属于重复宣告的消息数（仅prefix重复）
+\- | is_AWnA | 属于宣告-撤销多次-宣告的消息数
+\- | is_imp_wd | 属于隐式撤销的消息数（重复宣告，但其他属性变化）
+\- | is_WnA | 属于撤销多次-宣告的消息数
+\- | is_AWn | 属于宣告-多次撤销的消息数
+\- | is_AnW | 属于多次宣告-撤销的消息数
+\- | is_WAn | 属于撤销-多次宣告的消息数
+\- | is_dup_wd | 属于重复撤销的消息数
+\- | is_dup | 属于重复宣告的消息数（完全重复）
+\- | is_flap | 属于宣告-撤销-宣告，且属性完全不变的消息数
+\- | is_NADA | 属于宣告-撤销-宣告，但属性有变化的消息数
+\- | is_imp_wd_spath | 属于路径属性不变的隐式撤销的消息数
+\- | is_imp_wd_dpath | 属于路径属性变化的隐式撤销的消息数
+\- | type_0 | 针对同一prefix，源AS改变了的消息数(MOAS)
+\- | type_1 | 针对同一prefix，path中第2个AS改变了的消息数
+\- | type_2 | 针对同一prefix，path中第3个AS改变了的消息数
+\- | type_3 | 针对同一prefix，path中第4个AS改变了的消息数
+\- | ED_max | 同一peer-prefix下，最大的编辑距离值的消息数
+\- | ED_avg | 同一peer-prefix下，平均的编辑距离值的消息数
+\- | ED_0 | 同一peer-prefix下，编辑距离为0的消息数
+\- | ED_1 ~ ED_10 | 同一peer-prefix下，编辑距离为1~10的消息数
+ratio | ratio_firstOrder | 最活跃的宣告前缀/宣告总数（即 `v_pfx_A_max / v_A`）
+\- | ratio_ann | 宣告量占更新消息总量之比（即`v_A / v_total`）
+\- | ratio_wd | 撤销量占更新消息总量之比（即`v_W / v_total`）
+\- | ratio_origin0 | IGP占宣告量之比（即`v_IGP / v_A`）
+\- | ratio_origin1 | EGP占宣告量之比（即`v_EGP / v_A`）
+\- | ratio_origin2 | IMCOMPLETE占宣告量之比（即`v_ICMP / v_A`）
+\- | ratio_dup_ann | 完全重复宣告占宣告量之比（即`is_dup_ann / v_A`）
+\- | ratio_flap | 属性完全不变的宣-撤-宣占宣告量之比（即`is_flap / v_A`）
+\- | ratio_NADA | 属性有变化的宣-撤-宣占宣告量之比（即`is_NADA / v_A`）
+\- | ratio_imp_wd | 隐式撤销占宣告量之比（即`is_imp_wd / v_A`）
+\- | ratio_imp_wd2 | 隐式撤销占隐式撤销+撤销之比（即`is_imp_wd / (is_imp_wd+ v_W)`）
+\- | ratio_exp_wd | 真正撤销占隐式撤销+撤销之比（即`v_W / (is_imp_wd+ v_W)`）
+\- | ratio_imp_wd_dpath | 路径属性不同的隐式撤销占隐式撤销之比（即`is_imp_wd_dpath / is_imp_wd`）
+\- | ratio_imp_wd_spath | 路径属性相同的隐式撤销占隐式撤销之比（即`is_imp_wd_spath / is_imp_wd`）
+\- | ratio_new | 全新宣告占宣告量之比（即`is_new / v_A`）
+\- | ratio_wd_dups | 重复撤销占撤销量之比（即`is_dup_wd / v_W`）
+\- | ratio_longer_path | 更长路径宣告占宣告量之比（即`is_longer_path / v_A`）
+\- | ratio_shorter_path | 更短路径宣告占宣告量之比（即`is_shorter_path / v_A`）
+\- | ratio_longer_path2 | 更长路径宣告占更长/短宣告量之比（即`is_longer_path / (is_longer_path+ is_shorter_path)`）
+\- | ratio_shorter_path2 | 更短路径宣告占更长/短宣告量之比（即`is_shorter_path / (is_longer_path+ is_shorter_path)`）
+node_level_graph | nd_degree_centrality | 节点平均度中心性
+\- | nd_node_clique_number | 节点平均最大集团数
+\- | nd_number_of_cliques | 节点平均集团数
+\- | nd_closeness_centrality | 节点平均紧密中心性
+\- | nd_betweenness_centrality | 节点平均中介中心性
+\- | nd_local_efficiency | 节点平均局部效率
+\- | nd_harmonic_centrality | 节点平均谐波中心度
+\- | nd_eigenvector_centrality | 节点平均特征向量中心度
+\- | nd_pagerank | 节点平均重要度排名
+\- | nd_clustering | 节点平均聚类中心性
+\- | nd_triangles | 节点平均三角形数量
+\- | nd_eccentricity | 节点平均偏心率
+\- | nd_average_shortest_pth_length | 节点平均最短路径长度
+\- | nd_load_centrality | 节点平均负载中心性
+\- | nd_degree | 节点平均度数
+\- | nd_square_clustering | 节点平均平方聚类系数
+\- | nd_average_neighbor_degree | 节点平均邻居度数
+AS_level_graph | gp_nb_of_nodes | 总节点数
+\- | gp_nb_of_edges | 总边数
+\- | gp_diameter | 最大偏心率
+\- | gp_assortativity | 同配性
+\- | gp_largest_eigenvalue | 最大特征值
+\- | gp_algebraic_connectivity | 代数连通度
+\- | gp_effective_graph_resistance | 有效图阻抗
+\- | gp_symmetry_ratio | 对称率
+\- | gp_natural_connectivity | 自然连通度
+\- | gp_node_connectivity | 节点连通度
+\- | gp_edge_connectivity | 边连通度
+\- | gp_weighted_spectrum_3 | 三方加权频谱
+\- | gp_weighted_spectrum_4 | 四方加权频谱
+\- | gp_percolation_limit | 渗透极限
+\- | gp_nb_spanning_trees | 生成树数量
+\- | label	|	异常类型标签
+
+
+
+
+## 特征补充
+
+字段            |  说明
+ ----           |  ----
+ConcentratRatio |  前三个最活跃的宣告前缀/宣告总数（即 `vol_ann_pfx_max / v_A`）
+
+
+## 其他注意事项 
+
+1. BGP RAW DATA: 采集时间间隔不统一，如rrc00中20030723.0745之前为15min（且时刻不固定），之后为5min（时刻固定）。
+2. MRT文件解析后，path 字段可能存在`{}`形式，如下: 
+    - 58057 6939 4635 4788 38044 23736
+    - 58057 6939 4635 4788 38044 {23736}
+    - 58057 6939 1299 2603 2603 2603 6509 {271,7860,8111,53904}
+3. `stat.ripe.net`的API获取的路由，path字段可能存在`[]`形式。
+3. `Route-Views`中的MRT文件名格式不严谨，经常出现无规律的时间戳。
+
+
+# 发现：
+- 劫持震荡：
+当`is_MOAS`很大，而`vol_oriAS_peer_pfx`或`vol_oriAS_pfx`很小时，说明存在一个prefix反复被多个AS宣告的情况。
+- outage类型难溯源
```

### Comparing `fastFET-0.0.5/fastFET/BGPMAGNET/ProcessHandler.py` & `fastFET-0.0.6/fastFET/BGPMAGNET/ProcessHandler.py`

 * *Files identical despite different names*

### Comparing `fastFET-0.0.5/fastFET/BGPMAGNET/README.md` & `fastFET-0.0.6/fastFET/BGPMAGNET/README.md`

 * *Files identical despite different names*

### Comparing `fastFET-0.0.5/fastFET/BGPMAGNET/base.py` & `fastFET-0.0.6/fastFET/BGPMAGNET/base.py`

 * *Files identical despite different names*

### Comparing `fastFET-0.0.5/fastFET/BGPMAGNET/bgpparser/base.py` & `fastFET-0.0.6/fastFET/BGPMAGNET/bgpparser/base.py`

 * *Files identical despite different names*

### Comparing `fastFET-0.0.5/fastFET/BGPMAGNET/bgpparser/dump_form.py` & `fastFET-0.0.6/fastFET/BGPMAGNET/bgpparser/dump_form.py`

 * *Files identical despite different names*

### Comparing `fastFET-0.0.5/fastFET/BGPMAGNET/bgpparser/init.py` & `fastFET-0.0.6/fastFET/BGPMAGNET/bgpparser/init.py`

 * *Files identical despite different names*

### Comparing `fastFET-0.0.5/fastFET/BGPMAGNET/bgpparser/params.py` & `fastFET-0.0.6/fastFET/BGPMAGNET/bgpparser/params.py`

 * *Files identical despite different names*

### Comparing `fastFET-0.0.5/fastFET/BGPMAGNET/bgpparser/parse.py` & `fastFET-0.0.6/fastFET/BGPMAGNET/bgpparser/parse.py`

 * *Files identical despite different names*

### Comparing `fastFET-0.0.5/fastFET/BGPMAGNET/bgpparser/parse_Process.py` & `fastFET-0.0.6/fastFET/BGPMAGNET/bgpparser/parse_Process.py`

 * *Files identical despite different names*

### Comparing `fastFET-0.0.5/fastFET/BGPMAGNET/bgpparser/read_Process.py` & `fastFET-0.0.6/fastFET/BGPMAGNET/bgpparser/read_Process.py`

 * *Files identical despite different names*

### Comparing `fastFET-0.0.5/fastFET/BGPMAGNET/config/collector_list.ini` & `fastFET-0.0.6/fastFET/BGPMAGNET/config/collector_list.ini`

 * *Files identical despite different names*

### Comparing `fastFET-0.0.5/fastFET/BGPMAGNET/dataGetter.py` & `fastFET-0.0.6/fastFET/BGPMAGNET/dataGetter.py`

 * *Files identical despite different names*

### Comparing `fastFET-0.0.5/fastFET/BGPMAGNET/download.py` & `fastFET-0.0.6/fastFET/BGPMAGNET/download.py`

 * *Files identical despite different names*

### Comparing `fastFET-0.0.5/fastFET/BGPMAGNET/params.py` & `fastFET-0.0.6/fastFET/BGPMAGNET/params.py`

 * *Files identical despite different names*

### Comparing `fastFET-0.0.5/fastFET/BGPMAGNET/parse.py` & `fastFET-0.0.6/fastFET/BGPMAGNET/parse.py`

 * *Files identical despite different names*

### Comparing `fastFET-0.0.5/fastFET/BGPMAGNET/tools.py` & `fastFET-0.0.6/fastFET/BGPMAGNET/tools.py`

 * *Files identical despite different names*

### Comparing `fastFET-0.0.5/fastFET/README.md` & `fastFET-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,21 @@
-##
-logger.info( utils.logMemUsage(10, inspect.stack()[0][3] ))     # 调试锚点：随删
-##
+Metadata-Version: 2.1
+Name: fastFET
+Version: 0.0.6
+Summary: A fast feature extrating tool for BGP Dataset Collection.
+Home-page: https://github.com/JamesRay0713/fastFET
+Author: James Ray
+Author-email: hl1670704310@icloud.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+
 
 持续优化的问题：
 - 计算ED那里，对比测试多进程的情况。
 - 自定义多进程模块中，等待睡眠为1s是否合理。
 - 做一个对比各个特征计算时间的函数。
 - 构建函数：输入一个或多个新特征，能把采集结果追加到已有的DF.csv。这要涉及到`自定义特征采集函数`的API
 - 关于每slot如何构建全局拓扑图：还是要结合pl.DF来加速计算，避免逐条消息更新。
@@ -241,8 +252,8 @@
 3. `stat.ripe.net`的API获取的路由，path字段可能存在`[]`形式。
 3. `Route-Views`中的MRT文件名格式不严谨，经常出现无规律的时间戳。
 
 
 # 发现：
 - 劫持震荡：
 当`is_MOAS`很大，而`vol_oriAS_peer_pfx`或`vol_oriAS_pfx`很小时，说明存在一个prefix反复被多个AS宣告的情况。
-- outage类型难溯源
+- outage类型难溯源
```

### Comparing `fastFET-0.0.5/fastFET/RIPEStatAPI.py` & `fastFET-0.0.6/fastFET/RIPEStatAPI.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #! /usr/bin/env python
 # -*-coding:utf-8-*-
 '''
 - Description: `https://stat.ripe.net/data/*`的接口集合，实现对prefix, peer, AS, IP等相关历史数据的查找
 - version: 1.0
 - Author: JamesRay
 - Date: 2023-03-18 05:30:31
-- LastEditTime: 2023-03-19 06:55:09
+- LastEditTime: 2023-06-17 10:01:10
 '''
 import requests
 import jsonpath, json
 from typing import Union
 
 class tools():
     '''- common tools for the script'''
     
     @staticmethod
     def fill_url(*args, **kwargs):
         '''
-        - description: 利用参数组合成一个完整的url
+        - description: 生成url
         - args-> args {array}: array_0: str like `/data/*/data.json`
         - args-> kwargs {object}: 
         - return {*}
         '''
         domain= 'https://stat.ripe.net'
         url= domain+ args[0]
         if 'resource' in kwargs.keys():
@@ -40,16 +40,15 @@
                         url+= f"&{k}={v}"
         return url
 
 class ripeAPI():
 
     @staticmethod
     def pfx2AS(pfxes: Union[str, list], query_time= ''):
-        '''- 给定一个/一组prefix, 输出其所属的AS(列表)
-        - 注：该方法可以获取pfx的`母前缀`
+        '''- 给定一个/一组prefix, 输出所属的AS(列表)
         - args-> query_time {`'2017-04-26T16:00'`}：查找过去某一时刻该pfx所属的AS
             - 注意：查询时间只能是00:00, 08:00, 16:00'''
         if isinstance(pfxes, str):
             pfxes= [pfxes]
         res= []
         for resource in pfxes:
             url= tools.fill_url('/data/prefix-overview/data.json', resource= resource, query_time= query_time)                           
@@ -65,16 +64,17 @@
                 res.append(cur_res)
             except:
                 pass
         return res
 
     @staticmethod
     def AS2pfx(ASn:str, starttime='', endtime= ''):
-        '''- 给定一个AS, 输出其拥有的前缀列表
-        - args-> starttime/endtime {`'2017-04-30T00:00'`}'''
+        '''- 获取一个AS拥有的前缀列表
+        - args-> starttime/endtime {`'2017-04-30T00:00'`}
+        '''
         url= tools.fill_url('/data/announced-prefixes/data.json', resource= ASn, starttime= starttime, endtime= endtime)  
         try:
             data= requests.get(url).json()
             data= jsonpath.jsonpath(data['data']['prefixes'], '$..prefix')
             return data
         except:
             print('wrong with `starttime` or `endtime`')
@@ -94,25 +94,46 @@
         ''' - 获取指定时间(`'2023-01-31T00:00'`)的rrc列表及其peer子列表'''
         url= tools.fill_url('/data/ris-peers/data.json', query_time= query_time)
         data= requests.get(url).json()['data']['peers']
         return data
 
     @staticmethod
     def ip2pfx_and_AS(ips: Union[str, list]):
-        '''- 查找ip所在的prefix和AS。此法有可能返回空值。'''
+        '''- 查找ip所在的prefix和AS。可能返回空值。'''
         if isinstance(ips, str):
             ips= [ips]
         res= {}
         for ip in ips:
             url= tools.fill_url('/data/network-info/data.json', resource= ip)
             data= requests.get(url).json()['data']
             res[ip]= data
         return res
         
     @staticmethod
+    def full_table_peer_list(query_time= ''):
+        '''- 获取rrc中属于`full-table`的peers，即高视野peer。
+        - 参数格式：`"2021-02-01T09:00"`
+        - 返回2个set：`full-table`和非`full-table`, 其元素为`(asn, ip, pfx_version)` '''
+        url_for_thd= tools.fill_url('/data/ris-full-table-threshold/data.json', query_time= query_time)
+        data1= requests.get(url_for_thd).json()['data']
+        v4_thd= data1['v4']
+        v6_thd= data1['v6']
+
+        whole_peer_list= ripeAPI.rrc2peer(query_time)
+        p_full= set()
+        p_nfull=set()
+        for rrc, lis in whole_peer_list.items():
+            for dic in lis:
+                if dic['v4_prefix_count']>= v4_thd or dic['v6_prefix_count']>= v6_thd:
+                    p_full.add( (dic['asn'], dic['ip'], dic['v4_prefix_count']+dic['v6_prefix_count']) )
+                else:
+                    p_nfull.add( (dic['asn'], dic['ip']) )
+        return (p_full, p_nfull)
+
+    @staticmethod
     def reserved_prefixes():
         '''- 获取保留IP地址块列表'''
         lis= [
             '0.0.0.0/8', 
             '10.0.0.0/8', 
             '100.64.0.0/10', 
             '127.0.0.0/8', 
@@ -130,11 +151,12 @@
             '240.0.0.0/4', 
             '255.255.255.255/32'
         ]
         return lis
 
 
 if __name__== "__main__":
-    res= ripeAPI.ip2pfx_and_AS('111.91.233.1')
+    res= ripeAPI.full_table_peer_list("2021-02-01T09:00")
     '''with open('/home/huanglei/work/z_test/1_analysis_routing_flap/tt.json', 'w') as f:
         json.dump(res, f)'''
     print(res)
+    print(len(res[0]), len(res[1]))
```

### Comparing `fastFET-0.0.5/fastFET/bgpToolKit.py` & `fastFET-0.0.6/fastFET/bgpToolKit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 #! /usr/bin/env python
 # coding=utf-8
 '''
 - Description: BGP异常检测中常用的辅助函数
 - version: 1.0
 - Author: JamesRay
 - Date: 2023-02-06 13:10:54 
-- LastEditTime: 2023-03-20 00:25:45
+- LastEditTime: 2023-06-17 04:51:27
 '''
 import os, json, time, re, glob, jsonpath
 import requests
 from bs4 import BeautifulSoup
 from functools import partial
 from typing import Union, List, Dict
 
 import multiprocessing, subprocess
 from multiprocessing import Pool
 import tqdm
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 import networkx as nx
 import pandas as pd
 import polars as pl
 import numpy  as np
 from scipy.stats import kurtosis
 from scipy.fft import fft, ifft
 import statistics
 import pycountry
-    
+
 from sklearn.feature_selection import VarianceThreshold, chi2, SelectKBest, mutual_info_classif 
 from sklearn.model_selection import train_test_split, cross_val_score
 from sklearn.preprocessing import StandardScaler, MinMaxScaler
 from sklearn.ensemble import RandomForestClassifier as RFC
 import matplotlib.pyplot as plt
+import matplotlib.ticker as ticker
+from matplotlib.dates import DateFormatter, AutoDateLocator
+from matplotlib_venn import venn2
 
 from fastFET import utils
+from fastFET.RIPEStatAPI import ripeAPI
 from fastFET.featGraph import graphInterAS
 logger= utils.logger
 
 #######################
 #  地理位置的研究：peers, AS, prefix, IP
 #######################
 from geopy.geocoders import Bing
 import geoip2.database
 
 class CommonTool(object):
-    '''分析BGP事件时常用工具集：
-        - AS, prefix, IP等实体到地理位置的转换
-        - AS, prefix, IP间的互相搜索, 更多API参考: `https://stat.ripe.net/docs/02.data-api/`
-        - 获取保留IP地址块列表
-        '''
+    '''分析BGP事件时常用工具集'''
 
     @staticmethod
     def ip2coord(IPs:list):
         '''
         - description: 获取ip坐标。
         - 首选方法：利用`https://ipinfo.io/{ip}?token={my_token}`接口获取。
             - 优点: 精确; 缺点: 可能收费, 量大时很慢
@@ -83,63 +83,77 @@
             path_db= 'geoLite2-City.mmdb'
             try:
                 assert os.path.exists(path_db) == True
             except:
                 raise RuntimeError(f'there is no `{path_db}`, please execute command as follow:\n \
                     wget https://download.maxmind.com/app/geoip_download?edition_id=GeoLite2-City&license_key=ClwnOBc8c31uvck8&suffix=tar.gz ;tar -zxvf geoip* ; mv GeoLite*/GeoLite2-City.mmdb geoLite2-City.mmdb ; rm -r GeoLite* geoip* '
                 )
-                # reader对象用以ip2coord
+                
             reader = geoip2.database.Reader(path_db)
-                # geolocator对象用以 coord2city
             geolocator = Bing(api_key='Ag7S7BV4AkTdlUzzm_pgSZbQ9c_FBf9IbvSnSlui2x-kE6h-jnYKlT7EHYzRfxjC')
-                # 坐标池，用以加速coord2city, 经纬度是key, 城市名是value
             coord_city_dic= {}
             for ip in IPs:
                 response = reader.city(ip)
                 latitude = response.location.latitude
                 longitude = response.location.longitude
 
                 cityName = response.city.name
                 if cityName!= None:
                     cityName+= ','+ response.country.name
-                else:     #改用Bing map api来求。
+                else:     
                     if (latitude, longitude) not in coord_city_dic:
                         location = geolocator.reverse((latitude, longitude))
                         cityName= ' '
                         if location:
                             try:
                                 cityName = location.raw['address']['adminDistrict2']+ ', '+ location.raw['address']['countryRegion']
                             except:
                                 cityName = location.address
-                        time.sleep(0.15)     # Bing map API限速
+                        time.sleep(0.15)     
                         coord_city_dic[(latitude, longitude)]= cityName
                     else:
                         cityName= coord_city_dic[(latitude, longitude)]
                 res[ip]= [latitude, longitude, cityName]
                     
                 logger.info(f'done: {count} coord2city')
                 count+=1
             reader.close()
             return res
 
-    
+    @staticmethod
+    def cal_geo_dist(lat1, lon1, lat2, lon2):
+        '''
+        - description: 计算两坐标地理距离
+        '''
+        import math
+        R = 6371
+        dLat = math.radians(lat2 - lat1)
+        dLon = math.radians(lon2 - lon1)
+        lat1 = math.radians(lat1)
+        lat2 = math.radians(lat2)
+        a = math.sin(dLat/2) * math.sin(dLat/2) + math.sin(dLon/2) * math.sin(dLon/2) * math.cos(lat1) * math.cos(lat2)
+        c = 2 * math.atan2(math.sqrt(a), math.sqrt(1-a))
+        distance = R * c
+        return distance
+
+
 class PeersData(object):
-    '''收集RIPE-NCC和RouteViews项目中的peers信息, 用于观察peers分布等'''
+    '''收集RIPE-NCC和RouteViews项目中的peers信息'''
 
     @staticmethod
     def fromRV():
         '''
         - description: 采集来自RV的原始数据, 删了peerIP-v6部分
         - 注意：
             - `http://www.routeviews.org/peers/peering-status.html`仅展示32个采集点
                 - 包括`route-view, route-views6`
             - `http://archive.routeviews.org/`数据库展示了37个采集点
                 - 不包括`route-view`
                 - 包括`route-views6`和6个新增点`jinx,saopaulo,seix,mwix,bdix,ny`
-            - 当前函数仅收录31个采集点，即`32 - route-views6`, 因为那个点只含peerIP-v6
+            - 当前函数仅收录31个采集点，因为'route-views6'只含peerIP-v6
         - return {dict}: `{ collector: {ip1: {'asn':, 'ip':, 'v4_pfx_cnt': }, ip2: {},...}, ...}`
         - return {list}: `[ip, ...]`
         '''
         url= "http://www.routeviews.org/peers/peering-status.html"
         resRV={}
         respon= requests.get(url).text
         if not respon:
@@ -147,15 +161,14 @@
             return {}, []
         rawList= re.findall('route-view.+', respon)
         
         IPs= set()
         for row in rawList:                       
             rowlist= row.split()
             if ':' in rowlist[2]:   
-                # 把peerIP-v6排除
                 continue
             
             collector= re.search('.*(?=.routeviews.org)', rowlist[0]).group()
             if collector not in resRV.keys():
                 resRV[collector]= {}
                 #logger.info('start collecting with %s ~' % collector)
 
@@ -188,92 +201,85 @@
                     IPs.add( peer['ip'])
             data_new[rrc]= peer_lis_new
         return data_new, list(IPs)
 
     @staticmethod
     def get_peers_info(path_out= 'peers_info.json'):
         '''
-        - description: 获取所有peers的信息. 
-        - 结果存储在`./peers_info.json`
+        - description: 获取所有peers的信息, 结果存储在`./peers_info.json`
         - return {dict}: `{ 'rou': [{'asn', 'ip', 'v4_prefix_count', 'longitude', 'latitude', 'collector'}, {}, ...],
                             'rrc': [...] }`
         '''
         rv_info, rv_ips= PeersData.fromRV()
         rc_info, rc_ips= PeersData.fromRRC()
 
         ip_map= CommonTool.ip2coord(set(rv_ips+ rc_ips))
 
         res={}
         for data in (rv_info, rc_info):
             cur_res= []
-            # 3. 把坐标属性并入peer字典
             for rrc, rrc_dic in data.items():
                 for ip, peer_dic in rrc_dic.items():
                     peer_dic['latitude']=  ip_map[ip][0]
                     peer_dic['longitude']= ip_map[ip][1]
                     peer_dic['cityName'] = ip_map[ip][2] if ip_map[ip][2]!= None else ' '
                     peer_dic['collector']= rrc
                     cur_res.append(peer_dic)
 
-            # 4. 并入颜色属性到字典
-                # 下标对应采集点的编号
             colors = [
                 '#1F75FE', '#057DCD', '#3D85C6', '#0071C5', '#4B86B4',
                 '#17A589', '#52BE80', '#2ECC71', '#00B16A', '#27AE60',
                 '#E74C3C', '#FF5733', '#C0392B', '#FF7F50', '#D35400',
                 '#9B59B6', '#8E44AD', '#6A5ACD', '#7D3C98', '#BF55EC',
                 '#E67E22', '#FFA500', '#FF8C00', '#FF6347', '#FF4500',
                 '#F1C40F', '#FFD700', '#F0E68C', '#FFA07A', '#FFB900',
                 '#555555', '#BDC3C7', '#A9A9A9', '#D3D3D3', '#808080'
             ]
-                # 把采集点名字映射为下标
+            
             collector2idx= { val: idx for idx, val in enumerate( list(data.keys())) }
             for peer in cur_res:
                 peer['color']= colors[collector2idx[ peer['collector'] ]]
 
             key= list(data.keys())[0][:3]
             res[ key]= cur_res
 
-        # 5. 导出
         with open(path_out, 'w') as f:
             json.dump(res, f)
         logger.info( f"rrc: {len( res['rrc'])} peers.\nrou: {len( res['rou'])} peers.\n### all peers info stored at `{path_out}`")
 
         return res
 
     @staticmethod
     def get_rrc_info(path_in= './peers_info.json', path_out= 'peers_info_about_collector.csv'):
         '''
-        - description: 获取每个rrc的peers数量、城市列表. 这是对`get_peers_info()`输出的汇总。
+        - description: 获取每个rrc的peers数量、城市列表
         '''
         if not os.path.exists(path_in):
             PeersData.get_peers_info()
         with open(path_in) as f:
             datas= json.load(f)
         datas= datas['rou']+ datas['rrc']
-
-        # 得到每个rrc所在城市的列表
+        
         rrc_city= {}
         rrc_count= []
         for dic in datas:
             rrc_count.append( dic['collector'])
 
             if not dic['collector'] in rrc_city.keys():
                 rrc_city[dic['collector']]= [ dic['cityName'] ]
             else:
                 if dic['cityName']!= ' ':
                     rrc_city[dic['collector']].append( dic['cityName'])
 
-        # 得到RRC的规模（拥有多少peer）
         peer_num_in_RRC= pd.value_counts(rrc_count).sort_index().to_frame()
-        # 得到RRC的城市的去重列表
+        
         for rrc, city_lis in rrc_city.items():
             rrc_city[rrc]= [str(set(city_lis))]
         rrc_city_pd= pd.DataFrame(rrc_city).T
-        # 合并上述两列
+        
         res= pd.concat([peer_num_in_RRC, rrc_city_pd], axis=1)
         res.to_csv(path_out, header=['peer_num', 'cities'])
 
     @staticmethod
     def prepare_peer_worldMap(path_in= './peers_info.json', path_out= './peers_info_for_drawing.json'):
         '''
         - description: 调整peers_info数据格式，用于eChart作图。
@@ -293,22 +299,17 @@
                     p.pop(k)
                 data_new.append(p) 
             data_all[ project ]= data_new
 
         with open(path_out,'w') as f:
             json.dump(data_all, f)
 
-    #TODO: 针对两个项目中为公开peers的采集点，如何得到其peers和相应的地理信息？
-    #       考虑从采集点的RIB表中收集。
-    def get_peers_from_rib(rib_path):
-        pass
-
     @staticmethod
     def peerAS2country(project= 'rrc', p= './peers_info.json'):
-        '''- 获取每个国家的peers数量。可用于量化‘peers在欧美与非欧美国家间分布严重不均匀’'''
+        '''- 获取每个国家的peers数量'''
         if not os.path.exists(p):
             PeersData.get_rrc_info()
         with open(p) as f:
             data= json.load(f)[project]
         aa= pl.DataFrame(data)[['asn', 'cityName']]
         aa['cityName']= aa['cityName'].str.split(', ').arr.last()
         a_=aa.groupby('asn').agg(
@@ -316,21 +317,50 @@
         ).groupby('country').agg(
             pl.col('asn').count()
         ).sort('asn',reverse=True)
         return a_
     
     @staticmethod
     def _get_country_name(code):
-        '''-input国家代码; output国家名'''
+        '''-input国家代码, output国家名'''
         try:
             country = pycountry.countries.get(alpha_2=code)
             return country.name
         except:
             return None
 
+    @staticmethod
+    def get_peers_distance_DF(path= './peers_info.json', df_out_path= './peers_distance_each_other.csv'):
+        '''
+        - description: 计算peers两两之间的地理距离
+        - `peers_info.json`的数据源: peerIP来自`http://www.routeviews.org/peers/peering-status.html`和`https://www.ripe.net/analyse/internet-measurements/routing-information-service-ris/archive/ris-raw-data`
+                                    坐标来自`https://ipinfo.io/{ip}`
+        '''
+        with open(path) as f:
+            data= json.load(f)
+        coords= {'asn':[], 'latitude':[], 'longitude':[]}
+        for dic in data['rou']+data['rrc']:
+            coords['asn'].append( f"AS{dic['asn']}-{dic['collector'][:3]}")
+            coords['latitude'].append( float(dic['latitude']))
+            coords['longitude'].append( float(dic['longitude']))
+
+        peer_num  = len(coords['latitude'])
+        distances = np.zeros((peer_num, peer_num))
+        for i in range(peer_num):
+            for j in range(i, len(coords['latitude'])):
+                lat1, lon1 = coords['latitude'][i], coords['longitude'][i]
+                lat2, lon2 = coords['latitude'][j], coords['longitude'][j]
+                d = CommonTool.cal_geo_dist(lat1, lon1, lat2, lon2)
+                distances[i][j] = d
+                distances[j][i] = d
+
+        df = pd.DataFrame(distances, index=coords['asn'], columns=coords['asn'])
+        df.to_csv(df_out_path, index=True)
+        return df
+
 
 #######################
 # 分析MRT原始数据相关接口
 #######################
 
 class MRTfileHandler():
     '''用于处理RIPE和RouteViews项目中的MRT格式数据'''
@@ -338,32 +368,37 @@
     @staticmethod
     def collector_list(project=None):
         '''
         - description: 获取采集点列表。
         - args-> project {*}: one of `RIPE, RouteViews` or None
         - return {list}
         '''
-
-        # 26个采集点
+        
         collector_list_rrc= [f'rrc{i:02d}' for i in range(27)]
         collector_list_rrc.pop(17)
-        # 38个采集点
-        collector_list_rou= ["route-views.ny","route-views2","route-views.amsix","route-views.chicago","route-views.chile","route-views.eqix","route-views.flix","route-views.fortaleza","route-views.gixa","route-views.gorex","route-views.isc","route-views.jinx","route-views.kixp","route-views.linx","route-views.napafrica","route-views.nwax","route-views.perth","route-views.phoix","route-views.rio","route-views.saopaulo","route-views.sfmix","route-views.sg","route-views.soxrs","route-views.sydney","route-views.telxatl","route-views.wide","route-views2.saopaulo","route-views3","route-views4","route-views5","route-views6","route-views.peru","route-views.seix","route-views.mwix","route-views.bdix","route-views.bknix","route-views.uaeix","route-views"]
+        
+        collector_list_rou= ["route-views.ny","route-views2","route-views.amsix","route-views.chicago","route-views.chile",
+        "route-views.eqix","route-views.flix","route-views.fortaleza","route-views.gixa","route-views.gorex","route-views.isc",
+        "route-views.jinx","route-views.kixp","route-views.linx","route-views.napafrica","route-views.nwax","route-views.perth",
+        "route-views.phoix","route-views.rio","route-views.saopaulo","route-views.sfmix","route-views.sg","route-views.soxrs",
+        "route-views.sydney","route-views.telxatl","route-views.wide","route-views2.saopaulo","route-views3","route-views4",
+        "route-views5","route-views6","route-views.peru","route-views.seix","route-views.mwix","route-views.bdix",
+        "route-views.bknix","route-views.uaeix","route-views"]
         
         if project== 'RIPE':
             return collector_list_rrc
         elif project== 'RouteViews':
             return collector_list_rou
         else:
             return collector_list_rrc+ collector_list_rou
     
     @staticmethod
     def get_download_url(type:str, monitor:str, tarTime):
         '''
-        - description: 获取MRT文件下载链接。注意, 得到的链接可能404
+        - description: 获取MRT文件下载链接
         - args-> type {str}: any of `updates, rib, rib., ribs, bview, bview.`
         - args-> monitor {str}: 
         - args-> tarTime {str| datetime}: like `20210412.0800`
         - return {str}
         '''
         if isinstance(tarTime, datetime):
             tarTime= tarTime.strftime('%Y%m%d.%H%M')
@@ -391,41 +426,46 @@
         elif size_str.endswith('M'):
             return float(size_str[:-1])
         elif size_str.endswith('K'):
             return float(size_str[:-1]) / 1000
         elif size_str[-1] == 'G':
             return float(size_str[:-1])*1000
         else:
-            return float(size_str)
+            return float(size_str)/10**6
     
     @staticmethod
     def _get_month_list(time_start='20210416', time_end='20210718'):
         '''- 获取指定时间段内的月份列表，如：['2021.04', '2021.05',...]'''
-        
+        t1= time.time()
         # Convert the start and end dates to datetime objects
         start_date = datetime.strptime(time_start[:8], '%Y%m%d')
         end_date = datetime.strptime(time_end[:8], '%Y%m%d')
 
         # Generate a list of months between the start and end dates
         month_list = []
         while start_date <= end_date:
             month = start_date.strftime('%Y.%m')
             if month not in month_list:
                 month_list.append(month)
             start_date += timedelta(days=1)
+        print(f"time cost for getting `months_list`: {(time.time()-t1):.1f} s")
         return month_list
 
     @staticmethod
-    def _get_collector_file_size(collector, month_list) -> dict:
+    def _get_collector_file_size(collector, month_list=None) -> dict:
         '''
         - description: 从一个collector获取指定`月份`内的`MRT file size`的变化
         - args-> collector {str}: 
         - args-> month_list {list}: from `_get_month_list()`
-        - return {dict}: like: {collector: {'20210401.0000': '6M', '20210401.0005': '5M',...} }, value可能为空
+        - return {dict}: like: {collector: {'20210401.0000': '6M', '20210401.0005': '5M',...} }, value可为空
         '''
+        if not month_list:
+            collector, month_list= collector
+            month_list= [month_list]
+            
         diveded_map={'rrc':5, 'rou':15}
         pattern_dir={
             'rrc': r'href="updates\.(\d{8}\.\d+)\.gz.*:\d\d\s*(\d+\.?\d*[MKG]?)\s*', 
             'rou': r'updates\.(\d{8}\.\d+)\.bz2.*"right">\s*(\d+\.?\d*[MKG]?)\s*'
         }
         res_dic= {}
 
@@ -434,53 +474,76 @@
                 url= f'https://data.ris.ripe.net/{collector}/{month}/'
             else:
                 if collector== 'route-views2':
                     url= f'http://archive.routeviews.org/bgpdata/{month}/UPDATES/'
                 else:
                     url= f'http://archive.routeviews.org/{collector}/bgpdata/{month}/UPDATES/'
 
-            pageInfo= requests.get(url).text
-            matches= re.findall(pattern_dir[collector[:3]], pageInfo)
-            for time, size in matches:
-                # 很烦心的一个事：两个数据集中的时间格式并不是完全按照每5/15分钟一跳来存储MRT文件的。
-                # 在此我通过删除不能被5/15整除的时间，来简单地排除异常。
-                if int(time[-2:])% diveded_map[collector[:3]] ==0:
-                    res_dic[time]= size
+            try:
+                respon= requests.get(url, timeout= 4)
+                if respon.status_code==200:
+                    pageInfo= respon.text
+                else:
+                    print(f'请求失败: {collector}--> {url}')
+            
+                matches= re.findall(pattern_dir[collector[:3]], pageInfo)
+                for time, size in matches:
+                    if int(time[-2:])% diveded_map[collector[:3]] ==0:
+                        res_dic[time]= size
+            except Exception as e:
+                print(f'请求异常：{collector}--> {e}')
 
-        #logger.info(f'* * done: {collector}')
+        # print(f'* * done: {collector}')
         return {collector: res_dic}
 
     @staticmethod
-    def _get_collectors_file_size(time_start='20211004.1200', time_end=None, project=None):
+    def _get_collectors_file_size(time_start='20211004.1200', time_end=None, project=None, custom_rrcs= None):
         '''
         - description: 并行使用`_get_collector_file_size`。返回值排除了空数据的采集点。
         - args-> project {str}: either-or of 'RouteViews' and 'RIPE'
+        - args-> custom_rrcs {list}: 自定义采集点列表
         - return {dict}: `{'rrc': DF(collectors* dates), 'rou': ~same~}`
         '''
         if time_end==None:
             time_end= time_start
-        proj_map  = {'RouteViews': MRTfileHandler.collector_list('RIPE'), 'RIPE': MRTfileHandler.collector_list('RouteViews')}
-        collector_list= proj_map[project] if project else proj_map['RIPE']+ proj_map['RouteViews']
+        proj_map  = {'RouteViews': MRTfileHandler.collector_list('RouteViews'), 'RIPE': MRTfileHandler.collector_list('RIPE')}
+        if custom_rrcs:
+            collector_list= custom_rrcs
+        else:
+            collector_list= proj_map[project] if project else proj_map['RIPE']+ proj_map['RouteViews']
         month_list= MRTfileHandler._get_month_list(time_start, time_end)
+        
+        from tqdm import tqdm
+         
+        with Pool(processes=50) as pool:
+            total = len(collector_list)* len(month_list)
+            candi_list= [(c, m) for c in collector_list for m in month_list ]
+            desc = 'Processing collector files'
+            results = list(tqdm(pool.imap(MRTfileHandler._get_collector_file_size, candi_list), total=total, desc=desc))
 
-        # 并行获取每个collector的数据
-        with Pool(processes = 54) as pool:
-            results= pool.map(partial(MRTfileHandler._get_collector_file_size, month_list= month_list), collector_list)
-
-        # 处理汇总数据
         res= {}
         res_rrc= {}
         res_rou= {}
         for r in results:
-            if 'rrc' in list(r.keys())[0]:
-                res_rrc.update(r)
+            rrc_name= list(r.keys())[0]
+            if 'rrc' in rrc_name:
+                if rrc_name in list(res_rrc.keys()):
+                    res_rrc[rrc_name].update( r[rrc_name])
+                else:
+                    res_rrc.update(r)
             else:
-                res_rou.update(r)
+                if rrc_name in list(res_rou.keys()):
+                    res_rou[rrc_name].update( r[rrc_name])
+                else:
+                    res_rou.update(r)
+                    
         for dic in [res_rou, res_rrc]:
-            # 压缩日期到数天，并统一单位
+            if dic=={}:
+                continue
+            
             df= pd.DataFrame(dic )#.astype(str)
             df.sort_index()
             df.index = pd.to_datetime(df.index, format='%Y%m%d.%H%M')
             a= datetime.strptime(time_start, '%Y%m%d.%H%M')
             b= datetime.strptime(time_end, '%Y%m%d.%H%M')
             df = (df.loc[(df.index >= a) & (df.index <= b)]
                     .fillna('0')
@@ -502,36 +565,42 @@
             print(f'`{low_var_collectors=}`')
                             
             res[list(dic.keys())[0][:3]]= df
             
         return res
 
     @staticmethod
-    def draw_collectors_file_size(eventName='', time_start='20211004.1200', time_end=None, event_period=None):
+    def draw_collectors_file_size(eventName='', 
+        time_start='20211004.1200', 
+        time_end: str=None, 
+        event_period: tuple=None,
+        project: str= None,
+        custom_rrcs: list= None
+        ):
         '''
-        - description: 画图对比各采集点的`file_size`走势。有图像导出。
+        - description: 画图对比各采集点的`file_size`走势
         - args-> data {*}: all of values returned by `_get_collectors_file_size()`
         - args-> event_period {`('20211004.1200', '20211004.1200')`}: 当需要在图中作异常区间阴影时使用
         - return {*}
         '''
         if time_end== None:
             time_end= time_start
         #if not data:
-        data= MRTfileHandler._get_collectors_file_size(time_start, time_end)
+        data= MRTfileHandler._get_collectors_file_size(time_start, time_end,project= project, custom_rrcs= custom_rrcs)
         
         for project, df in data.items():
             #size_map= {'RIPE': 23, 'RouteViews': 32}
             print(f'{df.shape=}')
             title= f"{time_start[:8]}_{eventName}_{project}.jpg"
             utils.makePath(f'plot_file_sizes/{title}')
             ax= df.plot( # y=df.columns[3],
                     figsize=(10, df.shape[1]),
-                    subplots=True
+                    subplots=True 
             )
-            # 有并列子图时的造阴影
+            
             if event_period != None:
                 sat= datetime.strptime(event_period[0], '%Y%m%d.%H%M')
                 end= datetime.strptime(event_period[1], '%Y%m%d.%H%M')
                 for a in ax:
                     a.axvspan(sat, end, color='y', alpha= 0.35)
 
             plt.savefig(title)
@@ -549,33 +618,32 @@
         '''
         if time_end== None:
             time_end= time_start
         if not data:
             data= MRTfileHandler._get_collectors_file_size(time_start, time_end)
         res= pd.Series()
         for project, df in data.items():
-            # 计算峰度
             kurt = df.apply(kurtosis)
             score = (10 * (kurt - kurt.min()) / (kurt.max() - kurt.min())).sort_values(ascending=False)
             res= pd.concat([res, score])
         res= res.sort_values(ascending=False)
         return res, data
 
 class DownloadParseFiles():
-    '''- 简单场景下的MRT文件的下载和解析操作, 含2种模式。'''
-    def __init__(self, mode= 'all', time_str= '20230228.0000', time_end= None, coll= None, target_dir= os.getcwd(), core_num= 40) -> None:
+    '''- 简单场景下的MRT文件的下载和解析'''
+    def __init__(self, mode= 'a', time_str= '20230228.0000', time_end= None, coll= None, target_dir= './raw_data/', core_num= 60) -> None:
         ''' 
         - args-> mode {'all'/'a'}: 
             - `all`: 所有采集点模式，用于下载并解析`指定时刻time_str`的`所有采集点`的(rib)表；
             - `a`  : 单一采集点模式，用于下载并解析`指定时间段time_str ~ time_end`的`指定采集点coll`的(updates)表
         - args-> time_str {*}: 
         - args-> time_end {*}: 当mode='a'时有效
         - args-> coll {*}: 当mode='a'时有效
-        - args-> target_dir {*}: cwd
-        - args-> core_num {*}: 默认40核
+        - args-> target_dir {*}: 
+        - args-> core_num {*}: 默认60核
         '''
         self.mode= mode
         self.time_str= time_str
         self.time_end= time_end
         self.coll= coll
         self.core_num= core_num
         self.p_down= utils.makePath(f'{target_dir}/raw/')
@@ -601,77 +669,72 @@
                 satTime += timedelta(seconds= interval* 60)
                 
             url_list= [ MRTfileHandler.get_download_url('updates', self.coll, n) for n in need]
 
         return url_list
 
     def _download_file(self, queue, urls:list):
-        '''- 生产者: 下载所有urls, 将下载后的路径存入queue'''
+        ''''''
         for url in urls:
             # 先判url有效性
             response = requests.head(url).status_code
             if response==404:
                 print(f"FAILD: {url=}")
             else:
                 url_nodes= url.split('/')
                 output_file = f"{ self.p_down}{url_nodes[3]}_{url_nodes[-1]}"
                 subprocess.call(['wget', '-q', '-O', output_file, url])
                 queue.put(output_file)
 
     def _parse_file(self, queue):
-        '''- 消费者: 解析queue中的数个file, 返回其路径列表'''
+        ''''''
         target_files=[]
-        while True:     # 即只要队列中还有元素，则该消费者子进程持续执行
-            source = queue.get()    # 当queue中没有元素，则会一直空转等待元素。
+        while True:      
+            source = queue.get()     
             if source== None:
                 break
             output_file= self.p_pars+ os.path.basename(source)+ '.txt'
             subprocess.call(f'bgpdump -q -m {source} > {output_file}', shell=True)
             target_files.append(output_file)
             #print(f"done : {os.path.basename(source)}.txt")
         return target_files
 
     #@utils.timer
     def run(self):
-        '''- return {list}: 解析后的所有路径
-        '''
+        
         t1= time.time()
         url_list= self._get_url_list()
-        queue= multiprocessing.Manager().Queue()    # 要用可在进程间共享的队列
+        queue= multiprocessing.Manager().Queue()     
         cores_p= self.core_num//2
         cores_c= self.core_num//2
         pool1 = multiprocessing.Pool(processes=cores_p)
         pool2 = multiprocessing.Pool(processes=cores_c)
         
-        # 生产者
         sub_set_size= round( len(url_list)/ cores_p )
         for i in range(cores_p):
             if i+1== cores_p:
                 sub_set= url_list[i*sub_set_size:]
             else:
                 sub_set= url_list[i*sub_set_size: (i+1)*sub_set_size]
             pool1.apply_async( self._download_file, (queue, sub_set))
         pool1.close()
 
-        # 消费者
         print("has parsed files:")
         with tqdm.tqdm(total= len(url_list), dynamic_ncols= True) as pbar:            
             results= []
             real_res= []
 
             for i in range(cores_c):
                 res= pool2.apply_async(self._parse_file, (queue,))
                 results.append(res)
             pool1.join()
 
-                # 添加迫使消费者结束的哨兵
             for i in range(cores_c):
                 queue.put(None)
 
-            # 等待任务完成并更新进度条
             while len(results)>0:
                 for i in range(len(results)):
                     r= results[i]
                     if r.ready():
                         results.pop(i)
                         r_= r.get()
                         real_res+= r_
@@ -687,355 +750,702 @@
         for r in results:
             real_res+= r.get()'''
         real_res= sorted(real_res)
         print(f'download and parse cost: {(time.time()-t1):.2f}s')
         return real_res
 
 class COmatrixPfxAndPeer():
-    ''' - 从所有采集点的rib表获取全局 prefix和peer_AS的共现矩阵，以得到各peer的视野大小，判断其在全球路由收集中的重要性。
-        - 前提：用`DownloadParseFiles`类下载解析全局rib表。
-        - 另：通过共现矩阵pl.df查看peerAS的视野排名:`a= df[:,1:].sum().to_pandas().T.rename(columns={0: 'pfx_num'}).sort_values('pfx_num', ascending=False)`
+    ''' - 从所有采集点的rib表获取全局 prefix和peer_AS的共现矩阵
     '''
     @staticmethod
     def _COmatrix_a_rib(path):
-        '''- 获取一张路由表中的pfx-peer_AS共现矩阵 & originAS-peer_AS共现矩阵'''
-        # 被并行的函数一定要try,不然一个断，所有进程都断了
+        
         try:
             t1= time.time()
             #logger.info('start one rib...')
             df= pl.read_csv(path, sep='|',has_header=False,  ignore_errors= True)
             df.columns= utils.raw_fields
 
             df['mask']= pl.Series([True]* df.shape[0])
-            # 获取pfx-peer_AS共现矩阵
             pfx_2_peer= df.pivot(values='mask', index='dest_pref', columns='peer_AS').fill_null(False)
             
-            #  获取originAS-peer_AS共现矩阵（可得到：一个peer在AS层面的视野范围；一个AS能被多少个peer观察到）
             oriAS_2_peer= (df.select(['peer_AS', pl.col('path').str.split(' ').arr.last().alias('origin_AS'), 'mask'])
                             .pivot(values='mask', index= 'origin_AS', columns='peer_AS').fill_null(0))
             
             #logger.info(f"done:({(time.time()-t1):.1f}sec)  {os.path.basename(path)}")
             return (pfx_2_peer, oriAS_2_peer), os.path.basename(path)
         except Exception as e:
             print(e)
             print(f'ERROR: {path}')
             return (0,0), os.path.basename(path)
 
     @staticmethod
     def _COmatrix_post_handler(df_list: List[pl.DataFrame], out_path):
-        '''
-        - description: 合并和处理各个采集点上得到的pfx2peer/ oriAS2peer共现矩阵。
-        - args-> df_list {*}: 共现df列表
-        - return {*}
-        '''
+        
         DF= df_list[0]
         index_tag= DF.columns[0]
         for id, df in enumerate(df_list[1:]):
             if isinstance(df, pl.DataFrame):
                 df.columns =[index_tag]+ [f"{col}_{id}" for col in df.columns[1:]]
                 DF= DF.join(df, on= index_tag, how= 'outer')
         DF= DF.fill_null(False)
         
-        # 此时DF的情况：行上需区分v4,v6; 列上需合并AS号相同的peer
         ASset= set()
         cols= DF.columns[1:]
         for col in cols:
             curAS= col.split('_')[0]
             if curAS not in ASset:
                 ASset.add(curAS)
                 DF= DF.rename({col: curAS})
             else:
-                DF[curAS]= DF[curAS]| DF[col]     # bool或运算
+                DF[curAS]= DF[curAS]| DF[col]      
                 DF= DF.drop(col)
-
-        #DF_v4= DF.filter(pl.col(index_tag).str.contains(':')== False)
-        #DF_v6= DF.filter(pl.col(index_tag).str.contains(':'))
         DF.select([
             pl.col('dest_pref'),
             pl.exclude('dest_pref').cast(pl.Int8)
         ]).to_csv(out_path)
 
     @staticmethod
     def get_pfx2peer_COmatrix_parall(ribs_dir='/data/fet/ribs_all_collector_20230228.0000/parsed/',out_path= './COmatrix/', processes=4):
-        ''' - 输入各个采集点rib文件的列表, 获取pfx2peer/ oriAS2peer共现矩阵
-        # TODO: 考虑改用` https://publicdata.caida.org/datasets/as-relationships/serial-1/20230301.as-rel.txt.bz2`
-        '''
+        
         utils.makePath(out_path)
         paths= sorted(glob.glob(ribs_dir+'*'))
-        #paths= [paths[8],paths[13],paths[14],paths[4]]
         
         with Pool(processes=processes) as pool: 
             results=[]
             with tqdm.tqdm(total= len(paths),dynamic_ncols= True) as pbar:
                 for result, fname in pool.imap_unordered(COmatrixPfxAndPeer._COmatrix_a_rib, paths):
                     pbar.update()
                     pbar.set_postfix_str(f"{fname}")
                     results.append( result )
 
         p2p_list, o2p_list = zip(*results)
 
         COmatrixPfxAndPeer._COmatrix_post_handler(p2p_list, out_path+'COmatrix_pfx_2_peer.csv')
         COmatrixPfxAndPeer._COmatrix_post_handler(o2p_list, out_path+'COmatrix_oriAS_2_peer.csv')
         logger.info(f"ENDING: COmatrix about prefix and peer. result path: `{out_path}`")
+    
+    @staticmethod
+    def peers_rank_from_COmat():
+        '''- 计算全球peerAS的视野排名'''
+        zz= PeerSelector._get_existing_COmat()
+
+        df= (zz.sum().to_pandas().T
+            .drop('dest_pref')
+            .reset_index()
+            .rename(columns={'index': 'peerAS', 0: 'count'})
+            .sort_values('count', ascending=False, ignore_index=True)
+        )
+        df['percent']= df['count'].apply(lambda x: '{:.2%}'.format(x/zz.shape[0]))
+        return df
+
 
 class PeerSelector():
-    '''- 用于选择最佳peer'''
+    '''- 从rib表得到peers列表'''
 
-    # 来自COmatrixPfxAndPeer类
     @staticmethod
-    def _get_existing_COmat():
-        '''- 拿到共现矩阵'''
+    def _get_existing_COmat():        
         try:
             df= pl.read_csv('/data/fet/ribs_all_collector_20230228.0000/COmatrix/COmatrix_pfx_2_peer.csv')
         except:
             print('no COmatrix!')
             df= None
         return df
     
     @staticmethod
     def _df2graph(df= None):
-        '''- 由 df['peer_AS', 'dest_pref','path'] 生成带权有向图.
-        - 效率：操作97万行的df耗时10s, 3s拿到边集合, 7s造图 '''
         all_edge= ( df
             .groupby([ 'peer_AS', 'dest_pref' ])
-                .tail(1)    # rib表中一个peer-pfx下还有多条路由，说明这个peerAS有多个peerIP，只保留一条路由即可。当然这不算严谨，可能会失去一些边关系。
+                .tail(1)     
                 .drop_nulls()
                 .select([
                 #pl.col('dest_pref'),
                 pl.col('path').str.split(' ').alias('path_list_raw'),
                 pl.col('path').str.split(" ").arr.shift( -1 ).alias('path_list_sft')
             ])
-            .explode( ['path_list_raw', 'path_list_sft'] )  # 2列展开
+            .explode( ['path_list_raw', 'path_list_sft'] )   
             .filter( (pl.col('path_list_sft') != None)&
                     (pl.col('path_list_raw') != pl.col('path_list_sft')) &
                     (~pl.col('path_list_sft').str.contains('\{'))
-                    )       # 自此，每行的2列就是拓扑图中一个边的连接关系。 
-            # .unique()       # 去重效果：去重前274万边，去重后11万边。这是因为不同路由(pfx)间有大量重复的边，特别是tier-1与运营商之间
+                    )        
+             
         ).to_numpy()
 
         G = nx.DiGraph()
         weights = {}
         for edge in all_edge:
             u, v = edge
             if (u, v) in weights:
                     weights[(u, v)] += 1
             else:
                     weights[(u, v)] = 1
                     G.add_edge(u, v, weight=1)        
-        # 更新边的权重
+         
         for u, v, w in G.edges(data='weight'):
             G[u][v]['weight'] = weights[(u, v)]
         return G
 
     @staticmethod
     def _greaterthan_avg_degree(G: nx.Graph):
-        '''- 获取`大于平均度(3种)的节点数量`'''
         _df=pd.DataFrame({    
                             'gp_nb_nodes_gt_avg_tol_degree': dict(G.degree),
                             'gp_nb_nodes_gt_avg_out_degree': dict(G.out_degree()), 
                             'gp_nb_nodes_gt_avg_in_degree': dict(G.in_degree())
                         })
         res= _df.apply(lambda x: (x > x.mean()).sum()).to_dict()
         return res
 
     @staticmethod
     def _simple_feats_graph(G: nx.Graph, source_peer):
-        '''- 获取图的一个特征字典'''
-        # 数据准备：
+        ''''''
         #Gsub, _= GraphBase.get_subgraph_without_low_degree(G)  
 
-        # 特征集合1：无需k核子图就能即时获取的
         res1= {
-            # 全图特征
-            'gp_nb_of_nodes':       len(G.nodes),           # 节点数
-            'gp_nb_of_edges':       len(G.edges),           # 边数
-            'gp_density':           nx.density(G),          # 密度
-
-            # 节点平均特征
-                ## 度相关
-            'nd_degree':            graphInterAS.avgNode(G.degree),        # 平均度
-            'nd_in_degree':         graphInterAS.avgNode(G.in_degree),   # 平均入度
-            'nd_out_degree':        graphInterAS.avgNode(G.out_degree),  # 平均出度
-            'nd_degree_centrality': graphInterAS.avgNode(nx.degree_centrality, G),   # 平均度中心性
-            'nd_pagerank':          graphInterAS.avgNode(nx.pagerank, G)
-            
-            # 混合特征：同时涉及全图特征、节点平均特征
-            
+            'gp_nb_of_nodes':       len(G.nodes),            
+            'gp_nb_of_edges':       len(G.edges),            
+            'gp_density':           nx.density(G),   
+
+            'nd_degree':            graphInterAS.avgNode(G.degree),         
+            'nd_in_degree':         graphInterAS.avgNode(G.in_degree),    
+            'nd_out_degree':        graphInterAS.avgNode(G.out_degree),   
+            'nd_degree_centrality': graphInterAS.avgNode(nx.degree_centrality, G),    
+            'nd_pagerank':          graphInterAS.avgNode(nx.pagerank, G)            
         }
-        # 特征集合2：需要K核子图才能即时获取(<1s)
+
         res2= {
-            # 
-            
-            #
             #'nd_clustering':            graphInterAS.avgNode(nx.clustering, Gsub),
             #'nd_closeness_centrality':  graphInterAS.avgNode(nx.closeness_centrality, Gsub),
             #'nd_eigenvector_centrality':graphInterAS.avgNode(nx.eigenvector_centrality, Gsub),
-            #
         }
         
         res3= PeerSelector._greaterthan_avg_degree(G)
 
         res= {
             'peer_degree': G.degree[str(source_peer)]}
         for r in [res1, res2, res3]:
             res.update(r)
         return res
 
     @staticmethod
     def select_peer_from_a_rib(path_or_df, method= 'simple'):
-        '''- 从一个rib表中选出最佳的peer, 以致最小的路由数来构建全局拓扑
+        '''- 从一个rib表中选出最佳的peer
             - args-> path_or_df {`str | pl.df`}: 
             - args-> method
-                - 当为默认值，最佳peer = 能观察到pfx的数量的peer
-                - 当为其他值，需对每个peer下的路由提取信息，分别做全球AS拓扑图，
-                根据图的属性等获取评分，分最高的peer最佳
+                - 当为默认值，最佳peer = 能观察到pfx的数量的peer（即视野）
+                - 当为其他值，需对每个peer下的路由提取信息，分别做全球AS拓扑图，根据图的属性等获取评分，分数最高的peer最佳
             - return {list}: idx=0处的peer最佳
+            - 其他方法：调用`ripeAPI.full_table_peer_list`直接获取。
         '''
-        if isinstance(path_or_df, str): # 已经解析好的rib表
+        if isinstance(path_or_df, str):  
             df= utils.csv2df(path_or_df).select(['peer_AS', 'dest_pref', 'path'])
         else:
             df= path_or_df.select(['peer_AS', 'dest_pref', 'path'])
 
         peer_list= list(
             df.groupby('peer_AS').agg(pl.col('dest_pref').unique().count())
             .sort('dest_pref', reverse=True)[:,0])
         
         if method== 'simple':
-            return peer_list
-        else:
+            return peer_list     
+        else:    
             #COmat= PeerSelector._get_existing_COmat()
             result= {}
-            for cur_peer in peer_list:  ####for
+            for cur_peer in peer_list:   
                 newdf= df.filter(pl.col('peer_AS')== cur_peer)
                 G= PeerSelector._df2graph(newdf)
                 #Gsub,_= GraphBase.get_subgraph_without_low_degree(G)
 
                 cur_res= {
-                    # peer的视野（能观察到pfx的数量）
-                    #'peer_vision': COmat[str(cur_peer)].sum() if COmat else 0,
                     'peer_vision': newdf['dest_pref'].unique().shape[0],
                     'num_route':   newdf.shape[0],}
                 cur_res.update( PeerSelector._simple_feats_graph(G, cur_peer) )
                 result[cur_peer]= cur_res
                 print(f'done: {cur_peer}')
 
-            # 获取这张路由表中，每个peer的评分
             dfscore = pd.DataFrame(result)
             dfscore = pd.DataFrame(MinMaxScaler().fit_transform(dfscore.T).T, columns=dfscore.columns)
             dfscore = dfscore.sum()
             print(f"{dfscore=}")
 
             return dfscore.idxmax()
-
-
+ 
 #######################
-# 提取特征前，预处理原始消息。因为‘路由波动造成的无效波峰’影响时序曲线的正常表达
+# 提取特征前，预处理原始消息
 #######################
 
-class UpdsMsgPreHandler():
-    '''- 提取特征前，预处理原始消息。因为‘路由波动造成的无效波峰’影响时序曲线的正常表达
+class   UpdsMsgPreHandler():
+    '''- 提取特征前，预处理原始消息
     '''
-
     @staticmethod
-    def pfx_oriAS_mapping_from_rib(rib_path= ''):
+    def pfx_oriAS_mapping_from_global_rib(rib_path= ''):
         '''
         - description: 从一张rib表获取完整的全球prefix与originAS的映射。一般选取rrc00的最新rib表。
         - args-> rib_path {path or url}: 
-            - 默认为(2G): `'https://data.ris.ripe.net/rrc00/latest-bview.gz'`
-            - 也可用RIB汇总表(5G): `https://publicdata.caida.org/datasets/as-relationships/serial-1/20230301.all-paths.bz2`
-        - 注：默认下当rib表5800万行，耗时 30~40s
-        - return {`pl.df['pfx', 'originAS']`}: 一般地, pfx有100万左右; oriAS有7.7万左右。
+            - 默认为: `'https://data.ris.ripe.net/rrc00/latest-bview.gz'`
+            - 也可考虑RIB汇总表(过大, bgpdump无法解析): `https://publicdata.caida.org/datasets/as-relationships/serial-1/20230301.all-paths.bz2`
         '''
         if rib_path=='' or rib_path.startswith('http'):
-            # 下载，解析非常耗时
             if rib_path=='':
                 url= 'https://data.ris.ripe.net/rrc00/latest-bview.gz'
             else:
                 url= rib_path
             base_name= url.split('/')[-1]
             rib_path= os.getcwd()+'/'+ base_name+ '.txt'
             os.system(f"time wget {url}; time bgpdump -m {base_name} > {rib_path}; rm {base_name}")
                     
-        # 20s, 读取
         df= utils.csv2df(rib_path)[['peer_AS', 'dest_pref', 'path']]
-        # 20s, 找到视野最大的peerAS
+        num_peer= df['peer_AS'].unique().shape[0]
+        num_pfx = df['dest_pref'].unique().shape[0]
+        print(f"在{rib_path}中, 有{num_peer}种peerAS, 有{num_pfx}种前缀。")
+        
         max_peer= (df.groupby('peer_AS').agg(pl.col('dest_pref').unique().count())
             .sort('dest_pref', reverse=True)[0,0])
-        # 1s, 拿到pfx和oriAS
+        
         df= (df.filter((pl.col('peer_AS')== max_peer))
                 .groupby('dest_pref').agg(
                     pl.col('path').last().str.split(' ').arr.last()
                 )
                 .sort('dest_pref', reverse=False)
                 .rename({'dest_pref':'pfx', 'path':'originAS'})
-                .filter(~(pl.col('originAS').str.contains('\{')))    # 过滤掉`{ASN}`的特殊情况
+                .filter(~(pl.col('originAS').str.contains('\{')))
         )
         return df
 
+    ## main steps
     @staticmethod
-    def del_useless_updmsg():
+    def peers_select_by_updates(df, topN=12):
+        
+        peerIP_rank= df.groupby('peer_IP').agg(pl.col('dest_pref').unique().count()).sort('dest_pref', reverse=True).to_pandas()#['peer_IP'][0]
+        peers_reserved= peerIP_rank['peer_IP'].tolist()[:topN]
+        df= df.filter(pl.col('peer_IP').is_in(peers_reserved))
+        return df
+
+    def find_peak(df:pl.DataFrame, coef_std= 3, coef_mean= 1, changepoint_prior_scale= 0.05):
         '''
-        - description: 删除无用的宣告消息。何为无用：属于路由波动的条目
-        - method: 
-            - 以每分钟为最小单元来判断upds中是否有`波动路由`
+        - description: 定位疑似异常峰点, 并绘图查看峰点。
+        - args-> df {}: 原始路由消息
+        - args-> coef_std {*}: `prophet超参数`, 标准差的权重，用于设置异常点阈值
+        - args-> coef_mean {*}: `prophet超参数`, 均值的权重，用于设置异常点阈值
+        - args-> changepoint_prior_scale {0-100}: `prophet超参数`, 针对预测曲线 控制算法中的拐点数量和位置的灵活性。
+                该参数越小，算法越趋向于学习平滑的拟合曲线，越大则趋向于学习波动较大的拟合曲线。
+        - return : 
+            - df {pl}: 筛选后的原始df
+            - {dict} key：`count`被判定为异常的行号/分钟序号
+            - {dict} value：`count`被判定为异常时，prophet模型的预测值
+        '''
+        from prophet import Prophet
+        event_timestamp= df[0, 'timestamp']
+        df_out= RawMrtDataAnaly(df).df
+        df= ( df_out
+            #.filter(
+            #    ( pl.col('time_bin')>=0)
+            #    &( pl.col('time_bin')<500)
+            #)
+            .groupby('time_bin', maintain_order=True).agg([
+                pl.col('timestamp').first().apply( lambda x: datetime.fromtimestamp(x, tz= timezone.utc).strftime('%Y/%m/%d %H:%M')).alias('date'),
+                pl.col('timestamp').count().alias('count')
+            ])
+            .select(pl.exclude('time_bin'))
+            .to_pandas()#.loc[:100]
+        )
 
-        - return {*}
+        cols= df.columns
+        df = df.rename(columns={cols[0]: 'ds', cols[1]: 'y'})
+        df['ds']= pd.to_datetime(df['ds'], infer_datetime_format=True)
+
+        model = Prophet(changepoint_prior_scale= changepoint_prior_scale)
+        model.fit(df)
+
+        future = model.make_future_dataframe(periods=2, freq='min')
+        forecast = model.predict(future)
+        
+        forecast_yhat= forecast['yhat'][:len(df)]
+        #df['error'] = np.abs(df['y'] - forecast_yhat)
+        df['error']= df['y'] - forecast_yhat
+        std = df['error'].std()
+        mean = df['error'].mean()
+        
+        threshold = coef_std * std + coef_mean * mean
+        
+        anomalies = df[df['error'] > threshold]
+
+        fig = plt.figure(figsize=(8, 6)) 
+        plt.plot(df['ds'], df['y'], color='black', label='Original')
+        plt.plot(forecast['ds'], forecast['yhat'], color='black', linestyle='--', label='Predicted')
+        plt.scatter(anomalies['ds'], anomalies['y'], color='grey', marker='x', label='Candidates')
+        plt.legend(loc='best')
+        plt.xlabel('Time', fontsize=12)
+        plt.ylabel('Number of messages', fontsize=12)
+        plt.xticks(fontsize=10)
+        plt.yticks(fontsize=10)
+        plt.ylim(bottom=0)
+        plt.grid(axis='y', linestyle='--', alpha=0.7)
+        plt.gca().spines['top'].set_visible(False)
+        plt.gca().spines['right'].set_visible(False)
+        plt.show()
+
+        p = f'./draw_abnormal_points_with_prophet_{event_timestamp}.png'
+        plt.savefig(p, dpi=300, bbox_inches='tight')
+
+        print(f"Peak plot stored in：{p}")
+
+        row_numbers = df[df['error'] > threshold].index.tolist()
+        #diff_values = df[df['error'] > threshold]['error_with_neg'].tolist() 
+        row_yhat= forecast_yhat[df['error'] > threshold].tolist() 
+        #return {'row_nums': row_numbers, 'row_yhat': row_yhat}
+        a= zip(row_numbers, row_yhat)
+        dic_= {tup[0]:tup[1] for tup in a}
+        return df_out, dic_
+
+    def distinguish_norm_peak(df: pl.DataFrame, peak_info: dict, global_mapping: list, thd= 0.85):
+        '''- peak clipping'''
+        
+        peak_not_event=( df
+            .filter( 
+                pl.col('time_bin').is_in(list(peak_info.keys()))
+                & (pl.col('msg_type')== 'A')
+            )
+            .with_column(
+                (pl.col('dest_pref')+pl.lit(' ')+ pl.col('originAS')).alias('pfx_oriAS')
+            )
+            .groupby('time_bin', maintain_order=True).agg([
+                (pl.col('pfx_oriAS').is_in(global_mapping).sum()/pl.col('pfx_oriAS').count()).alias('ratio_old_mapping')
+            ])
+            .filter(pl.col('ratio_old_mapping')> thd)
+            ['time_bin']
+            .to_list()
+        )
+        print(f"Suspected abnormal peaks: {len(peak_info)}; Harmless peaks: {len(peak_not_event)}")
+        return peak_not_event
+
+    @staticmethod
+    def cut_peak(df:pl.DataFrame, dic_suspi, peak_not_event):
+        '''- '''
+        a=( df.filter( pl.col('time_bin').is_in(peak_not_event)   
+            # & (pl.col('msg_type')== 'A')   
+            )
+            .groupby('time_bin').apply(
+                lambda group_df: (group_df.sample( int(dic_suspi[group_df['time_bin'][0]]), shuffle=True ) )
+            ))
+        a= df.filter(~pl.col('time_bin').is_in(peak_not_event)).vstack(a)
+
+        a= a.sort('id')
+        print(f"after clipping peaks: {a.shape=}")
+        return a
+
+    @staticmethod
+    def run_cut_peak(df:pl.DataFrame, mapping_path, coef_std, coef_mean, thd):
+        '''- main func'''
+        global_mapping= UpdsMsgPreHandler.pfx_oriAS_mapping_from_global_rib(mapping_path)
+
+        df= UpdsMsgPreHandler.peers_select_by_updates(df)
+        df, dic_suspi= UpdsMsgPreHandler.find_peak(df, coef_std= coef_std, coef_mean=coef_mean)
+        lis_peak_normal= UpdsMsgPreHandler.distinguish_norm_peak(df, peak_info= dic_suspi, global_mapping=global_mapping,thd= thd)
+        df= UpdsMsgPreHandler.cut_peak(df, dic_suspi, lis_peak_normal)
+
+        df_plot= ( df
+            #.filter(
+            #    ( pl.col('time_bin')>=0)
+            #    &( pl.col('time_bin')<500)
+            #)
+            .groupby('time_bin', maintain_order=True).agg([
+                pl.col('timestamp').first().apply( lambda x: datetime.fromtimestamp(x, tz= timezone.utc).strftime('%Y/%m/%d %H:%M')).alias('date'),
+                pl.col('timestamp').count().alias('count')
+            ])
+            .select(pl.exclude('time_bin'))
+            .to_pandas()#.loc[:100]
+        )
+        df_plot['date']= pd.to_datetime(df_plot['date'], infer_datetime_format=True)
+        print('See the effect after peak shaving: ')
+        df_plot.set_index('date').plot(figsize=(8,6))
+
+        return df
+
+
+class RawMrtDataAnaly():
+    '''- 从原始updates路由数据中分析事件, 基于`pl.expr`'''
+
+    def __init__(self, df:pl.DataFrame) -> None:
+        
+        first_ts= df[0, 'timestamp']
+        self.df= (df
+            .filter(pl.col('msg_type')!= 'STATE')
+            .with_columns([
+                ((pl.col('timestamp')- first_ts)// 60).cast(pl.Int16).alias('protocol'),
+                pl.col('path').str.replace(' \{.*\}', '')
+            ])
+            .with_column(pl.col('path').str.split(' ').arr.last().alias('originAS'))
+            .rename({'protocol': 'time_bin'})
+            .with_row_count('id')
+            #.groupby('time_bin')
+        )
+        
+        full_table_peer= ripeAPI.full_table_peer_list( datetime.fromtimestamp(first_ts).strftime('%Y-%m-%dT%H:%M'))[0]
+        full_table_peer= [tup[1] for tup in full_table_peer]
+        _, peer_reserve= self.list_peers_rank()
+        
+        self.figsize= (8,6)
+        self.ts2dt_str= pl.col('timestamp').first().apply( lambda x: datetime.fromtimestamp(x, tz= timezone.utc).strftime('%Y/%m/%d %H:%M')).alias('date')
+        self.filter_dict={
+            'full-table': pl.col('peer_IP').is_in(full_table_peer),     
+            'num_gt_5pmin': pl.col('peer_IP').is_in(list(peer_reserve)), 
+        }
+
+    def _fmt_sci(self):
+        '''- set the axis'''
+        formatter = ticker.ScalarFormatter(useMathText=True)
+        formatter.set_scientific(True)
+        formatter.set_powerlimits((-2, 2))
+        return formatter
+    def _fmt_date(self, ax, str_fmt= '%dT%H'):
+        '''- set the format of date scale'''
+        date_format = DateFormatter(str_fmt)
+        date_locator = AutoDateLocator()
+        ax.xaxis.set_major_locator(date_locator)
+        ax.xaxis.set_major_formatter(date_format)
+    def _set_titles(self,ax, title=None, xlabel=None, ylabel=None):
+        if title:
+            ax.set_title(title)
+        if xlabel:
+            ax.set_xlabel(xlabel)
+        if ylabel:
+            ax.set_ylabel(ylabel)
+        
+    def TS_whole(self, out_file_name= None, filter_expr= None):
+        '''- 总览消息量的走势'''
+        if isinstance(filter_expr, pl.Expr):
+            ldf= self.df.lazy().filter(filter_expr)
+        else:
+            ldf= self.df.lazy()
+            
+        df= (ldf
+            .groupby(['time_bin'], maintain_order=True)
+            .agg([
+                self.ts2dt_str,
+                pl.col('timestamp').count().alias('count')
+            ])
+            .sort('time_bin')
+            #.select(pl.exclude('time_bin'))
+            .collect()
+            .to_pandas()
+            #.set_index('date')
+        )
+
+        df['date'] = pd.to_datetime(df['date'], infer_datetime_format=True)
+
+        plt.style.use('seaborn-v0_8-paper')
+        fig, ax = plt.subplots(figsize= self.figsize)
+        ax.plot(df['date'], df['count'], color='b', linewidth=2)
+
+        self._set_titles(ax,'number of updates', 'Date', 'Count')
+        #self._fmt_date(ax)
+        ax.yaxis.set_major_formatter(self._fmt_sci())
+        fig.tight_layout()
+        if out_file_name:
+            plt.savefig(f"{out_file_name}.jpg", dpi=300)
+        
+        plt.show()
+        return df
+
+    def TS_AW_compare(self, out_file_name= None, filter_expr= None):
+        '''- 对比宣告、撤销消息量的走势'''
+        if isinstance(filter_expr, pl.Expr):
+            ldf= self.df.lazy().filter(filter_expr)
+        else:
+            ldf= self.df.lazy()
+        df_= (ldf
+            .groupby(['msg_type','time_bin'], maintain_order=True)
+            .agg([
+                self.ts2dt_str,
+                pl.col('timestamp').count().alias('count')
+            ])
+            .sort('time_bin')
+            #.select(pl.exclude('time_bin'))
+            .collect()
+            .to_pandas()
+            #.set_index('date')
+        )
+        df_['date'] = pd.to_datetime(df_['date'], infer_datetime_format=True)
+
+        grouped = df_.groupby(['msg_type']).groups
+
+        plt.style.use('seaborn-v0_8-paper')
+        fig, ax = plt.subplots(figsize= self.figsize)
+        linestyle= {'A': '-', 'W':'--'}
+        for msg_type, idxs in grouped.items():
+            x= df_.loc[idxs, 'date']
+            y= df_.loc[idxs, 'count']
+            ax.plot(x, y, label= msg_type, linewidth=1, linestyle=linestyle[msg_type], color='black')    #  s=3,
+            ax.legend()
+        try:
+            start_date= df_.loc[(df_['msg_type']=='A'),:].iloc[125, 2]
+            end_date  = df_.loc[(df_['msg_type']=='A'),:].iloc[185, 2]
+            print(start_date, end_date)
+            plt.fill_between(
+                df_['date'], df_['count'].min(), df_['count'].max(), 
+                where=((df_['date'] >= start_date) & (df_['date'] <= end_date)), 
+                color='gray', alpha=0.3)
+        except:
+            print('cant draw shadow')
+        self._set_titles(ax,'number of updates', 'Date', 'Count')
+        #self._fmt_date(ax)
+        ax.yaxis.set_major_formatter(self._fmt_sci())
+        fig.tight_layout()
+        if out_file_name:
+            plt.savefig(f"{out_file_name}.jpg", dpi=300)
+        
+        plt.show()
+        return df_
+
+    def TS_peer_compare(self, out_file_name= None, filter_expr= None):
+        '''- 对比各个peer消息量的走势'''
+        if isinstance(filter_expr, pl.Expr):
+            ldf= self.df.lazy().filter(filter_expr)
+        else:
+            ldf= self.df.lazy()
+
+        df_= (ldf
+            .groupby(['peer_IP','time_bin'], maintain_order=True)
+            .agg([
+                self.ts2dt_str,     
+                pl.col('timestamp').count().alias('count')
+            ])
+            .sort('time_bin')
+            #.select(pl.exclude('time_bin'))
+            .collect()
+            .to_pandas()
+            #.set_index('date')
+        )
+        df_['date'] = pd.to_datetime(df_['date'], infer_datetime_format=True)
+
+        grouped = df_.groupby(['peer_IP']).groups
+
+        plt.style.use('seaborn-v0_8-paper')
+        fig, axes = plt.subplots(nrows=len(grouped), figsize=(10, len(grouped)), sharex=True)
+        i=0
+        for peer_IP, idxs in grouped.items():
+            x= df_.loc[idxs, 'date']
+            y= df_.loc[idxs, 'count']
+            ax = axes[i]
+            ax.plot(x, y, label=peer_IP)    #  s=3,, linewidth=1
+            #ax.set_title(f'{peer_IP}')
+            #ax.set_ylabel('Count')
+            ax.legend()
+            i+=1
+              
+        fig.tight_layout()
+        if out_file_name:
+            plt.savefig(f"{out_file_name}.jpg", dpi=300)
+        
+        plt.show()
+        return df_
+
+    def list_peers_rank(self, thd_per_min= 100):
+        '''- 阈值法筛选peers'''
+        thd= self.df['time_bin'].max()* thd_per_min
+        peers_rank= self.df['peer_IP'].value_counts()
+        peers_set= set((peers_rank
+            .filter(pl.col('counts')>=thd)
+            ['peer_IP'].to_list())
+            )
+        return peers_rank, peers_set
+
+    def df_Apeer(self, out_file_name= None, filter_expr= None):
+        '''- 获取一个peer下的完整消息'''
+        if isinstance(filter_expr, pl.Expr):
+            ldf= self.df.lazy().filter(filter_expr)
+        else:
+            ldf= self.df.lazy()
+        df_= (ldf
+            .select([
+                'time_bin', 
+                self.ts2dt_str,
+                'dest_pref',
+                pl.col('path').str.extract(' (\d+)$', 1).cast(pl.Utf8).alias('loc_0'),
+                pl.col('path').str.extract(' (\d+) \d+$', 1).cast(pl.Utf8).alias('loc_1'),
+                pl.col('path').str.extract(' (\d+) \d+ \d+$', 1).cast(pl.Utf8).alias('loc_2'),
+                pl.col('path').str.extract(' (\d+) \d+ \d+ \d+$', 1).cast(pl.Utf8).alias('loc_3'),
+                pl.col('path').str.extract(' (\d+) \d+ \d+ \d+ \d+$', 1).cast(pl.Utf8).alias('loc_4'),
+                pl.col('path').str.extract(' (\d+) \d+ \d+ \d+ \d+ \d+$', 1).cast(pl.Utf8).alias('loc_5'),
+                pl.col('path').str.extract(' (\d+) \d+ \d+ \d+ \d+ \d+ \d+$', 1).cast(pl.Utf8).alias('loc_6'),
+                pl.col('path').str.extract(' (\d+) \d+ \d+ \d+ \d+ \d+ \d+ \d+$', 1).cast(pl.Utf8).alias('loc_7'),
+                pl.col('path').str.extract(' (\d+) \d+ \d+ \d+ \d+ \d+ \d+ \d+ \d+$', 1).cast(pl.Utf8).alias('loc_8'),
+            ])
+            .collect()
+            .to_pandas()
+            #.set_index('date')
+        )
+        df_['date'] = pd.to_datetime(df_['date'], infer_datetime_format=True)
+        return df_
+
+    def set_local_mapping_and_draw_Veen(self, out_file_name= None, filter_expr= None, set_global_mapping= None):
+        '''
+        - 获取pfx_oriAS映射集合, 用Venn图比较全局pfx_oriAS映射和当前映射集合的关系
         '''
-        pass
+        if isinstance(filter_expr, pl.Expr):
+            ldf= self.df.lazy().filter(filter_expr)
+        else:
+            ldf= self.df.lazy()
+        df_= set(ldf
+            .select(pl.col('dest_pref')+pl.lit(' ')+ pl.col('originAS'))
+            .collect().to_series()        )
+        print(f"当前df子集中，含pfx-oriAS映射{len(df_)} 对。")
+        
+        if set_global_mapping!= None:
+            ratio= len(df_.difference(set_global_mapping))/len(df_)
+            print(f"本地新映射占本地总映射之比：{ratio:.2%}")
+            venn2([df_, set_global_mapping], set_labels=('pfx-AS_event', 'pfx-AS_global'))
+            plt.show()
 
+        return df_
 
 #######################
 # 分析特征
 #######################
 
 class FeatMatHandler:
-    '''- 得到特征矩阵后进行的加工操作：如谱残差'''
+    '''- 谱残差'''
     @staticmethod
     def spectral_residual(data, smooth_window=1):
         '''
-        - description: 
-        - args-> data {*}: 一个特征的时序数据
         - args-> smooth_window {*}: 较大的窗口可能会捕捉到更低频的周期成分，而较小的窗口可能会捕捉到更高频的周期成分。
         - return {*}
         '''
         data_fft = fft(data)
-        # 计算幅度谱和相位谱
+        
         amplitude_spectrum = np.abs(data_fft)
         phase_spectrum = np.angle(data_fft)
         log_data = np.log(amplitude_spectrum)  
-        # 平滑幅度谱
+        
         smoothed_amplitude = np.convolve(log_data, np.ones(smooth_window) / smooth_window, mode='same')
-        # 计算谱残差
+        
         spectral_residual = log_data - smoothed_amplitude
         residual_signal = np.real(ifft(np.exp(spectral_residual + 1j * phase_spectrum)))
-        # 计算异常分数（平方值）
+        
         anomaly_scores = np.square(residual_signal)
 
         return anomaly_scores
 
 class Filter:
-    '''- 进行特征过滤。'''
+    '''- 特征过滤'''
     def __init__(self, df:pd.DataFrame):
         df= df.fillna(0.0)        
         self.df= df
         self.x= df.iloc[:,2:-1]
         self.y= df.iloc[:,-1]
 
     def variance_filter(self,thd):
-        '''- 方差过滤: excluding low variance feats, return DF filtered several feats'''
+        '''- excluding low variance feats, return DF filtered several feats'''
         selector_vt = VarianceThreshold( thd )
         x_varThd = selector_vt.fit_transform(self.x)
         return pd.DataFrame(x_varThd, columns= selector_vt.get_feature_names_out())
 
     def chi2_filter(self, x_varThd):        
         ''' 
         description: to get the filtered feats which p_value >0.05 from chi2 and the rank(descending) of all feats by chi2
-        param {*} self
-        param {DF} x_varThd
-        return {DF, DF} x_chi2[rows* new_feats], df_chi2[all_feats* 1]
         '''                
         chival, pval= chi2(x_varThd, self.y)
         k_chi2= (pval<= 0.05).sum()         # get hyperparameters: k feats to be remained after chi2 filtering
         selector_chi2 = SelectKBest(chi2, k= k_chi2)
         x_chi2= selector_chi2.fit_transform(x_varThd, self.y)
         x_chi2= pd.DataFrame(x_chi2, columns= selector_chi2.get_feature_names_out() )
 
@@ -1053,258 +1463,102 @@
         x_mic= pd.DataFrame(x_mic, columns= selector_mic.get_feature_names_out() )
                 
         df_mic= pd.DataFrame(selector_mic.scores_, columns=['score_mic'],index= selector_mic.feature_names_in_)
         df_mic= df_mic.sort_values( 'score_mic',ascending=0)
 
         return x_mic, df_mic
 
-    '''def RFE_filter(self, x_varThd):
-        svc= SVC( kernel='linear')
-        rfecv= RFECV(estimator= svc, 
-            step=1, 
-            cv= StratifiedKFold(2), 
-            scoring= 'accuracy', 
-            min_features_to_select=1)
-        rfecv.fit(x_varThd, self.y)
-        return rfecv'''
-
     def redu_filter(self, x_flted1: pd.DataFrame, df_ranked1: pd.DataFrame, redu_thd: float):
         '''
         description: filter redundant feats by deleting corr between feats
-        param {*} self
-        param {pd} x_flted1     : [rows*part_feats]
-        param {pd} df_ranked1   : [all_feats*1]
-        param {float} redu_thd
-        return {pd} rele_table  : [num of deleted feats* 3]
-        return {pd} x_del_corr  : [rows*part_feats]
         '''
         df_corr= abs(x_flted1.corr(method= 'spearman'))
         df_corr_= df_corr[df_corr> redu_thd]
         df_corr_= pd.DataFrame( np.tril(df_corr_.values, -1), index= df_corr_.index, columns= df_corr_.columns)
         df_corr_= df_corr_.replace(np.nan, 0)
 
         #fig= plt.figure(figsize=(10,8))
         #sns.heatmap(df_corr_, annot= False)
-        rele_table=[]   # 相关系数(spearman)高的特征对的集合, (相关系数，feat1(to del), feat2(to save))
+        rele_table=[]   
         li_ranked1= df_ranked1.index.tolist()
 
         while df_corr_.sum().sum()> 0:
             cur_arr= df_corr_.values
             max_val= cur_arr.max()
             max_idx= np.unravel_index(cur_arr.argmax(), cur_arr.shape)
             feat1= df_corr_.index[max_idx[0]]
             feat2= df_corr_.columns[max_idx[1]]
             tar_col, tar_col2= (feat1, feat2) if li_ranked1.index(feat1)> li_ranked1.index(feat2) else (feat2,feat1)
             rele_table.append( (max_val, tar_col, tar_col2))
 
             df_corr_= df_corr_.drop(index= tar_col, columns= tar_col)
-                # 精简x特征子集并验证其模型效果
+            
         new_cols= df_corr_.columns
         x_del_corr= x_flted1[new_cols ]
         # cross_val_score(RFC(n_estimators=10,random_state=0),x_del_corr ,y,cv=5).mean()
 
         rele_table= pd.DataFrame(rele_table, columns=['corr', 'feat_del', 'feat_save'])
         return rele_table, x_del_corr
                 
     def get_redu_thd(self, x_flted1: pd.DataFrame, df_ranked1: pd.DataFrame):
         '''
         description: to find hyperparameters redundant threshold in df.corr()
-        return {*} max_thd
-        return {list(tuple)} mdl_score  : for plotting to find max_thd
         '''
         mdl_score= []
         for thd in np.arange(0,1, 0.01):
             _, x_new= self.redu_filter(x_flted1, df_ranked1, redu_thd= thd)
             score= cross_val_score(RFC(n_estimators=10,random_state=0),x_new ,self.y,cv=5).mean()
             mdl_score.append( (thd, score) )
         max_thd= max(mdl_score, key= lambda x: x[1])[0]
 
         return max_thd, mdl_score
 
     def run(self):
         x_varThd= self.variance_filter()
         x_chi2, df_chi2= self.chi2_filter(x_varThd)
-        max_thd, mdl_score= self.get_redu_thd( x_chi2, df_chi2)
-        rele_table, x_del_corr= self.redu_filter( x_chi2, df_chi2, redu_thd= max_thd)
-        return df_res
+        #max_thd, mdl_score= self.get_redu_thd( x_chi2, df_chi2)
+        #rele_table, x_del_corr= self.redu_filter( x_chi2, df_chi2, redu_thd= max_thd)
+        return df_chi2
 
 
 def txt2df(paths: Union[str, list], need_concat:bool= True):
     '''
-    - description: 读取数据文件为pandas.df对象。
-    - args-> `paths` {*}: 若为str, 则为一个文件路径;若为list, 则为一组文件路径, 可选择concat为一个df, 或输出一组df
-    - args-> `need_concat` {bool}: 
-    - return {*} 一个df (来自一个文件, 或多个文件的合并); 一组df (来自多个文件分别读取)
+    - description: 读取数据文件为pandas.df对象
     '''
     if isinstance(paths, str):
         df= pd.read_csv(paths)
         return df
     if isinstance(paths, list):
         df_list= []
         for path in paths:
             df_list.append( pd.read_csv(path))
         if need_concat:
             df= pd.concat(df_list, ignore_index=True)
-
-            # 合并后的大帧做些修改
+            
             df['time_bin']= df.index
-            label_map= {'normal': 0, 'hijack': 1, 'leak': 1, 'outage': 1}   # 简化为二分类问题
+            label_map= {'normal': 0, 'hijack': 1, 'leak': 1, 'outage': 1}
             df['label']= df['label'].map( label_map )
 
             return df
         else:
             return df_list
 
 
 def df2Xy(df, test_size= 0):
-    '''- arg(df): 一般第1,2列为time_bin和date, 最后一列为label
-       - 有归一化操作。
-       - return: 4个子df/series, 即X_train/test, y_train/test; 或2个df/series, 即 X,y (默认, test_size=0)'''
-    # load the time series data
+    '''- Split training and testing sets'''
     df = df.iloc[:, 2:]
-
-    # separate the input and output columns
     X = df.iloc[:, :-1]
     y = df.iloc[:, -1]
 
     if test_size==0:
         return X, y
     else:
-        # split the data into train and test sets
-        X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=test_size, shuffle=True)  # 打乱后，逻辑回归的模型效果原地起飞
-        # normalize the data
+        X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=test_size, shuffle=True)
         scaler = StandardScaler()
         X_train = scaler.fit_transform(X_train)
         X_test = scaler.transform(X_test)
 
         return X_train, X_test, y_train, y_test
 
-
-def multi_collector_plot(event_path:str):
-    '''针对单事件、多采集器的数据。把多采集器的数据整合到一个大图的多个子图中
-    - arg: 事件的任意一个数据文件的路径'''
-    import matplotlib.pyplot as plt
-    import os
-    # 先拿到事件相关的所有文件
-    event_name= event_path.split('__')[-2]
-    dir_name  = os.path.dirname(event_path)
-    lis= os.listdir(dir_name )
-    lis= [ dir_name+'/'+ s for s in lis if event_name in s ]
-    lis.sort()
-    lis= lis[:]     # 自定义裁剪df个数
-
-    # 后作大图: 子图矩阵整合的形式
-    nrows= 9; ncols= 2
-    fig, axes= plt.subplots(nrows= nrows, ncols= ncols, figsize= (10,10) )     # 
-    
-    plt.suptitle( event_name, fontsize=14)              # 主图标题
-    #plt.subplots_adjust( top= 1)                       # 主图标题与主图上边界的距离
-
-    for i in range(nrows):
-        for j in range(ncols):
-            title= simple_plot( lis[i*2+j], axes[i][j])
-            if i == 0:
-                axes[i][j].legend(prop={'size': 6})                     # 仅在第一行的
-            if i != nrows-1:
-                axes[i][j].set_xticklabels([])          # 仅在最后一行的子图有x刻度值
-                axes[i][j].set_xlabel('')               # 仅在最后一行的子图有xlabel
-            else:
-                axes[i][j].set_xlabel('time')
-    plt.tight_layout()                                  # 自动调整整体布局
-    plt.savefig(event_name+ "18个采集器的子图矩阵对比.jpg", dpi=300)               # 高分辨率把图导出
-    
-def simple_plot(file_path:str, front_k= -1, has_label= True, subax= None, subplots= False, need_scarler= False):
-    '''针对单事件、单采集器的数据。作图观测波峰，以确定真实label'''
-    
-    # 准备图标题
-    lis= file_path.split('__')
-    try:
-        title= lis[-2]+ '__'+ lis[-1][:-4]
-    except:
-        pass
-
-    # 准备df，并预处理
-    df= pd.read_csv(file_path)
-    print(df.shape)
-        # 把日期换成只显示时分
-    df['date']= df['date'].str.slice(11, 16)
-        # 数据归一化
-    if need_scarler:
-        scaler = MinMaxScaler()
-        df.iloc[:, 2:-1]= scaler.fit_transform(df.iloc[:, 2:-1])  # 最后一列是label（str）
-    
-    # 画图
-    num_feats= len(df.columns)-2
-    if front_k==-1:
-        y= df.columns[2: ]
-    else:
-        y= df.columns[2: front_k+2]
-        num_feats= front_k
-    if not subplots:
-        num_feats= 4
-    ax= df.plot(x='date',
-            y= y,
-            #y= ['v_IGP','v_pfx_t_cnt', 'v_pp_W_cnt', 'v_A', 'is_longer_unq_path'] ,
-            #title= title,
-            figsize= (10, num_feats),
-            subplots= subplots,
-            legend= True,
-            #logy=True,
-            ax= subax,
-        )
-    #ax.set_title( title,  fontsize= 10)    # 子图标题 .split('__')[-1]
-
-        # 造阴影区域
-    if has_label:
-        rows_label= df['label'][df['label'] != 'normal'].index     #  'normal'
-        rows_label= rows_label.tolist()
-        rows_label.append(-1)
-                # 把一堆断断续续的数字变成一段一段的元组，存入 sat_end_llist
-        sat_end_list= []
-        ptr1= 0; ptr2=0
-        while ptr2< len(rows_label)-1:
-            if rows_label[ptr2]+ 1== rows_label[ptr2+1]:    # 即下一个数字是连续的
-                ptr2+=1
-                continue
-            else:
-                sat_end_list.append( (rows_label[ptr1], rows_label[ptr2]))
-                ptr2+=1
-                ptr1= ptr2
-
-                # 造多个阴影
-        '''for tup in sat_end_list:
-            ax.axvspan(tup[0], tup[-1], color='y', alpha= 0.35)'''
-
-                # 有并列子图时的造阴影
-        if subplots:
-            for a in ax:
-                for tup in sat_end_list:
-                    a.axvspan(tup[0], tup[-1], color='y', alpha= 0.35)
-
-    plt.tight_layout()
-    plt.savefig('temp.jpg', dpi=300)
-    return
-
-
-'''def collectFeat(event: list):
-    ''输入事件列表，执行特征采集全过程，存储特征矩阵为.csv''
-    ee= FET.EventEditor()
-    ee.addEvents(event)
-    
-    raw_data_path= "/data/fet/"   # "/data/fet/"    '/home/huanglei/work/z_test/Dataset/'
-    fet= FET.FET(raw_dir= raw_data_path,increment=5)
-    fet.setCustomFeats( 'ALL' )
-    p= fet.run()'''
-
-
-
-
 if __name__=='__main__':
-    # step1 看哪个rrc合适
     data= MRTfileHandler.draw_collectors_file_size('RosTel_hijack_50', '20170425.0000', '20170430.0000', ('20170426.2030','20170426.2300'))
 
-    #peer_info[0]
-
-
-
-
-
```

### Comparing `fastFET-0.0.5/fastFET/collectData.py` & `fastFET-0.0.6/fastFET/collectData.py`

 * *Files 23% similar despite different names*

```diff
@@ -75,59 +75,57 @@
                 if event[2].strip():
                     end = dt.datetime.strptime(event[2].strip(), "%Y/%m/%d %H:%M:%S")+ dt.timedelta(hours= self.increment )
                 else:
                     end = dt.datetime.strptime(event[1].strip(), "%Y/%m/%d %H:%M:%S")+ dt.timedelta(hours= self.increment+ self.duration)
 
                 for monitor in event[3:]:
                     monitor= monitor.strip()
-                    interval_upd= utils.intervalMin('updates', monitor)     # 为5 或 15
+                    interval_upd= utils.intervalMin('updates', monitor)
                     satTime, endTime= utils.normSatEndTime(interval_upd, start, end)
-                    # 如上拿到了该事件该采集器下的标准化的起止时间。此时若ribtag关，则直接导出起止时间。若开，起始时间还需往前找
                     satTime_atRIB= None
                     if self.ribTag:
-                        interval_rib= utils.intervalMin('ribs', monitor)    # 为480 或 120
+                        interval_rib= utils.intervalMin('ribs', monitor)
                         satTime_atRIB, _= utils.normSatEndTime(interval_rib, satTime, endTime)
                     res[event[0]][monitor]= [satTime, endTime, satTime_atRIB]
 
         return res
 
     def isDwlad(self, type, monitor, satTime: datetime, endTime: datetime):
-        '''- 若下载过起止时间内的文件，则返回裁剪后的文件名列表；若未下载过，返回空列表'''
+        ''''''
         try:
             ppath, _, files = os.walk(self.collection_data_lib+ monitor).__next__()
             assert len(files) != 0
             try:
-                # Note: 只选择目录中的rib或updates的一类文件。
                 files= sorted( [ f for f in files if type in f])
                 files_cuted= utils.cut_files_list(files, satTime, endTime)
                 res= [ppath+ os.sep+ file for file in files_cuted]
                 return res
             except:
                 return []
         except:
             return []
 
     def download(self, type:str, monitor:str, satTime: datetime, endTime: datetime, only_rib= None):
         '''- download files in whole day, then cut files to sat and end. 
         - arg(type): only in 'updates', 'ribs', 'all'
         - arg(satTime, endTime): datetime type or str (e.g. `'2023-02-06-00:00'`)
-        - return: cuted  raw_files, or maybe empty list (该采集器没有收录这个时间段).'''
+        - return: cuted  raw_files, or maybe empty list'''
 
         str_map= {'updates': 'updates', 'rib.': 'ribs', 'bview.': 'ribs'}
         if not isinstance(satTime, str):
             sat= satTime.strftime('%Y-%m-%d')+ "-00:00"
             end= endTime.strftime('%Y-%m-%d')+ "-23:59"
         else:
             sat= satTime
             end= endTime
-        if type!= 'updates' and only_rib== False:   # 即只下载一个rib的情况
+        if type!= 'updates' and only_rib== False:
             target_time= satTime.strftime('%Y%m%d.%H%M')
             a_rib_url= bgpToolKit.MRTfileHandler.get_download_url(type, monitor, target_time)
             a_rib_filename= a_rib_url.split('/')[-1]
-            # 判断url是否有效
+            
             response = requests.head(a_rib_url).status_code
             if response==200:
                 target_path= f'{self.collection_data_lib}{monitor}/'
                 cmd= f"cd {target_path}; wget {a_rib_url}; mv {a_rib_filename} {monitor}_{a_rib_filename}"
                 p= subprocess.Popen(cmd, shell=True)
                 logger.info(f'    - {p.pid=}, downloading a `{monitor}` rib table...')
                 processList.append(p)
@@ -146,30 +144,28 @@
             destination= self.collection_data_lib,
             save_by_collector=1
         )
         bgpdbp.start_on()
         # check_error_list(sys.path[0]+ "/errorInfo.txt")
         whole_files= glob.glob(self.collection_data_lib+ monitor+ os.sep+ monitor+ '_'+ type+ '*')
         
-        # 当采集器未曾收录相应时间段，就会下载不到对应文件，用try来避错
         try:
             dest_files= utils.cut_files_list(whole_files, satTime, endTime)
         except:
             return []
         return dest_files
 
-    # 用于raw2txt中的多进程
     def trans_multiproc(self, tup):
             os.system('bgpdump -m '+ tup[1] + ' > '+ tup[0] +  os.path.basename(tup[1])+ '.txt')
 
     def raw2txt(self, dest_dir, raw_files, type, monitor= None):       
         '''- description: transform BGP update raw data to .txt by command `bgpdump`
         - return `.txt list`
         '''
-        if len(raw_files)==1:   # 用于每个采集点只解析一张rib时
+        if len(raw_files)==1:
             target_path= f"{dest_dir}{os.path.basename(raw_files[0])}.txt"
             cmd= f"bgpdump -m {raw_files[0]} > {target_path}"
             p= subprocess.Popen(cmd, shell=True)
             logger.info(f"    - {p.pid=}, parsing a rib of `{monitor if monitor!=None else ' '}`...")
             processList.append(p)
             return [target_path]
 
@@ -181,32 +177,26 @@
         pool.join()
 
         parsed_files= sorted(glob.glob(f'{dest_dir}/*{type}*'))
         return parsed_files
 
     def oneMonitor(self, type, txt_dir, monitor, fact_satTime: datetime, endTime: datetime):
         '''
-        - description: `getUpdTxts`的子函数, 用于单个monitor的多文件的下载(可能无)和解析(一定有)操作
-        - args-> self {*}: 
+        - description: 单个monitor的多文件的下载和解析
         - args-> type {*}: `'updates'`or`'rib.'`or`'bview.'`
-        - args-> txt_dir {*}: 当前event当前monitor下的解析文件路径
-        - args-> monitor {*}: 
-        - args-> fact_satTime {*}: 
-        - args-> endTime {*}: 
-        - return {*}: txtfiles 文件名列表; 也可能空列表，是采集器未收录的问题
         '''
         curDir= utils.makePath( txt_dir+ monitor+ '/' )        
-        os.system(f'rm {curDir}*_{type}*')               # 把对应事件下的曾经解析过的文件都删掉，以便重新下载再解析。
+        os.system(f'rm {curDir}*_{type}*')
         raw_files= self.isDwlad(type, monitor, fact_satTime, endTime)
-        if not len(raw_files):    # 未下载
+        if not len(raw_files): 
             st1= time.time()
             raw_files= self.download(type, monitor, fact_satTime, endTime, only_rib= not self.updTag )
             logger.info(' '*4+ '- %s dwladed: %.3f sec, %d files.' %( monitor, time.time()- st1, len(raw_files)))
 
-        if not len(raw_files):    # 下载后仍为空
+        if not len(raw_files):
             logger.warning(' '*4+ '- %s has missed files on website.' % monitor)
             return []
 
         st2= time.time()
         txtfiles= self.raw2txt( curDir, raw_files, type, monitor )
         #logger.info(' '*4+ '- %s parsed: %.3f sec, %d files.' %( monitor, time.time()- st2, len(raw_files)))
 
@@ -215,122 +205,110 @@
     def getUpdTxts(self, events_dict):
         '''解析updates文件
         - return:  `{'evtNm': {'monitor': ( [ .txt, ...]|None, str|None ) } } `'''
         res= deepcopy( events_dict )
         ppath, dirs, _= os.walk( self.collection_data_lib_parsed ).__next__()
         for evtNm, moniDict in events_dict.items():
             logger.info(' '*2+ '- %s:' % evtNm )
-            if evtNm in dirs:   # 当事件名目录已存在, 即可能解析过该事件了
+            if evtNm in dirs:
                 p2, moni_dirs, _ = os.walk( ppath+ evtNm+ os.sep ).__next__()
                 for monitor,[ satTime_tradiFeat, endTime, satTime_graphFeat ] in moniDict.items():
-                    # 以上3个时间都是标准化了的。updates消息的起始解析时刻有两种：
-                    #   - 只有传统特征时，就是`原starttime`
-                    #   - 要解析图特征时，把`原starttime`替换为`satTime_atRIB`
-                    # 需求的文件名列表是否都在 实际的文件名列表中 allin
+                    
                     txtfiles= sorted(glob.glob(p2+ monitor+ os.sep+ monitor+ '_updates*'))
                     if not satTime_graphFeat :
                         fact_satTime= satTime_tradiFeat
                         watershed_= None
                     else:
                         fact_satTime= satTime_graphFeat
                         watershed_= satTime_tradiFeat.strftime('%Y%m%d.%H%M')
 
                     interval= utils.intervalMin('updates', monitor[:3])
                     allin= utils.allIn(interval, txtfiles, fact_satTime, endTime)
 
                     if monitor in moni_dirs and allin :
                         target_files= utils.cut_files_list(txtfiles, fact_satTime, endTime)
-                        # 变量 watershed_ 用在有图特征的情况下，切分updates的文件列表target_files。使其前部分用于更新拓扑；后部分用于计算传统特征。
                         res[evtNm][monitor]= ( target_files, watershed_ )
                         logger.info(' '*4+ '- %s: upds has existed, don\'t need to parse.' % monitor)
-                    else:   # 未解析过该采集器
+                    else:
                         res[evtNm][monitor]= ( self.oneMonitor('updates', p2, monitor, fact_satTime, endTime), watershed_ )
                         
-            else:   # 未解析过该事件
+            else:
                 for monitor,[ satTime_tradiFeat, endTime, satTime_graphFeat ] in moniDict.items():
                     if not satTime_graphFeat :
                         fact_satTime= satTime_tradiFeat
                         watershed_= None
                     else:
                         fact_satTime= satTime_graphFeat
                         watershed_= satTime_tradiFeat.strftime('%Y%m%d.%H%M')
 
                     res[evtNm][monitor]= ( self.oneMonitor('updates', ppath+ evtNm+ '/', monitor, fact_satTime, endTime), watershed_ )
         return res
 
     def getRibTxts(self, events_dict):
         '''
-        - description: 解析rib文件。
-            - 当self.updTag= True, 每个 event/monitor 下仅需一个rib（startTime的左邻近）; 
-            - 当False, 则需全量下载解析指定时间段内的rib表
-        - args-> events_dict {*}: 
+        - description: 解析rib文件
         - return {*}: `{'evtNm': {'monitor': [.txt]|[] } } `
         '''
-        # 用于单个采集点采集一个rib的情况
         list_parsing=[]
         list_downloading=[]
 
         strmap= {'rrc': 'bview.', 'rou': 'rib.'}
         res= deepcopy( events_dict )
         ppath, dirs, _= os.walk( self.collection_data_lib_parsed ).__next__()
         for evtNm, moniDict in events_dict.items():
             logger.info(' '*2+ '- %s:' % evtNm )
 
             for monitor,[ _, endRIBtime, satRIBtime ] in moniDict.items():
                 txtFolder= ppath+ evtNm+ '/' + monitor+ '/'     
                 utils.makePath(txtFolder)
-
-                # 先看看txtFolder目录下是否已经解析好了相应数据。
+                
                 txtfiles= sorted(glob.glob( txtFolder+ monitor+ '_'+ strmap[monitor[:3]]+ '*' ))
                 interval= utils.intervalMin('ribs', monitor[:3])
-                if self.updTag:     # 仅需一张rib的情况
-                    if len(txtfiles) != 1:  # 当没有解析数据
-                        # 拿到basename
+                if self.updTag:
+                    if len(txtfiles) != 1:
                         target_time= satRIBtime.strftime('%Y%m%d.%H%M')
                         a_rib_url= bgpToolKit.MRTfileHandler.get_download_url(type, monitor, target_time)
                         basename = a_rib_url.split('/')[-1]
                         download_file= f"{self.collection_data_lib}{monitor}/{monitor}_{basename}"
                         pathTXT= f"{self.collection_data_lib_parsed}{evtNm}/{monitor}/{monitor}_{basename}.txt"
-                        # 当没下载
+                        
                         if not os.path.exists(download_file):
-                            # 当没下载，先判断url是否有效
                             response = requests.head(a_rib_url).status_code
                             if response==404:
                                 logger.warning(f'    - in {monitor}, url WRONG:`{a_rib_url}`')
                                 res[evtNm][monitor]= []
                             else:
                                 list_downloading.append({'url': a_rib_url, 'path': download_file})
                                 list_parsing.append({'pathMRT': download_file, 'pathTXT': pathTXT})
                                 res[evtNm][monitor]= [pathTXT]
-                        # 当已经下载
                         else:
                             list_parsing.append({'pathMRT': download_file, 'pathTXT': pathTXT})
                             res[evtNm][monitor]= [pathTXT]
                     else:   
                         logger.info(' '*4+ '- %s: ribs has existed, don\'t need to parse.' % monitor)    
                         res[evtNm][monitor]= txtfiles 
 
-                else:               # 需多张rib的情况
+                else:
                     allin= utils.allIn(interval, txtfiles, satRIBtime, endRIBtime)
                     if allin:
                         logger.info(' '*4+ '- %s: ribs has existed, don\'t need to parse.' % monitor) 
                     else:
                         txtfiles= self.oneMonitor(strmap[monitor[:3]], ppath+ evtNm+ '/', monitor, satRIBtime, endRIBtime)
-                    res[evtNm][monitor]= txtfiles  
-        # 并行下载
+                    res[evtNm][monitor]= txtfiles 
+                    
         if list_downloading:
             plist=[]
             for dic in list_downloading:
                 cmd= f"wget -q -O {dic['path']} {dic['url']}"
                 p= subprocess.Popen(cmd, shell=True)
                 logger.info(f'    - {p.pid=}, downloading: `{cmd}`...')
                 plist.append(p)
             for p in plist:
                 p.wait()
-        # 并行解析
+                
         if list_parsing:
             p2list=[]
             for dic in list_parsing:
                 cmd= f"bgpdump -m {dic['pathMRT']} > {dic['pathTXT']}"
                 p= subprocess.Popen(cmd, shell=True)
                 logger.info(f'    - {p.pid=}, parsing: `{cmd}`...')
                 p2list.append(p)
@@ -340,42 +318,39 @@
         return res
 
     def getRawTxts(self, events_dict: dict):
         '''- including download and parse
         - return `{ 'updates': {'evtNm': {'monitor': ([ '.txt', ...], str|None) } } |{}, 
                     'ribs'    : {'evtNm': {'monitor': [ '.txt', ...]|[]         } } |{}
                   }`
-        - 其中`ribs`的值在不求图特征时为 `{}`'''
-        if not os.path.exists( self.collection_data_lib_parsed ):   # 多余
+        '''
+        if not os.path.exists( self.collection_data_lib_parsed ):
             utils.makePath( self.collection_data_lib_parsed )
         resUpd, resRib= {},{}
-        # 收集updates文件
+        
         if self.updTag:
             logger.info('Start: parse `updates` data:')
             resUpd= self.getUpdTxts(events_dict)
             logger.info('End: `updates` data.')
         else:
             logger.info('ONLY analysis ribs with graph-features, no need to get any updates files.')
-        # 收集rib文件
         if self.ribTag:
             t1= time.time()
             logger.info('Start: parse `ribs` data:')
             resRib= self.getRibTxts(events_dict)
             logger.info(f'End({(time.time()-t1):.1f}sec): `ribs` data.')
         return {'updates': resUpd, 'ribs': resRib} 
     
 
     def run(self):
         '''
-        - description: 根据事件信息进行下载、解析模块的主api
+        - description: main func
         - return {*}: 
             `{ 'updates': {'evtNm': {'monitor': ( [ .txt, ...]|None, str|None ) } },
                 'ribs'  : {'evtNm': {'monitor': [.txt]|None                       } } | {}   } `
-            - 其中updates中的str: 为日期分水岭，当ribs的值为空，则此处为None;
-            - 当 self.updTag= False, 则 updates部分的值为空
         '''
         evtDic= self.getEventsDict()
         txtDic= self.getRawTxts(evtDic)
 
         # ending all of subprocess
         for p in processList:
             p.wait()
```

### Comparing `fastFET-0.0.5/fastFET/logConfig.json` & `fastFET-0.0.6/fastFET/logConfig.json`

 * *Files identical despite different names*

### Comparing `fastFET-0.0.5/fastFET.egg-info/PKG-INFO` & `fastFET-0.0.6/fastFET.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,264 +1,259 @@
-Metadata-Version: 2.1
-Name: fastFET
-Version: 0.0.5
-Summary: A fast feature extrating tool for BGP Dataset Collection.
-Home-page: https://github.com/JamesRay0713/fastFET
-Author: James Ray
-Author-email: hl1670704310@icloud.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-
-##
-logger.info( utils.logMemUsage(10, inspect.stack()[0][3] ))     # 调试锚点：随删
-##
-
-持续优化的问题：
-- 计算ED那里，对比测试多进程的情况。
-- 自定义多进程模块中，等待睡眠为1s是否合理。
-- 做一个对比各个特征计算时间的函数。
-- 构建函数：输入一个或多个新特征，能把采集结果追加到已有的DF.csv。这要涉及到`自定义特征采集函数`的API
-- 关于每slot如何构建全局拓扑图：还是要结合pl.DF来加速计算，避免逐条消息更新。
-- requirement的预安装，特别是bgpdump
-- 针对异常类型的特征设计：子前缀劫持、路径劫持、路由泄露等，连接其他框架？
-
-require add:
-    - pyarrow
-
-# BGP特征提取工具 
-
-## 组织结构
-
-### 1. 库路径
-
-```
-fastFET  
-    ├── BGPMAGNET/      BGP原始数据下载工具(by倪泽栋)  
-    ├── collectData.py  主模块：数据收集，包括下载、解析   
-    ├── event_list.csv　要采集的事件列表  
-    ├── featGraph.py    图特征采集功能集合   
-    ├── featTradition.py传统特征采集功能集合  
-    ├── featTree.py     特征树，集成所有特征及其pl.Expr  
-    ├── FET.py          主模块：特征采集  
-    ├── logConfig.json  日志配置  
-    ├── utils.py        工具集合   
-    ├── MultiProcess.py 多进程工具   
-    ├── README.md  
-    └── requirements.txt
-``` 
-
-### 2. cwd 默认路径
-```
-cwd  
-├── Dataset  
-│   ├── features/               特征提取最终数据  
-│   │　　└── date_event_monitor.csv  
-│   ├── MOAS/                   提取过程中属于multi-origin-AS的消息  
-│   ├── raw_cmpres              原始数据下载存放路径    
-│   │   ├── rrc00/    
-│   │   └── routeviews./    
-│   └── raw_parsed              原始数据解析存放路径    
-│       └── 事件名  
-│           └── 采集器名/  
-└── log                         日志路径    
-    ├── errors.log  
-    └── info.log 
-```
-
-## 使用方法
-
-创建特征提取工具对象`fet`, 指定特征集合, 添加目标事件信息, 开始提取特征。
-```python
-from fastFET import FET
-ev= FET.EventEditor()
-ev.addEvents([])
-fet= FET.FET()
-fet.setCustomFeats([])
-feat_path= fet.run()
-```
-- 先利用 EventEditor 的 addEvents 方法添加此次要采集特征的事件信息。
-    - 格式：事件名；起始时间；结束时间（可缺省）；采集器（可多个，用`,`相隔）
-    - 举例：`GoogleLeak,2017/08/25 05:00:00,2017/08/25 06:00:00,rrc06,rrc05`
-- 后利用 `fet` 对象实现特征采集操作。
-    1. 初始化对象: `fet= FET.FET()`, 参数见注释, 其中 `slot` 为特征采集的时间尺度, 默认1分钟。
-        
-    2. 自定义此次采集所需的特征集合: `fet.setCustomFeats([...])`
-        - 有3种自定义特征的方法：全量采集；按类别采集；按单个特征采集 (详见该方法的注释)
-        - 若想查看该工具现已集成的特征列表：`feats= fet.getAllFeats()`
-
-    3. 正式采集特征: `fet.run()`
-        - 参数: 当`fet`对象仅仅只从大量 rib 表采集图特征时`only_rib`才为`True`, 此时自定义的特征集合仅限于图特征
-        - 返回: 特征存放路径
-
-## 框架解释
-- RIPE NCC和RouteViews的`.gz`和`.bz2`原始数据经并行下载和 `bgpdump`工具转码得到的`.txt`文件，根据事件和采集器名分别存入 `./Dataset/raw_parsed/event_name/monitor_name/`
-- 利用 `polars` 数据分析工具高效提取BGP特征，按事件名存入 `./Dataset/features/date__event__collector.csv`。
-- 顺便收集了事件中出现的MOAS消息，存入`./Dataset/MOAS/`
-
-
-## 输出字段说明
-- 共139字段，含序列号，日期，136个特征，及标签。
-
-类别 | 字段 | 解释
-|---|---|--- 
-\- | time_bin | 时间序列号
-\- | date | 日期
-volume | v_total | 消息总数
-\- | v_A | 宣告消息总数
-\- | v_W | 撤销消息总数
-\- | v_IGP | 属于IGP的消息总数
-\- | v_EGP | 属于EGP的消息总数
-\- | v_ICMP | 属于IMCOMPLETE的消息总数
-\- | v_peer | 不同peer的数量
-\- | v_pfx_t_cnt | 不同prefix的数量
-\- | v_pfx_t_avg | 不同prefix出现过的平均次数
-\- | v_pfx_t_max | 不同prefix出现过的最大次数
-\- | v_pfx_A_cnt | 属宣告的不同prefix的数量
-\- | v_pfx_A_avg | 属宣告的不同prefix出现过的平均次数
-\- | v_pfx_A_max | 属宣告的不同prefix出现过的最大次数
-\- | v_pfx_W_cnt | 属撤销的不同prefix的数量
-\- | v_pfx_W_avg | 属撤销的不同prefix出现过的平均次数
-\- | v_pfx_W_max | 属撤销的不同prefix出现过的最大次数
-\- | v_pp_t_cnt | 不同peer-prefix对的数量
-\- | v_pp_t_avg | 不同peer-prefix对出现过的平均次数
-\- | v_pp_t_max | 不同peer-prefix对出现过的最大次数
-\- | v_pp_A_cnt | 属宣告的不同peer-prefix对的数量
-\- | v_pp_A_avg | 属宣告的不同peer-prefix对出现过的平均次数
-\- | v_pp_A_max | 属宣告的不同peer-prefix对出现过的最大次数
-\- | v_pp_W_cnt | 属撤销的不同peer-prefix对的数量
-\- | v_pp_W_avg | 属撤销的不同peer-prefix对出现过的平均次数
-\- | v_pp_W_max | 属撤销的不同peer-prefix对出现过的最大次数
-\- | v_oriAS_t_cnt | 源AS的数量
-\- | v_oriAS_t_avg | 源AS的平均出现次数
-\- | v_oriAS_t_max | 源AS的最大出现次数
-\- | v_oriAS_peer_cnt | 不同peer-originAS对的数量
-\- | v_oriAS_peer_avg | 不同peer-originAS对出现过的平均次数
-\- | v_oriAS_peer_max | 不同peer-originAS对出现过的最大次数
-\- | v_oriAS_pfx_cnt | 不同prefix-originAS对的数量
-\- | v_oriAS_pfx_avg | 不同prefix-originAS对出现过的平均次数
-\- | v_oriAS_pfx_max | 不同prefix-originAS对出现过的最大次数
-\- | v_oriAS_pp_cnt | 不同peer-prefix-originAS对的数量
-\- | v_oriAS_pp_avg | 不同peer-prefix-originAS对出现过的平均次数
-\- | v_oriAS_pp_max | 不同peer-prefix-originAS对出现过的最大次数
-path | path_len_max | 最大路径长度
-\- | path_len_avg | 平均路径长度
-\- | path_unq_len_max | 去重后的最大路径长度
-\- | path_unq_len_avg | 去重后的平均路径长度
-AS | As_total_cnt | 出现过的AS的数量
-\- | As_total_avg | 不同AS出现过的平均次数
-\- | As_total_max | 不同AS出现过的最大次数
-\- | AS_rare_avg | 所有消息的路径中含有稀有AS的总共数量
-\- | AS_rare_sum | 一条消息的路径中含有稀有AS的最大数量
-dynamic | is_WA | 属于撤销后宣告的消息数
-\- | is_AW | 属于宣告后撤销的消息数
-\- | is_WAW | 属于撤销-宣告-撤销的消息数
-\- | is_longer_path | 路径变长的消息数
-\- | is_shorter_path | 路径变短的消息数
-\- | is_longer_unq_path | 去重后路径变长的消息数
-\- | is_shorter_unq_path | 去重后路径变短的消息数
-\- | is_new | 属于全新宣告的消息数
-\- | is_dup_ann | 属于重复宣告的消息数（仅prefix重复）
-\- | is_AWnA | 属于宣告-撤销多次-宣告的消息数
-\- | is_imp_wd | 属于隐式撤销的消息数（重复宣告，但其他属性变化）
-\- | is_WnA | 属于撤销多次-宣告的消息数
-\- | is_AWn | 属于宣告-多次撤销的消息数
-\- | is_AnW | 属于多次宣告-撤销的消息数
-\- | is_WAn | 属于撤销-多次宣告的消息数
-\- | is_dup_wd | 属于重复撤销的消息数
-\- | is_dup | 属于重复宣告的消息数（完全重复）
-\- | is_flap | 属于宣告-撤销-宣告，且属性完全不变的消息数
-\- | is_NADA | 属于宣告-撤销-宣告，但属性有变化的消息数
-\- | is_imp_wd_spath | 属于路径属性不变的隐式撤销的消息数
-\- | is_imp_wd_dpath | 属于路径属性变化的隐式撤销的消息数
-\- | type_0 | 针对同一prefix，源AS改变了的消息数(MOAS)
-\- | type_1 | 针对同一prefix，path中第2个AS改变了的消息数
-\- | type_2 | 针对同一prefix，path中第3个AS改变了的消息数
-\- | type_3 | 针对同一prefix，path中第4个AS改变了的消息数
-\- | ED_max | 同一peer-prefix下，最大的编辑距离值的消息数
-\- | ED_avg | 同一peer-prefix下，平均的编辑距离值的消息数
-\- | ED_0 | 同一peer-prefix下，编辑距离为0的消息数
-\- | ED_1 ~ ED_10 | 同一peer-prefix下，编辑距离为1~10的消息数
-ratio | ratio_firstOrder | 最活跃的宣告前缀/宣告总数（即 `v_pfx_A_max / v_A`）
-\- | ratio_ann | 宣告量占更新消息总量之比（即`v_A / v_total`）
-\- | ratio_wd | 撤销量占更新消息总量之比（即`v_W / v_total`）
-\- | ratio_origin0 | IGP占宣告量之比（即`v_IGP / v_A`）
-\- | ratio_origin1 | EGP占宣告量之比（即`v_EGP / v_A`）
-\- | ratio_origin2 | IMCOMPLETE占宣告量之比（即`v_ICMP / v_A`）
-\- | ratio_dup_ann | 完全重复宣告占宣告量之比（即`is_dup_ann / v_A`）
-\- | ratio_flap | 属性完全不变的宣-撤-宣占宣告量之比（即`is_flap / v_A`）
-\- | ratio_NADA | 属性有变化的宣-撤-宣占宣告量之比（即`is_NADA / v_A`）
-\- | ratio_imp_wd | 隐式撤销占宣告量之比（即`is_imp_wd / v_A`）
-\- | ratio_imp_wd2 | 隐式撤销占隐式撤销+撤销之比（即`is_imp_wd / (is_imp_wd+ v_W)`）
-\- | ratio_exp_wd | 真正撤销占隐式撤销+撤销之比（即`v_W / (is_imp_wd+ v_W)`）
-\- | ratio_imp_wd_dpath | 路径属性不同的隐式撤销占隐式撤销之比（即`is_imp_wd_dpath / is_imp_wd`）
-\- | ratio_imp_wd_spath | 路径属性相同的隐式撤销占隐式撤销之比（即`is_imp_wd_spath / is_imp_wd`）
-\- | ratio_new | 全新宣告占宣告量之比（即`is_new / v_A`）
-\- | ratio_wd_dups | 重复撤销占撤销量之比（即`is_dup_wd / v_W`）
-\- | ratio_longer_path | 更长路径宣告占宣告量之比（即`is_longer_path / v_A`）
-\- | ratio_shorter_path | 更短路径宣告占宣告量之比（即`is_shorter_path / v_A`）
-\- | ratio_longer_path2 | 更长路径宣告占更长/短宣告量之比（即`is_longer_path / (is_longer_path+ is_shorter_path)`）
-\- | ratio_shorter_path2 | 更短路径宣告占更长/短宣告量之比（即`is_shorter_path / (is_longer_path+ is_shorter_path)`）
-node_level_graph | nd_degree_centrality | 节点平均度中心性
-\- | nd_node_clique_number | 节点平均最大集团数
-\- | nd_number_of_cliques | 节点平均集团数
-\- | nd_closeness_centrality | 节点平均紧密中心性
-\- | nd_betweenness_centrality | 节点平均中介中心性
-\- | nd_local_efficiency | 节点平均局部效率
-\- | nd_harmonic_centrality | 节点平均谐波中心度
-\- | nd_eigenvector_centrality | 节点平均特征向量中心度
-\- | nd_pagerank | 节点平均重要度排名
-\- | nd_clustering | 节点平均聚类中心性
-\- | nd_triangles | 节点平均三角形数量
-\- | nd_eccentricity | 节点平均偏心率
-\- | nd_average_shortest_pth_length | 节点平均最短路径长度
-\- | nd_load_centrality | 节点平均负载中心性
-\- | nd_degree | 节点平均度数
-\- | nd_square_clustering | 节点平均平方聚类系数
-\- | nd_average_neighbor_degree | 节点平均邻居度数
-AS_level_graph | gp_nb_of_nodes | 总节点数
-\- | gp_nb_of_edges | 总边数
-\- | gp_diameter | 最大偏心率
-\- | gp_assortativity | 同配性
-\- | gp_largest_eigenvalue | 最大特征值
-\- | gp_algebraic_connectivity | 代数连通度
-\- | gp_effective_graph_resistance | 有效图阻抗
-\- | gp_symmetry_ratio | 对称率
-\- | gp_natural_connectivity | 自然连通度
-\- | gp_node_connectivity | 节点连通度
-\- | gp_edge_connectivity | 边连通度
-\- | gp_weighted_spectrum_3 | 三方加权频谱
-\- | gp_weighted_spectrum_4 | 四方加权频谱
-\- | gp_percolation_limit | 渗透极限
-\- | gp_nb_spanning_trees | 生成树数量
-\- | label	|	异常类型标签
-
-
-
-
-## 特征补充
-
-字段            |  说明
- ----           |  ----
-ConcentratRatio |  前三个最活跃的宣告前缀/宣告总数（即 `vol_ann_pfx_max / v_A`）
-
-
-## 其他注意事项 
-
-1. BGP RAW DATA: 采集时间间隔不统一，如rrc00中20030723.0745之前为15min（且时刻不固定），之后为5min（时刻固定）。
-2. MRT文件解析后，path 字段可能存在`{}`形式，如下: 
-    - 58057 6939 4635 4788 38044 23736
-    - 58057 6939 4635 4788 38044 {23736}
-    - 58057 6939 1299 2603 2603 2603 6509 {271,7860,8111,53904}
-3. `stat.ripe.net`的API获取的路由，path字段可能存在`[]`形式。
-3. `Route-Views`中的MRT文件名格式不严谨，经常出现无规律的时间戳。
-
-
-# 发现：
-- 劫持震荡：
-当`is_MOAS`很大，而`vol_oriAS_peer_pfx`或`vol_oriAS_pfx`很小时，说明存在一个prefix反复被多个AS宣告的情况。
-- outage类型难溯源
-
+Metadata-Version: 2.1
+Name: fastFET
+Version: 0.0.6
+Summary: A fast feature extrating tool for BGP Dataset Collection.
+Home-page: https://github.com/JamesRay0713/fastFET
+Author: James Ray
+Author-email: hl1670704310@icloud.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+
+
+持续优化的问题：
+- 计算ED那里，对比测试多进程的情况。
+- 自定义多进程模块中，等待睡眠为1s是否合理。
+- 做一个对比各个特征计算时间的函数。
+- 构建函数：输入一个或多个新特征，能把采集结果追加到已有的DF.csv。这要涉及到`自定义特征采集函数`的API
+- 关于每slot如何构建全局拓扑图：还是要结合pl.DF来加速计算，避免逐条消息更新。
+- requirement的预安装，特别是bgpdump
+- 针对异常类型的特征设计：子前缀劫持、路径劫持、路由泄露等，连接其他框架？
+
+require add:
+    - pyarrow
+
+# BGP特征提取工具 
+
+## 组织结构
+
+### 1. 库路径
+
+```
+fastFET  
+    ├── BGPMAGNET/      BGP原始数据下载工具(by倪泽栋)  
+    ├── collectData.py  主模块：数据收集，包括下载、解析   
+    ├── event_list.csv　要采集的事件列表  
+    ├── featGraph.py    图特征采集功能集合   
+    ├── featTradition.py传统特征采集功能集合  
+    ├── featTree.py     特征树，集成所有特征及其pl.Expr  
+    ├── FET.py          主模块：特征采集  
+    ├── logConfig.json  日志配置  
+    ├── utils.py        工具集合   
+    ├── MultiProcess.py 多进程工具   
+    ├── README.md  
+    └── requirements.txt
+``` 
+
+### 2. cwd 默认路径
+```
+cwd  
+├── Dataset  
+│   ├── features/               特征提取最终数据  
+│   │　　└── date_event_monitor.csv  
+│   ├── MOAS/                   提取过程中属于multi-origin-AS的消息  
+│   ├── raw_cmpres              原始数据下载存放路径    
+│   │   ├── rrc00/    
+│   │   └── routeviews./    
+│   └── raw_parsed              原始数据解析存放路径    
+│       └── 事件名  
+│           └── 采集器名/  
+└── log                         日志路径    
+    ├── errors.log  
+    └── info.log 
+```
+
+## 使用方法
+
+创建特征提取工具对象`fet`, 指定特征集合, 添加目标事件信息, 开始提取特征。
+```python
+from fastFET import FET
+ev= FET.EventEditor()
+ev.addEvents([])
+fet= FET.FET()
+fet.setCustomFeats([])
+feat_path= fet.run()
+```
+- 先利用 EventEditor 的 addEvents 方法添加此次要采集特征的事件信息。
+    - 格式：事件名；起始时间；结束时间（可缺省）；采集器（可多个，用`,`相隔）
+    - 举例：`GoogleLeak,2017/08/25 05:00:00,2017/08/25 06:00:00,rrc06,rrc05`
+- 后利用 `fet` 对象实现特征采集操作。
+    1. 初始化对象: `fet= FET.FET()`, 参数见注释, 其中 `slot` 为特征采集的时间尺度, 默认1分钟。
+        
+    2. 自定义此次采集所需的特征集合: `fet.setCustomFeats([...])`
+        - 有3种自定义特征的方法：全量采集；按类别采集；按单个特征采集 (详见该方法的注释)
+        - 若想查看该工具现已集成的特征列表：`feats= fet.getAllFeats()`
+
+    3. 正式采集特征: `fet.run()`
+        - 参数: 当`fet`对象仅仅只从大量 rib 表采集图特征时`only_rib`才为`True`, 此时自定义的特征集合仅限于图特征
+        - 返回: 特征存放路径
+
+## 框架解释
+- RIPE NCC和RouteViews的`.gz`和`.bz2`原始数据经并行下载和 `bgpdump`工具转码得到的`.txt`文件，根据事件和采集器名分别存入 `./Dataset/raw_parsed/event_name/monitor_name/`
+- 利用 `polars` 数据分析工具高效提取BGP特征，按事件名存入 `./Dataset/features/date__event__collector.csv`。
+- 顺便收集了事件中出现的MOAS消息，存入`./Dataset/MOAS/`
+
+
+## 输出字段说明
+- 共139字段，含序列号，日期，136个特征，及标签。
+
+类别 | 字段 | 解释
+|---|---|--- 
+\- | time_bin | 时间序列号
+\- | date | 日期
+volume | v_total | 消息总数
+\- | v_A | 宣告消息总数
+\- | v_W | 撤销消息总数
+\- | v_IGP | 属于IGP的消息总数
+\- | v_EGP | 属于EGP的消息总数
+\- | v_ICMP | 属于IMCOMPLETE的消息总数
+\- | v_peer | 不同peer的数量
+\- | v_pfx_t_cnt | 不同prefix的数量
+\- | v_pfx_t_avg | 不同prefix出现过的平均次数
+\- | v_pfx_t_max | 不同prefix出现过的最大次数
+\- | v_pfx_A_cnt | 属宣告的不同prefix的数量
+\- | v_pfx_A_avg | 属宣告的不同prefix出现过的平均次数
+\- | v_pfx_A_max | 属宣告的不同prefix出现过的最大次数
+\- | v_pfx_W_cnt | 属撤销的不同prefix的数量
+\- | v_pfx_W_avg | 属撤销的不同prefix出现过的平均次数
+\- | v_pfx_W_max | 属撤销的不同prefix出现过的最大次数
+\- | v_pp_t_cnt | 不同peer-prefix对的数量
+\- | v_pp_t_avg | 不同peer-prefix对出现过的平均次数
+\- | v_pp_t_max | 不同peer-prefix对出现过的最大次数
+\- | v_pp_A_cnt | 属宣告的不同peer-prefix对的数量
+\- | v_pp_A_avg | 属宣告的不同peer-prefix对出现过的平均次数
+\- | v_pp_A_max | 属宣告的不同peer-prefix对出现过的最大次数
+\- | v_pp_W_cnt | 属撤销的不同peer-prefix对的数量
+\- | v_pp_W_avg | 属撤销的不同peer-prefix对出现过的平均次数
+\- | v_pp_W_max | 属撤销的不同peer-prefix对出现过的最大次数
+\- | v_oriAS_t_cnt | 源AS的数量
+\- | v_oriAS_t_avg | 源AS的平均出现次数
+\- | v_oriAS_t_max | 源AS的最大出现次数
+\- | v_oriAS_peer_cnt | 不同peer-originAS对的数量
+\- | v_oriAS_peer_avg | 不同peer-originAS对出现过的平均次数
+\- | v_oriAS_peer_max | 不同peer-originAS对出现过的最大次数
+\- | v_oriAS_pfx_cnt | 不同prefix-originAS对的数量
+\- | v_oriAS_pfx_avg | 不同prefix-originAS对出现过的平均次数
+\- | v_oriAS_pfx_max | 不同prefix-originAS对出现过的最大次数
+\- | v_oriAS_pp_cnt | 不同peer-prefix-originAS对的数量
+\- | v_oriAS_pp_avg | 不同peer-prefix-originAS对出现过的平均次数
+\- | v_oriAS_pp_max | 不同peer-prefix-originAS对出现过的最大次数
+path | path_len_max | 最大路径长度
+\- | path_len_avg | 平均路径长度
+\- | path_unq_len_max | 去重后的最大路径长度
+\- | path_unq_len_avg | 去重后的平均路径长度
+AS | As_total_cnt | 出现过的AS的数量
+\- | As_total_avg | 不同AS出现过的平均次数
+\- | As_total_max | 不同AS出现过的最大次数
+\- | AS_rare_avg | 所有消息的路径中含有稀有AS的总共数量
+\- | AS_rare_sum | 一条消息的路径中含有稀有AS的最大数量
+dynamic | is_WA | 属于撤销后宣告的消息数
+\- | is_AW | 属于宣告后撤销的消息数
+\- | is_WAW | 属于撤销-宣告-撤销的消息数
+\- | is_longer_path | 路径变长的消息数
+\- | is_shorter_path | 路径变短的消息数
+\- | is_longer_unq_path | 去重后路径变长的消息数
+\- | is_shorter_unq_path | 去重后路径变短的消息数
+\- | is_new | 属于全新宣告的消息数
+\- | is_dup_ann | 属于重复宣告的消息数（仅prefix重复）
+\- | is_AWnA | 属于宣告-撤销多次-宣告的消息数
+\- | is_imp_wd | 属于隐式撤销的消息数（重复宣告，但其他属性变化）
+\- | is_WnA | 属于撤销多次-宣告的消息数
+\- | is_AWn | 属于宣告-多次撤销的消息数
+\- | is_AnW | 属于多次宣告-撤销的消息数
+\- | is_WAn | 属于撤销-多次宣告的消息数
+\- | is_dup_wd | 属于重复撤销的消息数
+\- | is_dup | 属于重复宣告的消息数（完全重复）
+\- | is_flap | 属于宣告-撤销-宣告，且属性完全不变的消息数
+\- | is_NADA | 属于宣告-撤销-宣告，但属性有变化的消息数
+\- | is_imp_wd_spath | 属于路径属性不变的隐式撤销的消息数
+\- | is_imp_wd_dpath | 属于路径属性变化的隐式撤销的消息数
+\- | type_0 | 针对同一prefix，源AS改变了的消息数(MOAS)
+\- | type_1 | 针对同一prefix，path中第2个AS改变了的消息数
+\- | type_2 | 针对同一prefix，path中第3个AS改变了的消息数
+\- | type_3 | 针对同一prefix，path中第4个AS改变了的消息数
+\- | ED_max | 同一peer-prefix下，最大的编辑距离值的消息数
+\- | ED_avg | 同一peer-prefix下，平均的编辑距离值的消息数
+\- | ED_0 | 同一peer-prefix下，编辑距离为0的消息数
+\- | ED_1 ~ ED_10 | 同一peer-prefix下，编辑距离为1~10的消息数
+ratio | ratio_firstOrder | 最活跃的宣告前缀/宣告总数（即 `v_pfx_A_max / v_A`）
+\- | ratio_ann | 宣告量占更新消息总量之比（即`v_A / v_total`）
+\- | ratio_wd | 撤销量占更新消息总量之比（即`v_W / v_total`）
+\- | ratio_origin0 | IGP占宣告量之比（即`v_IGP / v_A`）
+\- | ratio_origin1 | EGP占宣告量之比（即`v_EGP / v_A`）
+\- | ratio_origin2 | IMCOMPLETE占宣告量之比（即`v_ICMP / v_A`）
+\- | ratio_dup_ann | 完全重复宣告占宣告量之比（即`is_dup_ann / v_A`）
+\- | ratio_flap | 属性完全不变的宣-撤-宣占宣告量之比（即`is_flap / v_A`）
+\- | ratio_NADA | 属性有变化的宣-撤-宣占宣告量之比（即`is_NADA / v_A`）
+\- | ratio_imp_wd | 隐式撤销占宣告量之比（即`is_imp_wd / v_A`）
+\- | ratio_imp_wd2 | 隐式撤销占隐式撤销+撤销之比（即`is_imp_wd / (is_imp_wd+ v_W)`）
+\- | ratio_exp_wd | 真正撤销占隐式撤销+撤销之比（即`v_W / (is_imp_wd+ v_W)`）
+\- | ratio_imp_wd_dpath | 路径属性不同的隐式撤销占隐式撤销之比（即`is_imp_wd_dpath / is_imp_wd`）
+\- | ratio_imp_wd_spath | 路径属性相同的隐式撤销占隐式撤销之比（即`is_imp_wd_spath / is_imp_wd`）
+\- | ratio_new | 全新宣告占宣告量之比（即`is_new / v_A`）
+\- | ratio_wd_dups | 重复撤销占撤销量之比（即`is_dup_wd / v_W`）
+\- | ratio_longer_path | 更长路径宣告占宣告量之比（即`is_longer_path / v_A`）
+\- | ratio_shorter_path | 更短路径宣告占宣告量之比（即`is_shorter_path / v_A`）
+\- | ratio_longer_path2 | 更长路径宣告占更长/短宣告量之比（即`is_longer_path / (is_longer_path+ is_shorter_path)`）
+\- | ratio_shorter_path2 | 更短路径宣告占更长/短宣告量之比（即`is_shorter_path / (is_longer_path+ is_shorter_path)`）
+node_level_graph | nd_degree_centrality | 节点平均度中心性
+\- | nd_node_clique_number | 节点平均最大集团数
+\- | nd_number_of_cliques | 节点平均集团数
+\- | nd_closeness_centrality | 节点平均紧密中心性
+\- | nd_betweenness_centrality | 节点平均中介中心性
+\- | nd_local_efficiency | 节点平均局部效率
+\- | nd_harmonic_centrality | 节点平均谐波中心度
+\- | nd_eigenvector_centrality | 节点平均特征向量中心度
+\- | nd_pagerank | 节点平均重要度排名
+\- | nd_clustering | 节点平均聚类中心性
+\- | nd_triangles | 节点平均三角形数量
+\- | nd_eccentricity | 节点平均偏心率
+\- | nd_average_shortest_pth_length | 节点平均最短路径长度
+\- | nd_load_centrality | 节点平均负载中心性
+\- | nd_degree | 节点平均度数
+\- | nd_square_clustering | 节点平均平方聚类系数
+\- | nd_average_neighbor_degree | 节点平均邻居度数
+AS_level_graph | gp_nb_of_nodes | 总节点数
+\- | gp_nb_of_edges | 总边数
+\- | gp_diameter | 最大偏心率
+\- | gp_assortativity | 同配性
+\- | gp_largest_eigenvalue | 最大特征值
+\- | gp_algebraic_connectivity | 代数连通度
+\- | gp_effective_graph_resistance | 有效图阻抗
+\- | gp_symmetry_ratio | 对称率
+\- | gp_natural_connectivity | 自然连通度
+\- | gp_node_connectivity | 节点连通度
+\- | gp_edge_connectivity | 边连通度
+\- | gp_weighted_spectrum_3 | 三方加权频谱
+\- | gp_weighted_spectrum_4 | 四方加权频谱
+\- | gp_percolation_limit | 渗透极限
+\- | gp_nb_spanning_trees | 生成树数量
+\- | label	|	异常类型标签
+
+
+
+
+## 特征补充
+
+字段            |  说明
+ ----           |  ----
+ConcentratRatio |  前三个最活跃的宣告前缀/宣告总数（即 `vol_ann_pfx_max / v_A`）
+
+
+## 其他注意事项 
+
+1. BGP RAW DATA: 采集时间间隔不统一，如rrc00中20030723.0745之前为15min（且时刻不固定），之后为5min（时刻固定）。
+2. MRT文件解析后，path 字段可能存在`{}`形式，如下: 
+    - 58057 6939 4635 4788 38044 23736
+    - 58057 6939 4635 4788 38044 {23736}
+    - 58057 6939 1299 2603 2603 2603 6509 {271,7860,8111,53904}
+3. `stat.ripe.net`的API获取的路由，path字段可能存在`[]`形式。
+3. `Route-Views`中的MRT文件名格式不严谨，经常出现无规律的时间戳。
+
+
+# 发现：
+- 劫持震荡：
+当`is_MOAS`很大，而`vol_oriAS_peer_pfx`或`vol_oriAS_pfx`很小时，说明存在一个prefix反复被多个AS宣告的情况。
+- outage类型难溯源
```

### Comparing `fastFET-0.0.5/fastFET.egg-info/SOURCES.txt` & `fastFET-0.0.6/fastFET.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 fastFET/FET.py
 fastFET/MultiProcess.py
 fastFET/README.md
 fastFET/RIPEStatAPI.py
 fastFET/__init__.py
 fastFET/bgpToolKit.py
 fastFET/collectData.py
+fastFET/drawing.py
 fastFET/event_list.csv
 fastFET/featGraph.py
 fastFET/featTradition.py
 fastFET/featTree.py
 fastFET/logConfig.json
 fastFET/utils.py
 fastFET.egg-info/PKG-INFO
```

