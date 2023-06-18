# Comparing `tmp/pyWalletConnect-1.3.3-py3-none-any.whl.zip` & `tmp/pyWalletConnect-1.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 41158 bytes, number of entries: 17
+Zip file size: 41318 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat      909 b- defN 22-Feb-07 21:32 pywalletconnect/__init__.py
 -rw-rw-rw-  2.0 fat     1196 b- defN 23-Jan-25 19:46 pywalletconnect/base58.py
--rw-rw-rw-  2.0 fat     6980 b- defN 23-Feb-26 19:07 pywalletconnect/client.py
+-rw-rw-rw-  2.0 fat     6978 b- defN 23-Jun-18 16:35 pywalletconnect/client.py
 -rw-rw-rw-  2.0 fat     7767 b- defN 23-Jan-25 19:46 pywalletconnect/client_v1.py
 -rw-rw-rw-  2.0 fat    15538 b- defN 23-Feb-26 19:08 pywalletconnect/client_v2irn.py
--rw-rw-rw-  2.0 fat    14542 b- defN 23-Jan-25 19:46 pywalletconnect/client_v2waku.py
+-rw-rw-rw-  2.0 fat    14424 b- defN 23-Jun-18 16:35 pywalletconnect/client_v2waku.py
 -rw-rw-rw-  2.0 fat     8770 b- defN 23-Jan-25 19:46 pywalletconnect/enc_tunnel.py
--rw-rw-rw-  2.0 fat     2940 b- defN 23-Feb-26 19:11 pywalletconnect/json_rpc.py
+-rw-rw-rw-  2.0 fat     2901 b- defN 23-Jun-18 16:35 pywalletconnect/json_rpc.py
 -rw-rw-rw-  2.0 fat     2282 b- defN 22-Feb-07 21:32 pywalletconnect/tls_socket.py
--rw-rw-rw-  2.0 fat       58 b- defN 23-Feb-26 20:11 pywalletconnect/version.py
+-rw-rw-rw-  2.0 fat       58 b- defN 23-Jun-18 16:35 pywalletconnect/version.py
 -rw-rw-rw-  2.0 fat     7965 b- defN 23-Jan-25 20:08 pywalletconnect/websocket.py
 -rw-rw-rw-  2.0 fat     1875 b- defN 23-Jan-25 19:46 pywalletconnect/ws_auth.py
--rw-rw-rw-  2.0 fat    35149 b- defN 23-Feb-27 09:26 pyWalletConnect-1.3.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    10657 b- defN 23-Feb-27 09:26 pyWalletConnect-1.3.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Feb-27 09:26 pyWalletConnect-1.3.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Feb-27 09:26 pyWalletConnect-1.3.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1444 b- defN 23-Feb-27 09:26 pyWalletConnect-1.3.3.dist-info/RECORD
-17 files, 118180 bytes uncompressed, 38780 bytes compressed:  67.2%
+-rw-rw-rw-  2.0 fat    35149 b- defN 23-Jun-18 16:55 pyWalletConnect-1.4.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    11532 b- defN 23-Jun-18 16:55 pyWalletConnect-1.4.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-18 16:55 pyWalletConnect-1.4.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-18 16:55 pyWalletConnect-1.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1444 b- defN 23-Jun-18 16:55 pyWalletConnect-1.4.0.dist-info/RECORD
+17 files, 118896 bytes uncompressed, 38940 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: pywalletconnect/websocket.py
 Comment: 
 
 Filename: pywalletconnect/ws_auth.py
 Comment: 
 
-Filename: pyWalletConnect-1.3.3.dist-info/LICENSE
+Filename: pyWalletConnect-1.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: pyWalletConnect-1.3.3.dist-info/METADATA
+Filename: pyWalletConnect-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: pyWalletConnect-1.3.3.dist-info/WHEEL
+Filename: pyWalletConnect-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: pyWalletConnect-1.3.3.dist-info/top_level.txt
+Filename: pyWalletConnect-1.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyWalletConnect-1.3.3.dist-info/RECORD
+Filename: pyWalletConnect-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pywalletconnect/client.py

```diff
@@ -104,15 +104,14 @@
                 }
                 logger.debug("Sending a WCv1 close message.")
                 self.write(datafull)
                 sleep(0.15)
                 logger.debug("WCv1 close message sent.")
 
         if isinstance(self, WCv2Client) and self.wallet_id:
-
             try:
                 sess_delete = rpc_query(
                     "wc_sessionDelete", {"code": 6000, "message": "User disconnected."}
                 )
                 msgsessdel = self.topics[self.wallet_id][
                     "secure_channel"
                 ].encrypt_payload(json_encode(sess_delete))
```

## pywalletconnect/client_v2waku.py

```diff
@@ -1,14 +1,10 @@
 from urllib.parse import urlparse, parse_qs
-from json import loads
 from logging import getLogger
-from re import compile as regex_compile
-from threading import Timer
 from time import sleep, time
-from uuid import uuid4
 
 from .websocket import WebSocketClient, CYCLES_TIMEOUT, UNIT_WAITING_TIME
 from .enc_tunnel import (
     EncryptedTunnelv2,
     KeyAgreement,
 )
 from .json_rpc import (
```

## pywalletconnect/json_rpc.py

```diff
@@ -14,14 +14,15 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 
 
 """JSON RPC for pyWalletConnect"""
 
 
 from json import dumps, loads
+from time import time_ns
 
 
 # ---- Helpers about messages encoding
 
 
 def json_encode(dataobj):
     """Compact JSON encoding."""
@@ -29,24 +30,19 @@
 
 
 # ---- JSON RPC functions to pack/unpack
 
 # The wallet is a JSON-RPC service in the WalletConnect standard
 
 
-id_counter = 0
-
-
 def rpc_query(method, params):
     """Build a JSON-RPC query object."""
-    global id_counter
-    id_counter += 1
     return {
         "jsonrpc": "2.0",
-        "id": id_counter,
+        "id": time_ns(),
         "method": method,
         "params": params,
     }
 
 
 def json_rpc_unpack_response(raw_response):
     """Decode JSON-RPC raw bytes response and return result."""
```

## pywalletconnect/version.py

```diff
@@ -1,3 +1,3 @@
 """pyWalletConnect version info."""
 
-VERSION = "1.3.3"
+VERSION = "1.4.0"
```

## Comparing `pyWalletConnect-1.3.3.dist-info/LICENSE` & `pyWalletConnect-1.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyWalletConnect-1.3.3.dist-info/METADATA` & `pyWalletConnect-1.4.0.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,247 +1,257 @@
-Metadata-Version: 2.1
-Name: pyWalletConnect
-Version: 1.3.3
-Summary: WalletConnect implementation for Python wallets
-Home-page: https://github.com/bitlogik/pyWalletConnect
-Author: BitLogiK
-Author-email: contact@bitlogik.fr
-License: GPLv3
-Keywords: blockchain wallet cryptography security
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
-Classifier: Intended Audience :: Telecommunications Industry
-Classifier: Topic :: Security :: Cryptography
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.1
-Description-Content-Type: text/markdown
-Requires-Dist: cryptography (>=3.3)
-Requires-Dist: wsproto (>=1.0.0)
-
-
-# pyWalletConnect
-
-![pyWalletConnect logo](logo.png)
-
-### A WalletConnect implementation for wallets in Python
-
-A Python3 library to link a wallet with a WalletConnect web3 app. This library connects a Python wallet with a web3 app online, using the WalletConnect standard.
-
-Thanks to WalletConnect, a Dapp is able to send JSON-RPC call requests to be handled by the Wallet, sign requests for transactions or messages remotely. Using WalletConnect, the wallet is a JSON-RPC service that the dapp can query through an encrypted tunnel and an online relay. This library is built for the wallet part, which establishes a link with the dapp and receives requests.
-
-WalletConnect version 2 support is beta.
-
-pyWalletConnect manages automatically on its own all the WalletConnect stack :
-
-```
-WalletConnect
-    |
- Topics managt
-    |
- JSON-RPC
-    |
-EncryptedTunnel
-    |
- WebSocket
-    |
-   HTTP
-    |
-   TLS
-    |
-  Socket
-```
-
-## Installation and requirements
-
-Works with Python >= 3.6.
-
-### Installation of this library
-
-Easiest way :  
-`python3 -m pip install pyWalletConnect`  
-
-From sources, download and run in this directory :  
-`python3 -m pip  install .`
-
-### Use
-
-Instanciate with `pywalletconnect.WCClient.from_wc_uri`, then use methods functions of this object.
-
-Basic example :
-
-```python
-from pywalletconnect import WCClient, WCClientInvalidOption
-# Input the wc URI
-string_uri = input("Input the WalletConnect URI : ")
-WCClient.set_wallet_metadata(WALLET_METADATA)  # Optional, else identify pyWalletConnect as wallet
-WCClient.set_project_id(WALLETCONNECT_PROJECT_ID)  # Required for v2
-WCClient.set_origin(WALLETCONNECT_ORIGIN_DOMAIN)  # Optional for v2
-try:
-    wallet_dapp = WCClient.from_wc_uri(string_uri)
-except WCClientInvalidOption as exc:
-    # In case error in the wc URI provided
-    wallet_dapp.close()
-    raise InvalidOption(exc)
-# Wait for the sessionRequest info
-# Can throw WCClientException "sessionRequest timeout"
-req_id, req_chain_id, request_info = wallet_dapp.open_session()
-if req_chain_id != account.chainID:
-    # Chain id mismatch
-    wallet_dapp.close()
-    raise InvalidOption("Chain ID from Dapp is not the same as the wallet.")
-# Display to the user request details provided by the Dapp.
-user_ok = input(f"WalletConnect link request from : {request_info['name']}. Approve? [y/N]")
-if user_ok.lower() == "y":
-    # User approved
-    wallet_dapp.reply_session_request(req_id, account.chainID, account.address)
-    # Now the session with the Dapp is opened
-    <...>
-else:
-    # User rejected
-    wclient.reject_session_request(req_id)
-    wallet_dapp.close()
-    raise UserInteration("user rejected the dapp connection request.")
-```
-
-There's a basic minimal working CLI demo at: https://gist.github.com/bitlogik/89b41bb60443c041704f82bcd9b43901
-
-pyWalletConnect maintains a TLS WebSocket opened with the host relay. It builds an internal pool of received request messages from the dapp.
-
-Once the session is opened, you can read the pending messages received from the Dapp from time to time. And then your wallet app can process these requests, and send back the reply.
-
-Use a daemon thread timer for example, to call the `get_message()` method in a short time frequency. 3-6 seconds is an acceptable delay. This can also be performed in a blocking *for* loop with a sleeping time. Then process the Dapp queries for further user wallet actions.
-
-Remember to keep track of the request id, as it is needed for `.reply(req_id, result)` ultimately when sending the processing result back to the dapp service. One way is to provide the id in argument in your processing methods. Also this can be done with global or shared parameters.
-
-When a WCClient object created from a WC link is closed or deleted, it will send to the dapp a closing session message.
-
-```python
-def process_sendtransaction(call_id, tx):
-    # Processing the RPC query eth_sendTransaction
-    # Collect the user approval about the tx query
-    < Accept (tx) ? >
-    if approved :
-        # Build and sign the provided transaction
-        <...>
-        # Broadcast the tx
-        # Provide the transaction id as result
-        return "0x..." # Tx id
-
-def watch_messages():
-    # Watch for messages received.
-    # For WalletConnect calls reading.
-    # Read all the message requests received from the dapp.
-    # Then dispatch to the wallet service handlers.
-    # get_message gives (id, method, params) or (None, "", [])
-    wc_message = wallet_dapp.get_message()
-    # Loop in the waiting messages pool, until depleted
-    while wc_message[0] is not None:
-        # Read a WalletConnect call message available
-        id_request = wc_message[0]
-        method = wc_message[1]
-        parameters = wc_message[2]
-        if "wc_sessionUpdate" == method:
-            if parameters[0].get("approved") is False:
-                raise Exception("Disconnected by the Dapp.")
-        # Dispatch query processing
-        elif "eth_signTypedData" == method:
-            result = process_signtypeddata(id_request, parameters[1])
-            wallet_dapp.reply(call_id, result)
-        elif "eth_sendTransaction" == method:
-            tx_to_sign = parameters[1]
-            result = process_sendtransaction(id_request, tx_to_sign)
-            wallet_dapp.reply(call_id, result)
-        elif "eth_sign" == method:
-            result = process_signtransaction(parameters[1])
-            wallet_dapp.reply(call_id, result)
-        <...>
-        # Next loop
-        wc_message = wallet_dapp.get_message()
-
-
-# GUI timer repeated or threading daemon
-# Will call watch_messages every 4 seconds
-apptimer = Timer(4000)
-# Call watch_messages when expires periodically
-apptimer.notify = watch_messages
-
-```
-
-See also the [RPC methods in WalletConnect](https://docs.walletconnect.org/v/1.0/json-rpc-api-methods/ethereum) to know more about the expected result regarding a specific RPC call.
-
-## Interface methods of WCClient
-
-`WCClient.set_wallet_metadata( wallet_metadata )`  
-Class method to set the wallet metadata as object (v2). See WalletConnect standard for the format.  
-Optional. If not provided, when v2, it sends the default pyWalletConnect metadata as wallet identification.
-
-`WCClient.set_project_id( project_id )`  
-Class method to set the WalletConnect project id. This is mandatory to use a project id when  
-using WC v2 with the official central bridge relay.
-
-`WCClient.set_origin( origin_domain )`  
-Class method to set the origin of the first HTTP query for websocket. Only for v2, optional.
-
-`WCClient.from_wc_uri( wc_uri_str )`  
-Create a WalletConnect wallet client from a wc v1 or v2 URI. (class method constructor)  
-*wc_uri_str* : the wc full EIP1328 URI provided by the Dapp.  
-You need to call *open_session* immediately after to get the session request info.
-
-`.close()`  
-Send a session close message, and close the underlying WebSocket connection.
-
-`.get_relay_url()`  
-Give the page address of the WebSocket relay bridge.
-
-`.get_message()`  
-Get a RPC call message from the internal waiting list. pyWalletConnect maintains an internal pool of received request messages from the dapp. And this get_message method pops out a message in a FIFO manner : the first method call provides the oldest (first) received message. It can be used like a pump : call *get_message()* until an empty response. Because it reads a message from the receiving bucket one by one.  
-This needs to be called periodically because this triggers the auto reconnection (When the WebSocket is abruptly disconnected by the relay).  
-Return : (RPCid, method, params) or (None, "", []) when no data were received since the last call (or from the initial session connection).  
-Non-blocking, so always returns immediately when there's no message, and returns (None, "", []).  
-When a v2 ping *wc_sessionPing* is received, it is automatically replied when getting it with get_message. In this case, the *get_message* method returns an empty method and no params. So filter *get_message* calls with 'id is None', means no more message left.
-
-`.reply( req_id, result_str )`  
-Send a RPC response to the webapp (through the relay).  
-*req_id* is the JSON-RPC id of the corresponding query request, where the result belongs to. One must kept track this id from the get_message, up to this reply. So a reply result is given back with its associated call query id.  
-*result_str* is the result field to provide in the RPC result response.
-
-`.open_session()`  
-Start a WalletConnect session : wait for the session call request message.  
-Must be called right after a WCClient creation.  
-Returns : (message RPCid, chain ID, peerMeta data object).  
-Or throws WalletConnectClientException("sessionRequest timeout")
-after 8 seconds and no sessionRequest received.
-
-`reply_session_request( msg_id, chain_id, account_address )`  
-Send a session approval message, when user approved the connection session request in the wallet.  
-*msg_id* is the RPC id of the session approval request.
-
-`.reject_session_request( req_id )`  
-Send a session rejection message to the webapp (through the relay). *req_id* is the RPC id of the session approval request.
-
-
-## License
-
-Copyright (C) 2021-2023  BitLogiK SAS
-
-This program is free software: you can redistribute it and/or modify  
-it under the terms of the GNU General Public License as published by  
-the Free Software Foundation, version 3 of the License.
-
-This program is distributed in the hope that it will be useful,  
-but WITHOUT ANY WARRANTY; without even the implied warranty of  
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  
-See the GNU General Public License for more details.
-
-
-## Support
-
-Open an issue in the Github repository for help about its use.
-
-
-
-
+Metadata-Version: 2.1
+Name: pyWalletConnect
+Version: 1.4.0
+Summary: WalletConnect implementation for Python wallets
+Home-page: https://github.com/bitlogik/pyWalletConnect
+Author: BitLogiK
+Author-email: contact@bitlogik.fr
+License: GPLv3
+Keywords: blockchain wallet cryptography security
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Telecommunications Industry
+Classifier: Topic :: Security :: Cryptography
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Requires-Dist: cryptography (>=3.3)
+Requires-Dist: wsproto (>=1.0.0)
+
+
+# pyWalletConnect
+
+![pyWalletConnect logo](logo.png)
+
+### A WalletConnect implementation for wallets in Python
+
+A Python3 library to link a wallet with a WalletConnect web3 app. This library connects a Python wallet with a web3 app online, using the WalletConnect standard.
+
+Thanks to WalletConnect, a Dapp is able to send JSON-RPC call requests to be handled by the wallet, remotely signing transactions or messages. Using WalletConnect, the wallet is a JSON-RPC service that the dapp can query through an encrypted tunnel and an online relay. This library is built for the wallet part, which establishes a link with the dapp and receives requests.
+
+pyWalletConnect manages automatically on its own all the WalletConnect stack :
+
+```
+WalletConnect
+    |
+Topics mgmt
+    |
+ JSON-RPC
+    |
+EncryptedTunnel
+    |
+ WebSocket
+    |
+   HTTP
+    |
+   TLS
+    |
+  Socket
+```
+
+## Installation and requirements
+
+Works with Python >= 3.7.
+
+### Installation of this library
+
+Easiest way :  
+`python3 -m pip install pyWalletConnect`  
+
+From sources, download and run in this directory :  
+`python3 -m pip  install .`
+
+### Use
+
+Instanciate with `pywalletconnect.WCClient.from_wc_uri`, then use methods functions of this object.
+
+Basic example :
+
+```python
+from pywalletconnect import WCClient, WCClientInvalidOption
+# Input the wc URI
+string_uri = input("Input the WalletConnect URI : ")
+WCClient.set_wallet_metadata(WALLET_METADATA)  # Optional, else identify pyWalletConnect as wallet
+WCClient.set_project_id(WALLETCONNECT_PROJECT_ID)  # Required for v2
+WCClient.set_origin(WALLETCONNECT_ORIGIN_DOMAIN)  # Optional for v2
+try:
+    wallet_dapp = WCClient.from_wc_uri(string_uri)
+except WCClientInvalidOption as exc:
+    # In case error in the wc URI provided
+    if hasattr(wallet_dapp, "wc_client"):
+        wallet_dapp.close()
+    raise InvalidOption(exc)
+# Wait for the sessionRequest info
+# Can throw WCClientException "sessionRequest timeout"
+req_id, req_chain_id, request_info = wallet_dapp.open_session()
+if req_chain_id != account.chainID:
+    # Chain id mismatch
+    wallet_dapp.close()
+    raise InvalidOption("Chain ID from Dapp is not the same as the wallet.")
+# Display to the user request details provided by the Dapp.
+user_ok = input(f"WalletConnect link request from : {request_info['name']}. Approve? [y/N]")
+if user_ok.lower() == "y":
+    # User approved
+    wallet_dapp.reply_session_request(req_id, account.chainID, account.address)
+    # Now the session with the Dapp is opened
+    <...>
+else:
+    # User rejected
+    wclient.reject_session_request(req_id)
+    wallet_dapp.close()
+    raise UserInteration("user rejected the dapp connection request.")
+```
+
+There's a basic minimal working CLI demo at: https://gist.github.com/bitlogik/89b41bb60443c041704f82bcd9b43901
+
+pyWalletConnect maintains a TLS WebSocket opened with the host relay. It builds an internal pool of received request messages from the dapp.
+
+Once the session is opened, you can read the pending messages received from the Dapp from time to time. And then your wallet app can process these requests, and send back the reply.
+
+Use a daemon thread timer for example, to call the `get_message()` method in a short time frequency. 3-6 seconds is an acceptable delay. This can also be performed in a blocking *for* loop with a sleeping time. Then process the Dapp queries for further user wallet actions.
+
+Remember to keep track of the request id, as it is needed for `.reply(req_id, result)` ultimately when sending the processing result back to the dapp service. One way is to provide the id in argument in your processing methods. Also this can be done with global or shared parameters.
+
+When a WCClient object (created from a WC link) is closed or deleted, it will automatically send to the dapp a closing session message.
+
+```python
+
+def process_sendtransaction(call_id, tx):
+    # Processing the RPC query eth_sendTransaction
+    # Collect the user approval about the tx query
+    < Accept (tx) ? >
+    if approved :
+        # Build and sign the provided transaction
+        <...>
+        # Broadcast the tx
+        # Provide the transaction id as result
+        return "0x..." # Tx id
+
+def watch_messages():
+    # Watch for messages received.
+    # For WalletConnect calls reading.
+    # Read all the message requests received from the dapp.
+    # Then dispatch to the wallet service handlers.
+    # get_message gives (id, method, params) or (None, "", [])
+    wc_message = wallet_dapp.get_message()
+    # Loop in the waiting messages pool, until depleted
+    while wc_message[0] is not None:
+        # Read a WalletConnect call message available
+        id_request = wc_message[0]
+        method = wc_message[1]
+        parameters = wc_message[2]
+        if method == "wc_sessionRequest" or method == "wc_sessionPayload":
+            # Read if v2 and convert to v1 format
+            if parameters.get("request"):
+                method = parameters["request"].get("method")
+                parameters = parameters["request"].get("params")
+        if "wc_sessionUpdate" == method:
+            if parameters[0].get("approved") is False:
+                raise Exception("Disconnected by the Dapp.")
+        #  v2 disconnect
+        if "wc_sessionDelete" == method:
+            raise Exception("Disconnected by the Dapp.")
+        # Dispatch query processing
+        elif "eth_signTypedData" == method:
+            result = process_signtypeddata(id_request, parameters[1])
+            wallet_dapp.reply(call_id, result)
+        elif "eth_sendTransaction" == method:
+            result = process_sendtransaction(id_request, parameters[0])
+            wallet_dapp.reply(call_id, result)
+        elif "eth_sign" == method:
+            result = process_signtransaction(parameters[1])
+            wallet_dapp.reply(call_id, result)
+        <...>
+        # Next loop
+        wc_message = wallet_dapp.get_message()
+
+
+# GUI timer repeated or threading daemon
+# Will call watch_messages every 4 seconds
+apptimer = Timer(4000)
+# Call watch_messages when expires periodically
+apptimer.notify = watch_messages
+
+```
+
+See also the [RPC methods in WalletConnect](https://docs.walletconnect.org/v/1.0/json-rpc-api-methods/ethereum) to know more about the expected result regarding a specific RPC call.
+
+## Interface methods of WCClient
+
+`WCClient.set_wallet_metadata( wallet_metadata )`  
+Class method to set the wallet metadata as object (v2). See [the WalletConnect standard for the format details](https://docs.walletconnect.com/2.0/specs/clients/core/pairing/data-structures#metadata).  
+Optional. If not provided, when v2, it sends the default pyWalletConnect metadata as wallet identification.
+
+`WCClient.set_project_id( project_id )`  
+Class method to set the WalletConnect project id. This is mandatory to use a project id when  
+using WC v2 with the official central bridge relay.
+
+`WCClient.set_origin( origin_domain )`  
+Class method to set the origin of the first HTTP query for websocket. Only for v2, optional.
+
+`WCClient.from_wc_uri( wc_uri_str )`  
+Create a WalletConnect wallet client from a wc v1 or v2 URI. (class method constructor)  
+*wc_uri_str* : the wc full EIP1328 URI provided by the Dapp.  
+You need to call *open_session* immediately after to get the session request info.
+
+`.close()`  
+Send a session close message, and close the underlying WebSocket connection.
+
+`.get_relay_url()`  
+Give the page address of the WebSocket relay bridge.
+
+`.get_message()`  
+Get a RPC call message from the internal waiting list. pyWalletConnect maintains an internal pool of received request messages from the dapp. And this get_message method pops out a message in a FIFO manner : the first method call provides the oldest (first) received message. It can be used like a pump : call *get_message()* until an empty response. Because it reads a message from the receiving bucket one by one.  
+This needs to be called periodically because this triggers the auto reconnection (When the WebSocket is abruptly disconnected by the relay).  
+Return : (RPCid, method, params) or (None, "", []) when no data were received since the last call (or from the initial session connection).  
+Non-blocking, so always returns immediately when there's no message, and returns (None, "", []).  
+When a v2 ping *wc_sessionPing* is received, it is automatically replied when getting it with get_message. In this case, the *get_message* method returns an empty method and no params. So filter *get_message* calls with 'id is None', means no more message left.
+
+`.reply( req_id, result_str )`  
+Send a RPC response to the webapp (through the relay).  
+*req_id* is the JSON-RPC id of the corresponding query request, where the result belongs to. One must kept track this id from the get_message, up to this reply. So a reply result is given back with its associated call query id.  
+*result_str* is the result field to provide in the RPC result response.
+
+`.open_session()`  
+Start a WalletConnect session : wait for the session call request message.  
+Must be called right after a WCClient creation.  
+Returns : (message RPCid, chain ID, peerMeta data object).  
+Or throws WalletConnectClientException("sessionRequest timeout")
+after 8 seconds and no sessionRequest received.
+
+`reply_session_request( msg_id, chain_id, account_address )`  
+Send a session approval message, when user approved the connection session request in the wallet.  
+*msg_id* is the RPC id of the session approval request.
+*chain_id* is the integer ideitifying the blockchain.
+*account_address* is a string of the address of the wallet account ("0x...").
+
+`.reject_session_request( req_id )`  
+Send a session rejection message to the dapp (through the relay).
+*req_id* is the RPC id of the session approval request.
+
+
+## License
+
+Copyright (C) 2021-2023  BitLogiK SAS
+
+This program is free software: you can redistribute it and/or modify  
+it under the terms of the GNU General Public License as published by  
+the Free Software Foundation, version 3 of the License.
+
+This program is distributed in the hope that it will be useful,  
+but WITHOUT ANY WARRANTY; without even the implied warranty of  
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  
+See the GNU General Public License for more details.
+
+
+## Support
+
+Open an issue in the Github repository for help about its use.
+
+
+
+
```

## Comparing `pyWalletConnect-1.3.3.dist-info/RECORD` & `pyWalletConnect-1.4.0.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 pywalletconnect/__init__.py,sha256=twRPUf3Ev6qvN54VuD79HBrxMXZMzwFqJDwJADyFWF8,909
 pywalletconnect/base58.py,sha256=f5ALRFwEFd7IMX946WyQNK5A-yGeOwuU5v6Z-Bnhd6s,1196
-pywalletconnect/client.py,sha256=1Gzp4Vzz-uetj3Tq3MSWKn5BbG2vpcHo0NJEb1odEhg,6980
+pywalletconnect/client.py,sha256=GGD--bPnYhm1tCZJeIdv2tija1pN-U42gt0fQuM142U,6978
 pywalletconnect/client_v1.py,sha256=TAK5iAoPwcjZcv_44yJ9HIxcaJnXXSDoNTc27Pqo0lY,7767
 pywalletconnect/client_v2irn.py,sha256=cuDXivQhzErYbOg-50Epx7ubA091yehzqQWZ26Gnk1U,15538
-pywalletconnect/client_v2waku.py,sha256=Gz0Cv5tWdEQ_PmNvMXaE8dHhfi-2QntVGxqkvLgslxw,14542
+pywalletconnect/client_v2waku.py,sha256=k8d38tV1tmCOZXQXC_ee_2ZV5zNLxuGC6g8XrqNaJqA,14424
 pywalletconnect/enc_tunnel.py,sha256=8f-qtBFmqiOgsNgD42DX_ujJSRjOOJPI-gnGfWFyqEI,8770
-pywalletconnect/json_rpc.py,sha256=0a86QTrc-XFkw6l-dIDC6hnBhJQng0jEfW0ZUiv0rXI,2940
+pywalletconnect/json_rpc.py,sha256=feF74KmNilFcWOG_N-WKnRrWOsH2iz5T8EM-NCDV8-g,2901
 pywalletconnect/tls_socket.py,sha256=8-8uyReJsRv7WqzW43F5RbAvp7FuHFp_HQQU-bVBGbA,2282
-pywalletconnect/version.py,sha256=scNJV8HF7e34lk0XHd4ZlGZyg6Seg6jNeoFLhMEZ8F8,58
+pywalletconnect/version.py,sha256=irvhv0xkqzz8zaIDL-WXidDrhoSuPyGncJnxOWSu-yc,58
 pywalletconnect/websocket.py,sha256=iE7I2wSLFCG1gSwweyJ23ycWIKGUXABJ_xXA2yk_POY,7965
 pywalletconnect/ws_auth.py,sha256=Et-kzX8ZyeGrrAbMQWMGsU3HW4cGzkteaOSGQdwvID0,1875
-pyWalletConnect-1.3.3.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-pyWalletConnect-1.3.3.dist-info/METADATA,sha256=zr28Sm1s_SjY4FqlxElju9LEoU9_zy2gQz0VTHHtdgk,10657
-pyWalletConnect-1.3.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyWalletConnect-1.3.3.dist-info/top_level.txt,sha256=MeiZvwObGZFsa0avWx0Bg--YOWz1SZQF7PV-Q1z3OLo,16
-pyWalletConnect-1.3.3.dist-info/RECORD,,
+pyWalletConnect-1.4.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+pyWalletConnect-1.4.0.dist-info/METADATA,sha256=w0KJK3SCmj5O2EQpmjeKqf18O8gelddy9nbrKc9JBlk,11532
+pyWalletConnect-1.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyWalletConnect-1.4.0.dist-info/top_level.txt,sha256=MeiZvwObGZFsa0avWx0Bg--YOWz1SZQF7PV-Q1z3OLo,16
+pyWalletConnect-1.4.0.dist-info/RECORD,,
```

