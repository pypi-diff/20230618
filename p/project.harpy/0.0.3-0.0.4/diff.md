# Comparing `tmp/project.harpy-0.0.3.tar.gz` & `tmp/project.harpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project.harpy-0.0.3.tar", last modified: Thu Jun  8 09:47:00 2023, max compression
+gzip compressed data, was "project.harpy-0.0.4.tar", last modified: Sun Jun 18 12:28:56 2023, max compression
```

## Comparing `project.harpy-0.0.3.tar` & `project.harpy-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 09:47:00.720914 project.harpy-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-04-09 02:21:24.000000 project.harpy-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      732 2023-06-08 09:47:00.720914 project.harpy-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-04-18 01:38:12.000000 project.harpy-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 09:47:00.711835 project.harpy-0.0.3/harpy/
--rw-rw-rw-   0        0        0        0 2023-04-18 02:08:24.000000 project.harpy-0.0.3/harpy/__init__.py
--rw-rw-rw-   0        0        0     2211 2023-05-15 20:34:04.000000 project.harpy-0.0.3/harpy/__main__.py
--rw-rw-rw-   0        0        0       81 2023-06-08 09:42:33.000000 project.harpy-0.0.3/harpy/__version__.py
--rw-rw-rw-   0        0        0      514 2023-04-12 19:14:24.000000 project.harpy-0.0.3/harpy/argtypes.py
--rw-rw-rw-   0        0        0     2498 2023-04-13 03:59:56.000000 project.harpy-0.0.3/harpy/cli.py
--rw-rw-rw-   0        0        0      745 2023-04-12 22:21:39.000000 project.harpy-0.0.3/harpy/consts.py
--rw-rw-rw-   0        0        0  1150157 2023-04-09 02:21:24.000000 project.harpy-0.0.3/harpy/db.json
--rw-rw-rw-   0        0        0      584 2023-04-11 18:47:25.000000 project.harpy-0.0.3/harpy/globs.py
--rw-rw-rw-   0        0        0     1224 2023-04-12 21:39:45.000000 project.harpy-0.0.3/harpy/handlers.py
--rw-rw-rw-   0        0        0     5419 2023-05-31 04:56:17.000000 project.harpy-0.0.3/harpy/net.py
--rw-rw-rw-   0        0        0     1506 2023-04-12 21:49:05.000000 project.harpy-0.0.3/harpy/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-08 09:47:00.718356 project.harpy-0.0.3/project.harpy.egg-info/
--rw-rw-rw-   0        0        0      732 2023-06-08 09:47:00.000000 project.harpy-0.0.3/project.harpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      435 2023-06-08 09:47:00.000000 project.harpy-0.0.3/project.harpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 09:47:00.000000 project.harpy-0.0.3/project.harpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-08 09:47:00.000000 project.harpy-0.0.3/project.harpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-08 09:47:00.000000 project.harpy-0.0.3/project.harpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-06-08 09:47:00.000000 project.harpy-0.0.3/project.harpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1037 2023-04-18 02:03:40.000000 project.harpy-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-08 09:47:00.720914 project.harpy-0.0.3/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-18 12:28:56.803915 project.harpy-0.0.4/
+-rwxrwxrwx   0 root         (0) root         (0)     1091 2023-04-09 02:21:24.000000 project.harpy-0.0.4/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      713 2023-06-18 12:28:56.794746 project.harpy-0.0.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       55 2023-04-18 01:38:12.000000 project.harpy-0.0.4/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-18 12:28:56.544967 project.harpy-0.0.4/harpy/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-18 02:08:24.000000 project.harpy-0.0.4/harpy/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2222 2023-06-18 12:10:45.000000 project.harpy-0.0.4/harpy/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)       81 2023-06-18 12:13:35.000000 project.harpy-0.0.4/harpy/__version__.py
+-rwxrwxrwx   0 root         (0) root         (0)      514 2023-04-12 19:14:24.000000 project.harpy-0.0.4/harpy/argtypes.py
+-rwxrwxrwx   0 root         (0) root         (0)     2627 2023-06-18 12:08:44.000000 project.harpy-0.0.4/harpy/cli.py
+-rwxrwxrwx   0 root         (0) root         (0)      745 2023-06-18 12:08:44.000000 project.harpy-0.0.4/harpy/consts.py
+-rwxrwxrwx   0 root         (0) root         (0)  1150157 2023-04-09 02:21:24.000000 project.harpy-0.0.4/harpy/db.json
+-rwxrwxrwx   0 root         (0) root         (0)      584 2023-04-11 18:47:25.000000 project.harpy-0.0.4/harpy/globs.py
+-rwxrwxrwx   0 root         (0) root         (0)     1224 2023-04-12 21:39:45.000000 project.harpy-0.0.4/harpy/handlers.py
+-rwxrwxrwx   0 root         (0) root         (0)     5549 2023-06-18 12:17:38.000000 project.harpy-0.0.4/harpy/net.py
+-rwxrwxrwx   0 root         (0) root         (0)     1515 2023-06-16 21:05:59.000000 project.harpy-0.0.4/harpy/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-18 12:28:56.759760 project.harpy-0.0.4/project.harpy.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      713 2023-06-18 12:28:55.000000 project.harpy-0.0.4/project.harpy.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      435 2023-06-18 12:28:56.000000 project.harpy-0.0.4/project.harpy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-18 12:28:55.000000 project.harpy-0.0.4/project.harpy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       46 2023-06-18 12:28:55.000000 project.harpy-0.0.4/project.harpy.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-18 12:28:55.000000 project.harpy-0.0.4/project.harpy.egg-info/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)        6 2023-06-18 12:28:55.000000 project.harpy-0.0.4/project.harpy.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1037 2023-04-18 02:03:40.000000 project.harpy-0.0.4/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-18 12:28:56.804925 project.harpy-0.0.4/setup.cfg
```

### Comparing `project.harpy-0.0.3/LICENSE` & `project.harpy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `project.harpy-0.0.3/PKG-INFO` & `project.harpy-0.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1
-Name: project.harpy
-Version: 0.0.3
-Summary: Active/passive ARP discovery tool
-Author: Serhat Çelik
-License: MIT
-Keywords: harpy,arp,discovery
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: System :: Networking
-Classifier: Topic :: System :: Networking :: Monitoring
-Requires-Python: ~=3.10
-License-File: LICENSE
+Metadata-Version: 2.1
+Name: project.harpy
+Version: 0.0.4
+Summary: Active/passive ARP discovery tool
+Author: Serhat Çelik
+License: MIT
+Keywords: harpy,arp,discovery
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: System :: Networking
+Classifier: Topic :: System :: Networking :: Monitoring
+Requires-Python: ~=3.10
+License-File: LICENSE
```

### Comparing `project.harpy-0.0.3/harpy/__main__.py` & `project.harpy-0.0.4/harpy/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 import threading
 
 from harpy.cli import Namespace, parser
 from harpy.consts import CLS, GGP, LOGO, PORT, WAIT_PRINT
 from harpy.globs import controller, interrupts, sent
 from harpy.handlers import Echo, Is
 from harpy.net import Sender, Sniffer
-from harpy.utils import get_manuf_db, ignore, signal_
+from harpy.utils import get_manuf_db, ignore, safesignal
 
 
 def start() -> list[threading.Thread]:
     """Start the program."""
     opts = parser.parse_args(namespace=Namespace())
 
-    signal_(signal.SIGINT, stop)
+    safesignal(signal.SIGINT, stop)
 
     Echo.disable()
 
     sock = socket.socket(socket.PF_PACKET, socket.SOCK_RAW, socket.htons(GGP))
 
     atexit.register(sock.close)
 
@@ -33,34 +33,34 @@
 
     sock.bind((opts.device, PORT))
 
     manuf_db = get_manuf_db(os.path.join(os.path.dirname(__file__), 'db.json'))
 
     threads = []  # type: list[threading.Thread]
 
-    sniffer = Sniffer(sock, opts.network, manuf_db, opts.F, opts.S)
+    sniffer = Sniffer(sock, opts.netw, manuf_db, opts.F, opts.S)
     threads.append(sniffer)
 
     if not opts.p:
-        sender = Sender(sock, opts.network, opts.node, opts.sleep, opts.R)
+        sender = Sender(sock, opts.netw, opts.node, opts.sleep, opts.f, opts.R)
         threads.append(sender)
 
     for thread in threads:
         thread.start()
 
     while not controller.wait(WAIT_PRINT):  # Non-blocking wait
         with ignore(signal.SIGINT):
             print(CLS, *LOGO, *sniffer, opts() + '>\t' + sent.get(), sep='\n')
 
     return threads
 
 
 def stop(*args):
     """Stop the program."""
-    signal_(signal.SIGINT, signal.SIG_IGN)
+    safesignal(signal.SIGINT, signal.SIG_IGN)
     controller.set()
 
 
 def join(threads: list[threading.Thread]):
     """Join all threads."""
     for thread in threads:
         thread.join()
```

### Comparing `project.harpy-0.0.3/harpy/argtypes.py` & `project.harpy-0.0.4/harpy/argtypes.py`

 * *Files identical despite different names*

### Comparing `project.harpy-0.0.3/harpy/cli.py` & `project.harpy-0.0.4/harpy/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 mutual = modes.add_mutually_exclusive_group()
 
 ########################
 # Positional Arguments #
 ########################
 parser.add_argument(
-    'network',
+    'netw',
     type=ipv4,
     help='ip range in cidr format',
     metavar='range',
 )
 
 ###########
 # Options #
@@ -75,14 +75,20 @@
     version=__version__,
 )
 
 #########
 # Modes #
 #########
 modes.add_argument(
+    '-f',
+    action='store_true',
+    help='enable fast mode, only scan specific hosts',
+    dest='f',
+)
+modes.add_argument(
     '-F',
     action='store_true',
     help='enable filter mode, exclude hosts not in range',
     dest='F',
 )
 mutual.add_argument(
     '-p',
```

### Comparing `project.harpy-0.0.3/harpy/consts.py` & `project.harpy-0.0.4/harpy/consts.py`

 * *Files identical despite different names*

### Comparing `project.harpy-0.0.3/harpy/db.json` & `project.harpy-0.0.4/harpy/db.json`

 * *Files identical despite different names*

### Comparing `project.harpy-0.0.3/harpy/globs.py` & `project.harpy-0.0.4/harpy/globs.py`

 * *Files identical despite different names*

### Comparing `project.harpy-0.0.3/harpy/handlers.py` & `project.harpy-0.0.4/harpy/handlers.py`

 * *Files identical despite different names*

### Comparing `project.harpy-0.0.3/harpy/net.py` & `project.harpy-0.0.4/harpy/net.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,41 +26,45 @@
 class Thread(threading.Thread):
     """Base class for network threads."""
 
     def __init__(self, s: socket.socket, n: ipaddress.IPv4Network):
         super().__init__()
 
         self.sock = s
-        self.network = n
+        self.netw = n
 
         self.src = s.getsockname()[-1].hex()
         self.sha = self.src
 
 
 class Sender(Thread):
     """Sender thread."""
 
     name = 'Sender'
 
-    def __init__(self, s, n, node: int, sleep: int, repeat: bool):
+    def __init__(self, s, n, node: int, sleep: int, fast: bool, repeat: bool):
         super().__init__(s, n)
 
         self.node = node
         self.sleep = sleep / 1000
+        self.fast = fast
         self.repeat = repeat
 
         self.hosts = iter(n.hosts()) if not repeat else cycle(n.hosts())
 
     def run(self):
         """Method representing the thread's activity."""
         while not controller.is_set() and (host := next(self.hosts, None)):
             tpa = str(host)
 
             node = int(tpa.rsplit('.', 1)[-1])
 
+            if self.fast and node not in [1, 2, 100, 127, 200, 254]:
+                continue
+
             # Fix gratuitous ARP
             spa = str(host - node + (node != self.node) * self.node)
 
             # https://en.wikipedia.org/wiki/Ethernet_frame
             eth = struct.pack(
                 FMT_ETH,
                 b'\xff' * 6,  # Destination MAC Address
@@ -159,15 +163,15 @@
             if eth[2] != b'\x08\x06':
                 continue
 
             arp = struct.unpack(FMT_ARP, packet[BUF_ETH:BUFSIZE])
 
             spa = socket.inet_ntoa(arp[6])
 
-            if self.exclude and ipaddress.IPv4Address(spa) not in self.network:
+            if self.exclude and ipaddress.IPv4Address(spa) not in self.netw:
                 continue
 
             who_has = int(arp[4] == b'\x00\x01')
             is_at = 1 - who_has
 
             sha = arp[5].hex()
```

### Comparing `project.harpy-0.0.3/harpy/utils.py` & `project.harpy-0.0.4/harpy/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,19 +38,19 @@
     return {}
 
 
 @contextmanager
 def ignore(signum: signal.Signals) -> Generator[None, None, None]:
     """Ignore the given signal during the execution."""
     handler = signal.getsignal(signum)
-    signal_(signum, signal.SIG_IGN)
+    safesignal(signum, signal.SIG_IGN)
     yield
-    signal_(signum, handler)
+    safesignal(signum, handler)
 
 
-def signal_(signum: signal.Signals, handler):
+def safesignal(signum: signal.Signals, handler):
     """Thread-safe signal."""
     if threading.current_thread() is not threading.main_thread():
         return
     # https://github.com/python/cpython/issues/67584
     with suppress(TypeError):
         signal.signal(signum, handler)
```

### Comparing `project.harpy-0.0.3/project.harpy.egg-info/PKG-INFO` & `project.harpy-0.0.4/project.harpy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1
-Name: project.harpy
-Version: 0.0.3
-Summary: Active/passive ARP discovery tool
-Author: Serhat Çelik
-License: MIT
-Keywords: harpy,arp,discovery
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: System :: Networking
-Classifier: Topic :: System :: Networking :: Monitoring
-Requires-Python: ~=3.10
-License-File: LICENSE
+Metadata-Version: 2.1
+Name: project.harpy
+Version: 0.0.4
+Summary: Active/passive ARP discovery tool
+Author: Serhat Çelik
+License: MIT
+Keywords: harpy,arp,discovery
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: System :: Networking
+Classifier: Topic :: System :: Networking :: Monitoring
+Requires-Python: ~=3.10
+License-File: LICENSE
```

### Comparing `project.harpy-0.0.3/pyproject.toml` & `project.harpy-0.0.4/pyproject.toml`

 * *Files identical despite different names*

