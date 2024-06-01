# Comparing `tmp/nftpy-1.1.4.tar.gz` & `tmp/nftpy-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nftpy-1.1.4.tar", max compression
+gzip compressed data, was "nftpy-1.1.5.tar", max compression
```

## Comparing `nftpy-1.1.4.tar` & `nftpy-1.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1091 2024-05-28 18:17:49.643296 nftpy-1.1.4/LICENSE
--rw-r--r--   0        0        0      269 2024-05-31 21:45:25.785865 nftpy-1.1.4/nftpy/__init__.py
--rw-r--r--   0        0        0     2669 2024-05-28 18:17:49.646297 nftpy-1.1.4/nftpy/errors.py
--rw-r--r--   0        0        0      152 2024-05-28 18:17:49.644297 nftpy-1.1.4/nftpy/EVM/__init__.py
--rw-r--r--   0        0        0    14009 2024-05-28 18:17:49.644297 nftpy-1.1.4/nftpy/EVM/abi.py
--rw-r--r--   0        0        0     7094 2024-05-31 22:32:29.791736 nftpy-1.1.4/nftpy/EVM/chains.py
--rw-r--r--   0        0        0     6253 2024-05-31 21:45:25.784864 nftpy-1.1.4/nftpy/EVM/nft.py
--rw-r--r--   0        0        0    14364 2024-05-31 22:42:24.611775 nftpy-1.1.4/nftpy/EVM/wallet.py
--rw-r--r--   0        0        0    15051 2024-05-28 18:17:49.647298 nftpy-1.1.4/nftpy/opensea.py
--rw-r--r--   0        0        0      570 2024-05-31 21:45:25.785865 nftpy-1.1.4/pyproject.toml
--rw-r--r--   0        0        0    14229 2024-05-31 22:42:24.944847 nftpy-1.1.4/README.md
--rw-r--r--   0        0        0    14552 1970-01-01 00:00:00.000000 nftpy-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-05-28 18:17:49.643296 nftpy-1.1.5/LICENSE
+-rw-r--r--   0        0        0      285 2024-06-01 05:36:12.515801 nftpy-1.1.5/nftpy/__init__.py
+-rw-r--r--   0        0        0     2669 2024-06-01 05:25:48.705907 nftpy-1.1.5/nftpy/errors.py
+-rw-r--r--   0        0        0      168 2024-06-01 05:36:12.514801 nftpy-1.1.5/nftpy/EVM/__init__.py
+-rw-r--r--   0        0        0    14009 2024-05-28 18:17:49.644297 nftpy-1.1.5/nftpy/EVM/abi.py
+-rw-r--r--   0        0        0     7094 2024-06-01 05:35:56.993423 nftpy-1.1.5/nftpy/EVM/chains.py
+-rw-r--r--   0        0        0     6253 2024-06-01 05:35:56.994424 nftpy-1.1.5/nftpy/EVM/nft.py
+-rw-r--r--   0        0        0    14387 2024-06-01 05:45:48.310250 nftpy-1.1.5/nftpy/EVM/wallet.py
+-rw-r--r--   0        0        0    15051 2024-06-01 02:59:48.543399 nftpy-1.1.5/nftpy/opensea.py
+-rw-r--r--   0        0        0      570 2024-06-01 05:36:12.515801 nftpy-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0    13725 2024-06-01 05:57:20.368338 nftpy-1.1.5/README.md
+-rw-r--r--   0        0        0    14066 1970-01-01 00:00:00.000000 nftpy-1.1.5/PKG-INFO
```

### Comparing `nftpy-1.1.4/LICENSE` & `nftpy-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.4/nftpy/errors.py` & `nftpy-1.1.5/nftpy/errors.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.4/nftpy/EVM/abi.py` & `nftpy-1.1.5/nftpy/EVM/abi.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.4/nftpy/EVM/chains.py` & `nftpy-1.1.5/nftpy/EVM/chains.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.4/nftpy/EVM/nft.py` & `nftpy-1.1.5/nftpy/EVM/nft.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.4/nftpy/EVM/wallet.py` & `nftpy-1.1.5/nftpy/EVM/wallet.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,111 +61,121 @@
             connections.append((None, conn))
 
         for thread in threads:
             thread.join()
 
         return connections
 
+    def _threaded_query(self, func, *args, **kwargs):
+        results = {}
+        threads = []
+
+        def query(chain, conn, results):
+            result = func(chain, conn, *args, **kwargs)
+            results[chain.symbol if chain else ""] = result
+
+        for chain, conn in self._connections:
+            thread = Thread(target=query, args=(chain, conn, results))
+            threads.append(thread)
+            thread.start()
+
+        for thread in threads:
+            thread.join()
+
+        return results
+
     def get_balance_wei(self, chain=None) -> dict:
         """
         Get the balance of the wallet in Wei.
 
         Args:
             chain (Chains, optional): The specific chain to get the balance from if not defined in wallet
 
         Returns:
             dict: A dictionary with the chain symbol as key and the balance as value.
         """
-        balances = {}
         if chain:
             conn = Web3(Web3.HTTPProvider(chain.rpc_url))
             if conn.is_connected():
                 balance = conn.eth.get_balance(self._address)
-                balances[chain.symbol] = balance
+                return {chain.symbol: balance}
             else:
                 raise InvalidRPCURL(chain.rpc_url, chain.name)
         else:
-            for chain, conn in self._connections:
-                symbol = chain.symbol if chain else "Balance"
-                balance = conn.eth.get_balance(self._address)
-                balances[symbol] = balance
-        return balances
+            def get_balance(chain, conn):
+                return conn.eth.get_balance(self._address)
+            return self._threaded_query(get_balance)
 
     def get_balance(self, chain=None) -> dict:
         """
         Get the balance of the wallet in Ether.
 
         Args:
             chain (Chains, optional): The specific chain to get the balance from if not defined in wallet
 
         Returns:
             dict: A dictionary with the chain symbol as key and the balance as value.
         """
-        balances = {}
         if chain:
             conn = Web3(Web3.HTTPProvider(chain.rpc_url))
             if conn.is_connected():
                 balance = conn.eth.get_balance(self._address)
-                balances[chain.symbol] = Web3.from_wei(balance, 'ether')
+                return {chain.symbol: Web3.from_wei(balance, 'ether')}
             else:
                 raise InvalidRPCURL(chain.rpc_url, chain.name)
         else:
-            for chain, conn in self._connections:
-                symbol = chain.symbol if chain else "Balance"
+            def get_balance(chain, conn):
                 balance = conn.eth.get_balance(self._address)
-                balances[symbol] = Web3.from_wei(balance, 'ether')
-        return {"Balances": balances}
+                return Web3.from_wei(balance, 'ether')
+            return {"Balances": self._threaded_query(get_balance)}
 
     def get_gas_price_wei(self, chain=None) -> dict:
         """
         Get the current gas price in Wei.
 
         Args:
             chain (Chains, optional): The specific chain to get the gas price from.
 
         Returns:
             dict: A dictionary with the chain symbol as key and the gas price as value.
         """
-        gas_prices = {}
         if chain:
             conn = Web3(Web3.HTTPProvider(chain.rpc_url))
             if conn.is_connected():
                 gas_price = conn.eth.gas_price
-                gas_prices[chain.symbol] = gas_price
+                return {chain.symbol: gas_price}
             else:
                 raise InvalidRPCURL(chain.rpc_url, chain.name)
         else:
-            for chain, conn in self._connections:
-                gas_price = conn.eth.gas_price
-                gas_prices[chain.symbol] = gas_price
-        return gas_prices
+            def get_gas_price(chain, conn):
+                return conn.eth.gas_price
+            return self._threaded_query(get_gas_price)
 
     def get_gas_price_gwei(self, chain=None) -> dict:
         """
         Get the current gas price in Gwei.
 
         Args:
             chain (Chains, optional): The specific chain to get the gas price from.
 
         Returns:
             dict: A dictionary with the chain symbol as key and the gas price as value.
         """
-        gas_prices = {}
         if chain:
             conn = Web3(Web3.HTTPProvider(chain.rpc_url))
             if conn.is_connected():
                 gas_price = conn.eth.gas_price
-                gas_prices[chain.symbol] = Web3.from_wei(gas_price, 'gwei')
+                return {chain.symbol: Web3.from_wei(gas_price, 'gwei')}
             else:
                 raise InvalidRPCURL(chain.rpc_url, chain.name)
         else:
-            for chain, conn in self._connections:
+            def get_gas_price(chain, conn):
                 gas_price = conn.eth.gas_price
-                gas_prices[chain.symbol] = Web3.from_wei(gas_price, 'gwei')
-        return gas_prices
+                return Web3.from_wei(gas_price, 'gwei')
+            return self._threaded_query(get_gas_price)
 
     def transfer_nft(self, to: str, contract_address: str, amount: int, gas_limit: int, gas_price_gwei: int = None,
                      gas_price_wei: int = None, abi: ABI = None, abi_str: str = None,
                      chain = None, token_id: int = None) -> dict:
         """
         Transfer an NFT to another wallet.
 
@@ -275,95 +285,87 @@
 
         Args:
             chain (Chains, optional): The specific chain to get the transaction count from.
 
         Returns:
             dict: A dictionary with the chain symbol as key and the transaction count as value.
         """
-        counts = {}
         if chain:
             conn = Web3(Web3.HTTPProvider(chain.rpc_url))
             if conn.is_connected():
                 count = conn.eth.get_transaction_count(self._address)
-                counts[chain.symbol] = count
+                return {chain.symbol: count}
             else:
                 raise InvalidRPCURL(chain.rpc_url, chain.name)
         else:
-            for chain, conn in self._connections:
-                count = conn.eth.get_transaction_count(self._address)
-                counts[chain.symbol] = count
-        return counts
+            def get_count(chain, conn):
+                return conn.eth.get_transaction_count(self._address)
+            return self._threaded_query(get_count)
 
     def estimate_gas(self, to: str, value: int, data: bytes = b'', chain=None) -> dict:
         """
         Estimate the gas required for a transaction.
 
         Args:
             to (str): The recipient address.
             value (int): The value to send in Wei.
             data (bytes, optional): The data to include in the transaction.
             chain (Chains, optional): The specific chain to estimate the gas on.
 
         Returns:
             dict: A dictionary with the chain symbol as key and the gas estimate as value.
         """
-        estimates = {}
         if chain:
             conn = Web3(Web3.HTTPProvider(chain.rpc_url))
             if conn.is_connected():
                 estimate = conn.eth.estimate_gas({'to': to, 'value': value, 'data': data})
-                estimates[chain.symbol] = estimate
+                return {chain.symbol: estimate}
             else:
                 raise InvalidRPCURL(chain.rpc_url, chain.name)
         else:
-            for chain, conn in self._connections:
-                estimate = conn.eth.estimate_gas({'to': to, 'value': value, 'data': data})
-                estimates[chain.symbol] = estimate
-        return estimates
+            def estimate_gas(chain, conn):
+                return conn.eth.estimate_gas({'to': to, 'value': value, 'data': data})
+            return self._threaded_query(estimate_gas)
 
     def is_synced(self, chain=None) -> dict:
         """
         Check if the blockchain is synced for RPC debugging!
 
         Args:
             chain (Chains, optional): The specific chain to check the sync status on.
 
         Returns:
             dict: A dictionary with the chain symbol as key and the sync status as value.
         """
-        sync_status = {}
         if chain:
             conn = Web3(Web3.HTTPProvider(chain.rpc_url))
             if conn.is_connected():
                 synced = not conn.eth.syncing
-                sync_status[chain.symbol] = synced
+                return {chain.symbol: synced}
             else:
                 raise InvalidRPCURL(chain.rpc_url, chain.name)
         else:
-            for chain, conn in self._connections:
-                synced = not conn.eth.syncing
-                sync_status[chain.symbol] = synced
-        return sync_status
+            def check_sync(chain, conn):
+                return not conn.eth.syncing
+            return self._threaded_query(check_sync)
 
     def get_latest_block(self, chain=None) -> dict:
         """
         Get the latest block details.
 
         Args:
             chain (Chains, optional): The specific chain to get the latest block from.
 
         Returns:
             dict: A dictionary with the chain symbol as key and the latest block details as value.
         """
-        blocks = {}
         if chain:
             conn = Web3(Web3.HTTPProvider(chain.rpc_url))
             if conn.is_connected():
                 block = conn.eth.get_block('latest')
-                blocks[chain.symbol] = block
+                return {chain.symbol: block}
             else:
                 raise InvalidRPCURL(chain.rpc_url, chain.name)
         else:
-            for chain, conn in self._connections:
-                block = conn.eth.get_block('latest')
-                blocks[chain.symbol] = block
-        return blocks
+            def get_block(chain, conn):
+                return conn.eth.get_block('latest')
+            return self._threaded_query(get_block)
```

### Comparing `nftpy-1.1.4/nftpy/opensea.py` & `nftpy-1.1.5/nftpy/opensea.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.4/pyproject.toml` & `nftpy-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nftpy"
-version = "1.1.4"
+version = "1.1.5"
 description = "A NFT specific Python library for easy NFT integration in Python"
 authors = ["CoulterStutz <coultercash@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/coulterstutz/nftpy"
 repository = "https://github.com/coulterstutz/nftpy"
```

### Comparing `nftpy-1.1.4/README.md` & `nftpy-1.1.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,16 @@
 # nftpy
-[![PyPi](https://img.shields.io/badge/PyPi-1.1.4-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/nftpy/)](https://pypi.org/project/nftpy/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.1.5-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/nftpy/)](https://pypi.org/project/nftpy/)
 [![Python](https://img.shields.io/badge/Python-3.7,%203.8,%203.9,%203.10,%203.11,%203.12-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/nftpy/)](https://pypi.org/project/nftpy/)
 
 A Python package designed to facilitate the integration and adoption of NFT (ERC721, ERC1155) tokens in software applications.
 
-### Changes in 1.1.4
-###### Added EVM Chain Support for these testnets:
-- Holesky Testnet (ETH)
-- BSC Testnet (BSC)
-- Mumbai Testnet (MATIC)
-- Goerli Testnet (ARB)
-- Goerli Testnet (OPTIMISM)
-- Fuji Testnet (AVAX)
-- Fantom Testnet (FTM)
-- Alfajores Testnet (CELO)
-- Baklava Testnet (CELO)
-- Cronos Testnet (CRONOS)
-
-###### Fixed Custom Chain Assignment
-- Custom Chains are now assigned in a class not the Chains:Enum class. 
-- NFTWallet and  other EVM instances now no longer require a block explorer argument for custom chains.
-
-###### Optimizations
-- Wallet now returns using the chain symbol instead of the chain name
-- Wallet now uses threading to connect to multiple chains
-
+### Changes in 1.1.5
+#### Threaded NFTWallet class for fast chain querying!
+If you are querying to multiple chains at once, fear no more as processing times are slashed for multichain querying!
 ## Features
 
 #### EVM Interaction with NFT Tokens
 ![Ethereum](https://img.shields.io/badge/Ethereum%20Based%20Networks-3C3C3D?style=for-the-badge&logo=Ethereum&logoColor=white)
 
 nftpy enables interaction with the Ethereum Virtual Machine (EVM) through RPC to retrieve contract details and token holders. It provides a direct communication pathway between the client and the blockchain. Currently, transactional methods are not supported but will be implemented in future updates. The following methods are available:
```

### Comparing `nftpy-1.1.4/PKG-INFO` & `nftpy-1.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nftpy
-Version: 1.1.4
+Version: 1.1.5
 Summary: A NFT specific Python library for easy NFT integration in Python
 Home-page: https://github.com/coulterstutz/nftpy
 License: MIT
 Author: CoulterStutz
 Author-email: coultercash@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,40 +12,22 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: web3 (>=6.2.0,<7.0.0)
 Project-URL: Repository, https://github.com/coulterstutz/nftpy
 Description-Content-Type: text/markdown
 
 # nftpy
-[![PyPi](https://img.shields.io/badge/PyPi-1.1.4-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/nftpy/)](https://pypi.org/project/nftpy/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.1.5-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/nftpy/)](https://pypi.org/project/nftpy/)
 [![Python](https://img.shields.io/badge/Python-3.7,%203.8,%203.9,%203.10,%203.11,%203.12-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/nftpy/)](https://pypi.org/project/nftpy/)
 
 A Python package designed to facilitate the integration and adoption of NFT (ERC721, ERC1155) tokens in software applications.
 
-### Changes in 1.1.4
-###### Added EVM Chain Support for these testnets:
-- Holesky Testnet (ETH)
-- BSC Testnet (BSC)
-- Mumbai Testnet (MATIC)
-- Goerli Testnet (ARB)
-- Goerli Testnet (OPTIMISM)
-- Fuji Testnet (AVAX)
-- Fantom Testnet (FTM)
-- Alfajores Testnet (CELO)
-- Baklava Testnet (CELO)
-- Cronos Testnet (CRONOS)
-
-###### Fixed Custom Chain Assignment
-- Custom Chains are now assigned in a class not the Chains:Enum class. 
-- NFTWallet and  other EVM instances now no longer require a block explorer argument for custom chains.
-
-###### Optimizations
-- Wallet now returns using the chain symbol instead of the chain name
-- Wallet now uses threading to connect to multiple chains
-
+### Changes in 1.1.5
+#### Threaded NFTWallet class for fast chain querying!
+If you are querying to multiple chains at once, fear no more as processing times are slashed for multichain querying!
 ## Features
 
 #### EVM Interaction with NFT Tokens
 ![Ethereum](https://img.shields.io/badge/Ethereum%20Based%20Networks-3C3C3D?style=for-the-badge&logo=Ethereum&logoColor=white)
 
 nftpy enables interaction with the Ethereum Virtual Machine (EVM) through RPC to retrieve contract details and token holders. It provides a direct communication pathway between the client and the blockchain. Currently, transactional methods are not supported but will be implemented in future updates. The following methods are available:
```

