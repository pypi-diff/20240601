# Comparing `tmp/nftpy-1.1.3.tar.gz` & `tmp/nftpy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nftpy-1.1.3.tar", max compression
+gzip compressed data, was "nftpy-1.1.4.tar", max compression
```

## Comparing `nftpy-1.1.3.tar` & `nftpy-1.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1091 2024-05-28 18:17:49.643296 nftpy-1.1.3/LICENSE
--rw-r--r--   0        0        0      269 2024-05-29 05:22:35.638204 nftpy-1.1.3/nftpy/__init__.py
--rw-r--r--   0        0        0     2669 2024-05-28 18:17:49.646297 nftpy-1.1.3/nftpy/errors.py
--rw-r--r--   0        0        0      152 2024-05-28 18:17:49.644297 nftpy-1.1.3/nftpy/EVM/__init__.py
--rw-r--r--   0        0        0    14009 2024-05-28 18:17:49.644297 nftpy-1.1.3/nftpy/EVM/abi.py
--rw-r--r--   0        0        0     3873 2024-05-29 05:22:35.638204 nftpy-1.1.3/nftpy/EVM/chains.py
--rw-r--r--   0        0        0     6286 2024-05-28 18:17:49.645297 nftpy-1.1.3/nftpy/EVM/nft.py
--rw-r--r--   0        0        0    14109 2024-05-28 18:17:49.645297 nftpy-1.1.3/nftpy/EVM/wallet.py
--rw-r--r--   0        0        0    15051 2024-05-28 18:17:49.647298 nftpy-1.1.3/nftpy/opensea.py
--rw-r--r--   0        0        0      570 2024-05-29 05:22:35.639204 nftpy-1.1.3/pyproject.toml
--rw-r--r--   0        0        0    14092 2024-05-29 05:22:35.637203 nftpy-1.1.3/README.md
--rw-r--r--   0        0        0    14419 1970-01-01 00:00:00.000000 nftpy-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-05-28 18:17:49.643296 nftpy-1.1.4/LICENSE
+-rw-r--r--   0        0        0      269 2024-05-31 21:45:25.785865 nftpy-1.1.4/nftpy/__init__.py
+-rw-r--r--   0        0        0     2669 2024-05-28 18:17:49.646297 nftpy-1.1.4/nftpy/errors.py
+-rw-r--r--   0        0        0      152 2024-05-28 18:17:49.644297 nftpy-1.1.4/nftpy/EVM/__init__.py
+-rw-r--r--   0        0        0    14009 2024-05-28 18:17:49.644297 nftpy-1.1.4/nftpy/EVM/abi.py
+-rw-r--r--   0        0        0     7094 2024-05-31 22:32:29.791736 nftpy-1.1.4/nftpy/EVM/chains.py
+-rw-r--r--   0        0        0     6253 2024-05-31 21:45:25.784864 nftpy-1.1.4/nftpy/EVM/nft.py
+-rw-r--r--   0        0        0    14364 2024-05-31 22:42:24.611775 nftpy-1.1.4/nftpy/EVM/wallet.py
+-rw-r--r--   0        0        0    15051 2024-05-28 18:17:49.647298 nftpy-1.1.4/nftpy/opensea.py
+-rw-r--r--   0        0        0      570 2024-05-31 21:45:25.785865 nftpy-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0    14229 2024-05-31 22:42:24.944847 nftpy-1.1.4/README.md
+-rw-r--r--   0        0        0    14552 1970-01-01 00:00:00.000000 nftpy-1.1.4/PKG-INFO
```

### Comparing `nftpy-1.1.3/LICENSE` & `nftpy-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.3/nftpy/errors.py` & `nftpy-1.1.4/nftpy/errors.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.3/nftpy/EVM/abi.py` & `nftpy-1.1.4/nftpy/EVM/abi.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.3/nftpy/EVM/nft.py` & `nftpy-1.1.4/nftpy/EVM/nft.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import json
 import requests
 from .chains import Chains
 from .abi import ABI
-from enum import Enum
 from web3 import Web3
 from ..errors import *
 
 
 class NFT:
-    def __init__(self, contract_address: str, network: Chains = Chains.ETH, rpc_url: str = None, abi: ABI = ABI.ERC721):
+    def __init__(self, contract_address: str, network=Chains.ETH, rpc_url: str = None, abi: ABI = ABI.ERC721):
         """
         Creates an Object Interface for interaction with a contract on chain
 
         Args:
             contract_address (str): The address of the NFT contract.
             network (Chains): The blockchain network on which the contract is deployed (ex. Chains.ETH).
             rpc_url (str): Optional custom RPC URL. If not provided, the default URL for the network will be used.
```

### Comparing `nftpy-1.1.3/nftpy/EVM/wallet.py` & `nftpy-1.1.4/nftpy/EVM/wallet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,168 +1,175 @@
 import time
-
+from threading import Thread
 from web3 import Web3
 from web3.exceptions import TransactionNotFound
-
 from .abi import ABI
 from .chains import Chains
 from ..errors import *
 
 class NFTWallet:
     """
     A class to interact with NFTs on various EVM Based networks from a wallet.
 
     Args:
         private_key (str, optional): The private key of the wallet for full access.
         address (str, optional): The address of the wallet for read-only access.
         chains (list[Chains], optional): A list of blockchain networks to connect to.
         rpc_url (str, optional): Custom RPC URL to connect to.
     """
-    def __init__(self, private_key: str = None, address: str = None, chains: list[Chains] = None, rpc_url: str = None):
+    def __init__(self, private_key: str = None, address: str = None, chains: list = None, rpc_url: str = None):
         if not private_key and not address:
             raise NoCredentialsProvidedError()
         self._private_key = private_key
         self._address = address or self._get_address_from_private_key()
         self.chains = chains or []
         self._rpc_url = rpc_url
         self._connections = self._connect_to_chains()
 
     def _get_address_from_private_key(self):
         account = Web3().eth.account.from_key(self._private_key)
         return account.address
 
     def _connect_to_chains(self):
+        def connect(chain, connections):
+            conn = Web3(Web3.HTTPProvider(chain.rpc_url))
+            if not conn.is_connected():
+                raise InvalidRPCURL(chain.rpc_url, chain.name)
+            connections.append((chain, conn))
+
         connections = []
+        threads = []
+
         if not self.chains and not self._rpc_url:
             for chain in Chains:
-                conn = Web3(Web3.HTTPProvider(chain.rpc_url))
-                if not conn.is_connected():
-                    raise InvalidRPCURL(chain.rpc_url, chain.name)
-                connections.append((chain, conn))
+                thread = Thread(target=connect, args=(chain, connections))
+                threads.append(thread)
+                thread.start()
         elif self.chains and not self._rpc_url:
             for chain in self.chains:
-                conn = Web3(Web3.HTTPProvider(chain.rpc_url))
-                if not conn.is_connected():
-                    raise InvalidRPCURL(chain.rpc_url, chain.name)
-                connections.append((chain, conn))
+                thread = Thread(target=connect, args=(chain, connections))
+                threads.append(thread)
+                thread.start()
         elif self.chains and self._rpc_url:
             for chain in self.chains:
-                conn = Web3(Web3.HTTPProvider(self._rpc_url))
-                if not conn.is_connected():
-                    raise InvalidRPCURL(self._rpc_url, chain.name)
-                connections.append((chain, conn))
+                thread = Thread(target=connect, args=(chain, connections))
+                threads.append(thread)
+                thread.start()
         elif not self.chains and self._rpc_url:
             conn = Web3(Web3.HTTPProvider(self._rpc_url))
             if not conn.is_connected():
                 raise InvalidRPCURL(self._rpc_url)
             connections.append((None, conn))
+
+        for thread in threads:
+            thread.join()
+
         return connections
 
-    def get_balance_wei(self, chain: Chains = None) -> dict:
+    def get_balance_wei(self, chain=None) -> dict:
         """
         Get the balance of the wallet in Wei.
 
         Args:
             chain (Chains, optional): The specific chain to get the balance from if not defined in wallet
 
         Returns:
-            dict: A dictionary with the chain name as key and the balance as value.
+            dict: A dictionary with the chain symbol as key and the balance as value.
         """
         balances = {}
         if chain:
             conn = Web3(Web3.HTTPProvider(chain.rpc_url))
             if conn.is_connected():
                 balance = conn.eth.get_balance(self._address)
-                balances[chain.name] = balance
+                balances[chain.symbol] = balance
             else:
                 raise InvalidRPCURL(chain.rpc_url, chain.name)
         else:
             for chain, conn in self._connections:
-                symbol = chain.name if chain else "Balance"
+                symbol = chain.symbol if chain else "Balance"
                 balance = conn.eth.get_balance(self._address)
                 balances[symbol] = balance
         return balances
 
-    def get_balance(self, chain: Chains = None) -> dict:
+    def get_balance(self, chain=None) -> dict:
         """
         Get the balance of the wallet in Ether.
 
         Args:
             chain (Chains, optional): The specific chain to get the balance from if not defined in wallet
 
         Returns:
-            dict: A dictionary with the chain name as key and the balance as value.
+            dict: A dictionary with the chain symbol as key and the balance as value.
         """
         balances = {}
         if chain:
             conn = Web3(Web3.HTTPProvider(chain.rpc_url))
             if conn.is_connected():
                 balance = conn.eth.get_balance(self._address)
-                balances[chain.name] = Web3.from_wei(balance, 'ether')
+                balances[chain.symbol] = Web3.from_wei(balance, 'ether')
             else:
                 raise InvalidRPCURL(chain.rpc_url, chain.name)
         else:
             for chain, conn in self._connections:
-                symbol = chain.name if chain else "Balance"
+                symbol = chain.symbol if chain else "Balance"
                 balance = conn.eth.get_balance(self._address)
                 balances[symbol] = Web3.from_wei(balance, 'ether')
         return {"Balances": balances}
 
-    def get_gas_price_wei(self, chain: Chains = None) -> dict:
+    def get_gas_price_wei(self, chain=None) -> dict:
         """
         Get the current gas price in Wei.
 
         Args:
             chain (Chains, optional): The specific chain to get the gas price from.
 
         Returns:
-            dict: A dictionary with the chain name as key and the gas price as value.
+            dict: A dictionary with the chain symbol as key and the gas price as value.
         """
         gas_prices = {}
         if chain:
             conn = Web3(Web3.HTTPProvider(chain.rpc_url))
             if conn.is_connected():
                 gas_price = conn.eth.gas_price
-                gas_prices[chain.name] = gas_price
+                gas_prices[chain.symbol] = gas_price
             else:
                 raise InvalidRPCURL(chain.rpc_url, chain.name)
         else:
             for chain, conn in self._connections:
                 gas_price = conn.eth.gas_price
-                gas_prices[chain.name] = gas_price
+                gas_prices[chain.symbol] = gas_price
         return gas_prices
 
-    def get_gas_price_gwei(self, chain: Chains = None) -> dict:
+    def get_gas_price_gwei(self, chain=None) -> dict:
         """
         Get the current gas price in Gwei.
 
         Args:
             chain (Chains, optional): The specific chain to get the gas price from.
 
         Returns:
-            dict: A dictionary with the chain name as key and the gas price as value.
+            dict: A dictionary with the chain symbol as key and the gas price as value.
         """
-
         gas_prices = {}
         if chain:
             conn = Web3(Web3.HTTPProvider(chain.rpc_url))
             if conn.is_connected():
                 gas_price = conn.eth.gas_price
-                gas_prices[chain.name] = Web3.from_wei(gas_price, 'gwei')
+                gas_prices[chain.symbol] = Web3.from_wei(gas_price, 'gwei')
             else:
                 raise InvalidRPCURL(chain.rpc_url, chain.name)
         else:
             for chain, conn in self._connections:
                 gas_price = conn.eth.gas_price
-                gas_prices[chain.name] = Web3.from_wei(gas_price, 'gwei')
+                gas_prices[chain.symbol] = Web3.from_wei(gas_price, 'gwei')
         return gas_prices
 
     def transfer_nft(self, to: str, contract_address: str, amount: int, gas_limit: int, gas_price_gwei: int = None,
                      gas_price_wei: int = None, abi: ABI = None, abi_str: str = None,
-                     chain: Chains = None, token_id: int = None) -> dict:
+                     chain = None, token_id: int = None) -> dict:
         """
         Transfer an NFT to another wallet.
 
         Args:
             to (str): The recipient wallet address.
             contract_address (str): The contract address of the NFT.
             amount (int): The amount of NFTs to transfer.
@@ -214,27 +221,32 @@
             })['data'],
         }
 
         signed_tx = conn.eth.account.sign_transaction(tx, private_key=self._private_key)
 
         try:
             tx_hash = conn.eth.send_raw_transaction(signed_tx.rawTransaction)
-            return {
-                'transaction_hash': tx_hash.hex(),
-                'explorer_url': f"{chain.explorer_url}/tx/{tx_hash.hex()}"
-            }
+            if chain.explorer_url != None:
+                return {
+                    'transaction_hash': tx_hash.hex(),
+                    'explorer_url': f"{chain.explorer_url}/tx/{tx_hash.hex()}"
+                }
+            else:
+                return {
+                    'transaction_hash': tx_hash.hex(),
+                }
         except ValueError as e:
             if 'gas' in str(e):
                 raise TransactionGasError()
             elif 'balance' in str(e):
                 raise TransactionBalanceError()
             else:
                 raise e
 
-    def wait_until_transaction_processes(self, tx_hash, chain: Chains) -> bool:
+    def wait_until_transaction_processes(self, tx_hash, chain) -> bool:
         """
         Wait until a transaction is processed.
 
         Args:
             tx_hash (str or bytes): The transaction hash.
             chain (Chains): The specific chain to check the transaction on.
 
@@ -253,105 +265,105 @@
                 receipt = conn.eth.get_transaction_receipt(tx_hash)
                 if receipt is not None and receipt.status == 1:
                     return True
             except TransactionNotFound:
                 pass
             time.sleep(1)
 
-    def get_transaction_count(self, chain: Chains = None) -> dict:
+    def get_transaction_count(self, chain=None) -> dict:
         """
         Get the number of transactions sent from the address.
 
         Args:
             chain (Chains, optional): The specific chain to get the transaction count from.
 
         Returns:
-            dict: A dictionary with the chain name as key and the transaction count as value.
+            dict: A dictionary with the chain symbol as key and the transaction count as value.
         """
         counts = {}
         if chain:
             conn = Web3(Web3.HTTPProvider(chain.rpc_url))
             if conn.is_connected():
                 count = conn.eth.get_transaction_count(self._address)
-                counts[chain.name] = count
+                counts[chain.symbol] = count
             else:
                 raise InvalidRPCURL(chain.rpc_url, chain.name)
         else:
             for chain, conn in self._connections:
                 count = conn.eth.get_transaction_count(self._address)
-                counts[chain.name] = count
+                counts[chain.symbol] = count
         return counts
 
-    def estimate_gas(self, to: str, value: int, data: bytes = b'', chain: Chains = None) -> dict:
+    def estimate_gas(self, to: str, value: int, data: bytes = b'', chain=None) -> dict:
         """
         Estimate the gas required for a transaction.
 
         Args:
             to (str): The recipient address.
             value (int): The value to send in Wei.
             data (bytes, optional): The data to include in the transaction.
             chain (Chains, optional): The specific chain to estimate the gas on.
 
         Returns:
-            dict: A dictionary with the chain name as key and the gas estimate as value.
+            dict: A dictionary with the chain symbol as key and the gas estimate as value.
         """
         estimates = {}
         if chain:
             conn = Web3(Web3.HTTPProvider(chain.rpc_url))
             if conn.is_connected():
                 estimate = conn.eth.estimate_gas({'to': to, 'value': value, 'data': data})
-                estimates[chain.name] = estimate
+                estimates[chain.symbol] = estimate
             else:
                 raise InvalidRPCURL(chain.rpc_url, chain.name)
         else:
             for chain, conn in self._connections:
                 estimate = conn.eth.estimate_gas({'to': to, 'value': value, 'data': data})
-                estimates[chain.name] = estimate
+                estimates[chain.symbol] = estimate
         return estimates
 
-    def is_synced(self, chain: Chains = None) -> dict:
+    def is_synced(self, chain=None) -> dict:
         """
         Check if the blockchain is synced for RPC debugging!
 
         Args:
             chain (Chains, optional): The specific chain to check the sync status on.
 
         Returns:
-            dict: A dictionary with the chain name as key and the sync status as value.
+            dict: A dictionary with the chain symbol as key and the sync status as value.
         """
         sync_status = {}
         if chain:
             conn = Web3(Web3.HTTPProvider(chain.rpc_url))
             if conn.is_connected():
                 synced = not conn.eth.syncing
-                sync_status[chain.name] = synced
+                sync_status[chain.symbol] = synced
             else:
                 raise InvalidRPCURL(chain.rpc_url, chain.name)
         else:
             for chain, conn in self._connections:
                 synced = not conn.eth.syncing
-                sync_status[chain.name] = synced
+                sync_status[chain.symbol] = synced
         return sync_status
 
-    def get_latest_block(self, chain: Chains = None) -> dict:
+    def get_latest_block(self, chain=None) -> dict:
         """
         Get the latest block details.
 
         Args:
             chain (Chains, optional): The specific chain to get the latest block from.
 
         Returns:
-            dict: A dictionary with the chain name as key and the latest block details as value.
+            dict: A dictionary with the chain symbol as key and the latest block details as value.
         """
         blocks = {}
         if chain:
             conn = Web3(Web3.HTTPProvider(chain.rpc_url))
             if conn.is_connected():
                 block = conn.eth.get_block('latest')
-                blocks[chain.name] = block
+                blocks[chain.symbol] = block
             else:
                 raise InvalidRPCURL(chain.rpc_url, chain.name)
         else:
             for chain, conn in self._connections:
                 block = conn.eth.get_block('latest')
-                blocks[chain.name] = block
-        return blocks
+                blocks[chain.symbol] = block
+        return blocks
```

### Comparing `nftpy-1.1.3/nftpy/opensea.py` & `nftpy-1.1.4/nftpy/opensea.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.3/pyproject.toml` & `nftpy-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nftpy"
-version = "1.1.3"
+version = "1.1.4"
 description = "A NFT specific Python library for easy NFT integration in Python"
 authors = ["CoulterStutz <coultercash@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/coulterstutz/nftpy"
 repository = "https://github.com/coulterstutz/nftpy"
```

### Comparing `nftpy-1.1.3/README.md` & `nftpy-1.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,53 @@
-# NFTPy
-[![PyPi](https://img.shields.io/badge/PyPi-1.1.3-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/NFTPy/)](https://pypi.org/project/NFTPy/)
-[![Python](https://img.shields.io/badge/Python-3.7,%203.8,%203.9,%203.10,%203.11,%203.12-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/NFTPy/)](https://pypi.org/project/NFTPy/)
+# nftpy
+[![PyPi](https://img.shields.io/badge/PyPi-1.1.4-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/nftpy/)](https://pypi.org/project/nftpy/)
+[![Python](https://img.shields.io/badge/Python-3.7,%203.8,%203.9,%203.10,%203.11,%203.12-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/nftpy/)](https://pypi.org/project/nftpy/)
 
 A Python package designed to facilitate the integration and adoption of NFT (ERC721, ERC1155) tokens in software applications.
 
+### Changes in 1.1.4
+###### Added EVM Chain Support for these testnets:
+- Holesky Testnet (ETH)
+- BSC Testnet (BSC)
+- Mumbai Testnet (MATIC)
+- Goerli Testnet (ARB)
+- Goerli Testnet (OPTIMISM)
+- Fuji Testnet (AVAX)
+- Fantom Testnet (FTM)
+- Alfajores Testnet (CELO)
+- Baklava Testnet (CELO)
+- Cronos Testnet (CRONOS)
+
+###### Fixed Custom Chain Assignment
+- Custom Chains are now assigned in a class not the Chains:Enum class. 
+- NFTWallet and  other EVM instances now no longer require a block explorer argument for custom chains.
+
+###### Optimizations
+- Wallet now returns using the chain symbol instead of the chain name
+- Wallet now uses threading to connect to multiple chains
+
 ## Features
 
 #### EVM Interaction with NFT Tokens
 ![Ethereum](https://img.shields.io/badge/Ethereum%20Based%20Networks-3C3C3D?style=for-the-badge&logo=Ethereum&logoColor=white)
 
-NFTPy enables interaction with the Ethereum Virtual Machine (EVM) through RPC to retrieve contract details and token holders. It provides a direct communication pathway between the client and the blockchain. Currently, transactional methods are not supported but will be implemented in future updates. The following methods are available:
+nftpy enables interaction with the Ethereum Virtual Machine (EVM) through RPC to retrieve contract details and token holders. It provides a direct communication pathway between the client and the blockchain. Currently, transactional methods are not supported but will be implemented in future updates. The following methods are available:
 
 - **get_balance**: Retrieve the balance of NFTs for a given address.
 - **get_token_uri**: Fetch the metadata URI of a specific token.
 - **get_owner**: Determine the owner of a specific token.
 - **get_approved**: Get the approved address for a specific ERC721 token.
 - **is_approved_for_all**: Check if an address is approved for all tokens owned by another address (ERC721).
 - **get_token_metadata**: Get the metadata for a specific ERC721 token.
 - **get_token_balance**: Get the balance of a specific ERC1155 token for a specific wallet address.
 - **get_tokens_balance**: Gets the balance of a specific list of tokens.
 - **is_approved_for_all_erc1155**: Check if an address is approved for all tokens owned by another address (ERC1155).
 
 #### EVM Wallet Interaction
-NFTPy includes comprehensive features for interacting with Ethereum wallets, including querying balances, fetching gas prices, and transferring NFTs. The wallet interface supports both read-only and transactional operations.
+nftpy includes comprehensive features for interacting with Ethereum wallets, including querying balances, fetching gas prices, and transferring NFTs. The wallet interface supports both read-only and transactional operations.
 
 **Wallet Features:**
 - **get_balance**: Retrieve the balance of NFTs for a given address in Ether.
 - **get_balance_wei**: Retrieve the balance of NFTs for a given address in Wei.
 - **get_gas_price_wei**: Fetch the current gas price in Wei.
 - **get_gas_price_gwei**: Fetch the current gas price in Gwei.
 - **transfer_nft**: Transfer an NFT from the wallet to another address.
@@ -35,61 +56,56 @@
 - **estimate_gas**: Estimate the gas required for a transaction.
 - **is_synced**: Check if the blockchain is synced.
 - **get_latest_block**: Get the latest block on the blockchain.
 
 #### Built-in OpenSea Interface
 ![OpenSea Support](https://img.shields.io/badge/OpenSea-%232081E2.svg?style=for-the-badge&logo=opensea&logoColor=white)
 
-NFTPy includes a built-in interface for interacting with OpenSea via an API key. This allows for in-package queries to OpenSea, enabling access to pricing information and other OpenSea-specific data. The OpenSea interface can be configured to focus on a single collection or query multiple collections. The available methods include:
+nftpy includes a built-in interface for interacting with OpenSea via an API key. This allows for in-package queries to OpenSea, enabling access to pricing information and other OpenSea-specific data. The OpenSea interface can be configured to focus on a single collection or query multiple collections. The available methods include:
 
 - **get_collection_stats**: Obtain statistics for a collection.
 - **list_events_by_nft**: List events related to a specific NFT.
 - **get_collection**: Fetch details of a specific collection.
 - **get_contract**: Retrieve details of a specific contract.
 - **get_nft**: Get details of a specific NFT.
 - **list_nfts_by_account**: List NFTs owned by a specific account.
 - **list_nfts_by_collection**: List NFTs in a specific collection.
 - **list_nfts_by_contract**: List NFTs under a specific contract.
 - **get_payment_token**: Get details of a specific payment token.
 - **get_traits**: Get traits of a specific collection.
 - **get_all_listings_on_collection**: Get all listings of a specific collection.
 
 #### Custom Chain Support
-NFTPy allows the creation of custom chains with specific chain IDs, RPC URLs, explorer URLs, and names. This feature enhances flexibility by enabling the addition of blockchain networks that are not predefined in the library.
+nftpy allows the creation of custom chains with specific chain IDs, RPC URLs, explorer URLs, and names. This feature enhances flexibility by enabling the addition of blockchain networks that are not predefined in the library.
 
 **Creating a Custom Chain:**
 ```python
-from NFTPy.EVM import Chains
+from nftpy.EVM import Chain
 
-# Create a custom chain
-custom_chain = Chains.custom_chain(
-    chain_id=999,
-    rpc_url="https://custom-rpc-url.com",
-    explorer_url="https://custom-explorer.com",
-    name="Custom Blockchain"
+custom_chain = Chain(
+        name = "Ethereum",
+        symbol = "ETH",
+        chain_id = 1,
+        rpc_url = "https://eth.llamarpc.com",
+        explorer_url = "https://etherscan.io",
+        testnet = False
 )
-
-# Access custom chain attributes
-print(custom_chain.chain_id)       # Outputs: 999
-print(custom_chain.rpc_url)        # Outputs: https://custom-rpc-url.com
-print(custom_chain.explorer_url)   # Outputs: https://custom-explorer.com
-print(custom_chain.name)           # Outputs: Custom Blockchain
 ```
 
 # Example Usage
-### Interacting on-chain with a collection | NFTPy.EVM.NFT
-Using NFTPy.EVM.NFT we are going to be querying the Pixelmon NFT collection on Ethereum mainnet!
+### Interacting on-chain with a collection | nftpy.EVM.NFT
+Using nftpy.EVM.NFT we are going to be querying the Pixelmon NFT collection on Ethereum mainnet!
 We will first start off by creating our class. We are going to define our class with three arguments:
 - contract_address: The address of the contract you are trying to query.
 - abi: The ABI of the contract you are trying to query. The EVM.ABI class provides presets for our ABI. You can also paste an ABI into the field.
 - network: This dictates what RPC URL to use and sets a preset that works best with the network.
 - rpc_url: If you do not want to use a preset and instead want to use a custom RPC, define it using this field.
 
 ```python
-import NFTPy.EVM as EVM
+import nftpy.EVM as EVM
 Pixelmon = EVM.NFT("0x32973908FaeE0Bf825A343000fE412ebE56F802A", abi=EVM.ABI.ERC721, network=EVM.Chains.ETH)
 #                   Contract Address                                ABI              Network To Query (Ethereum)
 ```
 Now that we have created our NFT object, we can query it. We will start with getting the metadata of a token. I am just putting a random token as the argument.
 ```python
 print(Pixelmon.get_token_metadata(5580))
 ```
@@ -140,15 +156,15 @@
 print(f'Tokens Balance: {tokens_balance}')
 
 # Check if an address is approved for all tokens (ERC1155)
 is_approved_erc1155 = erc1155_nft.is_approved_for_all_erc1155(wallet_address, '0xOperatorAddress')
 print(f'Is Approved For All (ERC1155): {is_approved_erc1155}')
 ```
 
-### Interacting with a Wallet | NFTPy.NFTWallet
+### Interacting with a Wallet | nftpy.NFTWallet
 
 Creating an instance of `NFTWallet` requires either a private key for full access or just an address for read-only access. You can also specify multiple chains to connect to different networks simultaneously.
 
 ```python
 from nftpy import *
 
 # Initialize the wallet with a private key and specify chains
@@ -207,23 +223,23 @@
 # Output: {"Balances": {'Sepolia Testnet': 123456789012345678}}
 
 # Get the current gas price in Wei
 print(readonly_wallet.get_gas_price_wei()) 
 # Output: {'Sepolia Testnet': 20000000000}
 ```
 
-### Interacting with OpenSea API | NFTPy.OpenSea
+### Interacting with OpenSea API | nftpy.OpenSea
 We will first start by creating our class with the following arguments:
 - api_key: Your OpenSea API key.
 - chain: The blockchain network (e.g., Ethereum, Polygon).
 - collection_slug: The slug of the collection you want to query (the last part of the url when browsing the collection on opensea) This assigns the interface to a specific collection. If you are using the interface to view multiple collections then you should leave this blank
 
-**Please Note**: When defining the chain, it should be done with NFTPy.OpenSea.Chain as the api requires a special format for chain definition
+**Please Note**: When defining the chain, it should be done with nftpy.OpenSea.Chain as the api requires a special format for chain definition
 ```python
-from NFTPy import OpenSea, OpenSeaChain
+from nftpy import OpenSea, OpenSeaChain
 opensea = OpenSea(api_key='your-opensea-api-key', chain=OpenSeaChain.POLYGON, collection_slug='your-collection-slug')
 ```
 If we want to query the stats of the NFT collection we can run the following command. If you did not define a collection slug when initializing the interface you will need to define it inside this function
 ```python
 opensea.get_collection_stats()
 ```
 After running that, we should see an output resembling this:
@@ -255,24 +271,12 @@
 ```python
 print(opensea.get_collection('your-collection-slug'))  # Fetch details of a collection
 print(opensea.get_nft('0xYourContractAddress', '1'))  # Get details of a specific NFT
 print(opensea.list_events_by_nft('0xYourContractAddress', '1'))  # List events related to a specific NFT
 print(opensea.list_nfts_by_account('0xYourWalletAddress'))  # List NFTs owned by an account
 ```
 
-# Changes in 1.1.4
-### Added EVM Chain Support for these test nets
-- Holesky Testnet (ETH)
-- BSC Testnet (BSC)
-- Mumbai Testnet (MATIC)
-- Goreli (ARB)
-- Goreli (OPTIMISM)
-- Fuji Testnet (AVAX)
-- Fantom Testnet 
-- Alfajores Testnet (CELO)
-- Cronos Testnet (CHRONOS)
-
 # Coming Soon
 ## Chain Integration
 - ![Solana](https://img.shields.io/badge/Solana-00FF94?style=for-the-badge&logo=Solana&logoColor=white)
 - ![Tron](https://img.shields.io/badge/Tron-FF0600?style=for-the-badge&logo=Tron&logoColor=white)
 - ![Tezos](https://img.shields.io/badge/Tezos-2C7DF7?style=for-the-badge&logo=Tezos&logoColor=white)
```

### Comparing `nftpy-1.1.3/PKG-INFO` & `nftpy-1.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,70 @@
 Metadata-Version: 2.1
 Name: nftpy
-Version: 1.1.3
+Version: 1.1.4
 Summary: A NFT specific Python library for easy NFT integration in Python
 Home-page: https://github.com/coulterstutz/nftpy
 License: MIT
 Author: CoulterStutz
 Author-email: coultercash@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: web3 (>=6.2.0,<7.0.0)
 Project-URL: Repository, https://github.com/coulterstutz/nftpy
 Description-Content-Type: text/markdown
 
-# NFTPy
-[![PyPi](https://img.shields.io/badge/PyPi-1.1.3-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/NFTPy/)](https://pypi.org/project/NFTPy/)
-[![Python](https://img.shields.io/badge/Python-3.7,%203.8,%203.9,%203.10,%203.11,%203.12-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/NFTPy/)](https://pypi.org/project/NFTPy/)
+# nftpy
+[![PyPi](https://img.shields.io/badge/PyPi-1.1.4-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/nftpy/)](https://pypi.org/project/nftpy/)
+[![Python](https://img.shields.io/badge/Python-3.7,%203.8,%203.9,%203.10,%203.11,%203.12-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/nftpy/)](https://pypi.org/project/nftpy/)
 
 A Python package designed to facilitate the integration and adoption of NFT (ERC721, ERC1155) tokens in software applications.
 
+### Changes in 1.1.4
+###### Added EVM Chain Support for these testnets:
+- Holesky Testnet (ETH)
+- BSC Testnet (BSC)
+- Mumbai Testnet (MATIC)
+- Goerli Testnet (ARB)
+- Goerli Testnet (OPTIMISM)
+- Fuji Testnet (AVAX)
+- Fantom Testnet (FTM)
+- Alfajores Testnet (CELO)
+- Baklava Testnet (CELO)
+- Cronos Testnet (CRONOS)
+
+###### Fixed Custom Chain Assignment
+- Custom Chains are now assigned in a class not the Chains:Enum class. 
+- NFTWallet and  other EVM instances now no longer require a block explorer argument for custom chains.
+
+###### Optimizations
+- Wallet now returns using the chain symbol instead of the chain name
+- Wallet now uses threading to connect to multiple chains
+
 ## Features
 
 #### EVM Interaction with NFT Tokens
 ![Ethereum](https://img.shields.io/badge/Ethereum%20Based%20Networks-3C3C3D?style=for-the-badge&logo=Ethereum&logoColor=white)
 
-NFTPy enables interaction with the Ethereum Virtual Machine (EVM) through RPC to retrieve contract details and token holders. It provides a direct communication pathway between the client and the blockchain. Currently, transactional methods are not supported but will be implemented in future updates. The following methods are available:
+nftpy enables interaction with the Ethereum Virtual Machine (EVM) through RPC to retrieve contract details and token holders. It provides a direct communication pathway between the client and the blockchain. Currently, transactional methods are not supported but will be implemented in future updates. The following methods are available:
 
 - **get_balance**: Retrieve the balance of NFTs for a given address.
 - **get_token_uri**: Fetch the metadata URI of a specific token.
 - **get_owner**: Determine the owner of a specific token.
 - **get_approved**: Get the approved address for a specific ERC721 token.
 - **is_approved_for_all**: Check if an address is approved for all tokens owned by another address (ERC721).
 - **get_token_metadata**: Get the metadata for a specific ERC721 token.
 - **get_token_balance**: Get the balance of a specific ERC1155 token for a specific wallet address.
 - **get_tokens_balance**: Gets the balance of a specific list of tokens.
 - **is_approved_for_all_erc1155**: Check if an address is approved for all tokens owned by another address (ERC1155).
 
 #### EVM Wallet Interaction
-NFTPy includes comprehensive features for interacting with Ethereum wallets, including querying balances, fetching gas prices, and transferring NFTs. The wallet interface supports both read-only and transactional operations.
+nftpy includes comprehensive features for interacting with Ethereum wallets, including querying balances, fetching gas prices, and transferring NFTs. The wallet interface supports both read-only and transactional operations.
 
 **Wallet Features:**
 - **get_balance**: Retrieve the balance of NFTs for a given address in Ether.
 - **get_balance_wei**: Retrieve the balance of NFTs for a given address in Wei.
 - **get_gas_price_wei**: Fetch the current gas price in Wei.
 - **get_gas_price_gwei**: Fetch the current gas price in Gwei.
 - **transfer_nft**: Transfer an NFT from the wallet to another address.
@@ -52,61 +73,56 @@
 - **estimate_gas**: Estimate the gas required for a transaction.
 - **is_synced**: Check if the blockchain is synced.
 - **get_latest_block**: Get the latest block on the blockchain.
 
 #### Built-in OpenSea Interface
 ![OpenSea Support](https://img.shields.io/badge/OpenSea-%232081E2.svg?style=for-the-badge&logo=opensea&logoColor=white)
 
-NFTPy includes a built-in interface for interacting with OpenSea via an API key. This allows for in-package queries to OpenSea, enabling access to pricing information and other OpenSea-specific data. The OpenSea interface can be configured to focus on a single collection or query multiple collections. The available methods include:
+nftpy includes a built-in interface for interacting with OpenSea via an API key. This allows for in-package queries to OpenSea, enabling access to pricing information and other OpenSea-specific data. The OpenSea interface can be configured to focus on a single collection or query multiple collections. The available methods include:
 
 - **get_collection_stats**: Obtain statistics for a collection.
 - **list_events_by_nft**: List events related to a specific NFT.
 - **get_collection**: Fetch details of a specific collection.
 - **get_contract**: Retrieve details of a specific contract.
 - **get_nft**: Get details of a specific NFT.
 - **list_nfts_by_account**: List NFTs owned by a specific account.
 - **list_nfts_by_collection**: List NFTs in a specific collection.
 - **list_nfts_by_contract**: List NFTs under a specific contract.
 - **get_payment_token**: Get details of a specific payment token.
 - **get_traits**: Get traits of a specific collection.
 - **get_all_listings_on_collection**: Get all listings of a specific collection.
 
 #### Custom Chain Support
-NFTPy allows the creation of custom chains with specific chain IDs, RPC URLs, explorer URLs, and names. This feature enhances flexibility by enabling the addition of blockchain networks that are not predefined in the library.
+nftpy allows the creation of custom chains with specific chain IDs, RPC URLs, explorer URLs, and names. This feature enhances flexibility by enabling the addition of blockchain networks that are not predefined in the library.
 
 **Creating a Custom Chain:**
 ```python
-from NFTPy.EVM import Chains
+from nftpy.EVM import Chain
 
-# Create a custom chain
-custom_chain = Chains.custom_chain(
-    chain_id=999,
-    rpc_url="https://custom-rpc-url.com",
-    explorer_url="https://custom-explorer.com",
-    name="Custom Blockchain"
+custom_chain = Chain(
+        name = "Ethereum",
+        symbol = "ETH",
+        chain_id = 1,
+        rpc_url = "https://eth.llamarpc.com",
+        explorer_url = "https://etherscan.io",
+        testnet = False
 )
-
-# Access custom chain attributes
-print(custom_chain.chain_id)       # Outputs: 999
-print(custom_chain.rpc_url)        # Outputs: https://custom-rpc-url.com
-print(custom_chain.explorer_url)   # Outputs: https://custom-explorer.com
-print(custom_chain.name)           # Outputs: Custom Blockchain
 ```
 
 # Example Usage
-### Interacting on-chain with a collection | NFTPy.EVM.NFT
-Using NFTPy.EVM.NFT we are going to be querying the Pixelmon NFT collection on Ethereum mainnet!
+### Interacting on-chain with a collection | nftpy.EVM.NFT
+Using nftpy.EVM.NFT we are going to be querying the Pixelmon NFT collection on Ethereum mainnet!
 We will first start off by creating our class. We are going to define our class with three arguments:
 - contract_address: The address of the contract you are trying to query.
 - abi: The ABI of the contract you are trying to query. The EVM.ABI class provides presets for our ABI. You can also paste an ABI into the field.
 - network: This dictates what RPC URL to use and sets a preset that works best with the network.
 - rpc_url: If you do not want to use a preset and instead want to use a custom RPC, define it using this field.
 
 ```python
-import NFTPy.EVM as EVM
+import nftpy.EVM as EVM
 Pixelmon = EVM.NFT("0x32973908FaeE0Bf825A343000fE412ebE56F802A", abi=EVM.ABI.ERC721, network=EVM.Chains.ETH)
 #                   Contract Address                                ABI              Network To Query (Ethereum)
 ```
 Now that we have created our NFT object, we can query it. We will start with getting the metadata of a token. I am just putting a random token as the argument.
 ```python
 print(Pixelmon.get_token_metadata(5580))
 ```
@@ -157,15 +173,15 @@
 print(f'Tokens Balance: {tokens_balance}')
 
 # Check if an address is approved for all tokens (ERC1155)
 is_approved_erc1155 = erc1155_nft.is_approved_for_all_erc1155(wallet_address, '0xOperatorAddress')
 print(f'Is Approved For All (ERC1155): {is_approved_erc1155}')
 ```
 
-### Interacting with a Wallet | NFTPy.NFTWallet
+### Interacting with a Wallet | nftpy.NFTWallet
 
 Creating an instance of `NFTWallet` requires either a private key for full access or just an address for read-only access. You can also specify multiple chains to connect to different networks simultaneously.
 
 ```python
 from nftpy import *
 
 # Initialize the wallet with a private key and specify chains
@@ -224,23 +240,23 @@
 # Output: {"Balances": {'Sepolia Testnet': 123456789012345678}}
 
 # Get the current gas price in Wei
 print(readonly_wallet.get_gas_price_wei()) 
 # Output: {'Sepolia Testnet': 20000000000}
 ```
 
-### Interacting with OpenSea API | NFTPy.OpenSea
+### Interacting with OpenSea API | nftpy.OpenSea
 We will first start by creating our class with the following arguments:
 - api_key: Your OpenSea API key.
 - chain: The blockchain network (e.g., Ethereum, Polygon).
 - collection_slug: The slug of the collection you want to query (the last part of the url when browsing the collection on opensea) This assigns the interface to a specific collection. If you are using the interface to view multiple collections then you should leave this blank
 
-**Please Note**: When defining the chain, it should be done with NFTPy.OpenSea.Chain as the api requires a special format for chain definition
+**Please Note**: When defining the chain, it should be done with nftpy.OpenSea.Chain as the api requires a special format for chain definition
 ```python
-from NFTPy import OpenSea, OpenSeaChain
+from nftpy import OpenSea, OpenSeaChain
 opensea = OpenSea(api_key='your-opensea-api-key', chain=OpenSeaChain.POLYGON, collection_slug='your-collection-slug')
 ```
 If we want to query the stats of the NFT collection we can run the following command. If you did not define a collection slug when initializing the interface you will need to define it inside this function
 ```python
 opensea.get_collection_stats()
 ```
 After running that, we should see an output resembling this:
@@ -272,25 +288,13 @@
 ```python
 print(opensea.get_collection('your-collection-slug'))  # Fetch details of a collection
 print(opensea.get_nft('0xYourContractAddress', '1'))  # Get details of a specific NFT
 print(opensea.list_events_by_nft('0xYourContractAddress', '1'))  # List events related to a specific NFT
 print(opensea.list_nfts_by_account('0xYourWalletAddress'))  # List NFTs owned by an account
 ```
 
-# Changes in 1.1.4
-### Added EVM Chain Support for these test nets
-- Holesky Testnet (ETH)
-- BSC Testnet (BSC)
-- Mumbai Testnet (MATIC)
-- Goreli (ARB)
-- Goreli (OPTIMISM)
-- Fuji Testnet (AVAX)
-- Fantom Testnet 
-- Alfajores Testnet (CELO)
-- Cronos Testnet (CHRONOS)
-
 # Coming Soon
 ## Chain Integration
 - ![Solana](https://img.shields.io/badge/Solana-00FF94?style=for-the-badge&logo=Solana&logoColor=white)
 - ![Tron](https://img.shields.io/badge/Tron-FF0600?style=for-the-badge&logo=Tron&logoColor=white)
 - ![Tezos](https://img.shields.io/badge/Tezos-2C7DF7?style=for-the-badge&logo=Tezos&logoColor=white)
```

