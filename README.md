#  Basic Blockchain Implementation in Python
This repository contains the Python code to implement basic blockchain operations. It is organized into several modules, each performing a specific functionality. We'll be re-implementing and extending this solution using Javascript/Typescript.

## Overview

The solution consists of various components that together create a simple blockchain structure:

### 1. **Block Module (`Block.py`)**:
Defines the Block class, containing details such as previous block's hash, transactions, and nonce. The hashing functionality is included to create hash values for blocks.

### 2. **Blockchain Module (`Blockchain.py`)**:
Manages the entire blockchain, including block insertion, validation, UTXO retrieval, and JSON serialization. It interacts with various other modules to validate transactions and blocks.

### 3. **Configuration Module (`CONFIG.py`)**:
Stores constant values such as the mining target, used elsewhere in the code.

### 4. **Cryptography Module (`crypto.py`)**:
Contains various cryptographic functions like key generation, password generation, signing, and verification using the RSA algorithm.

### 5. **Genesis Module (`Genesis.py`)**:
Handles the genesis block creation and defines the creator's public key.

### 6. **Hashing Module (`hashing.py`)**:
Provides hashing functions utilizing SHA-3_256.

### 7. **Main Module (`Main.py`)**:
Coordinates the overall working by integrating wallet, miner, and blockchain operations.

### 8. **Mempool Module (`Mempool.py`)**:
Manages the memory pool where transactions are held before being added to a block.

### 9. **Miner Module (`Miner.py`)**:
Handles the mining process, including proof-of-work and rewards.

### 10. **Transaction Module (`Transaction.py`)**:

### 11. **UTXO Module (`UTXO.py`)**:

### 12. **Wallet Module (`Wallet.py`)**:


## Future Development

The next phase of this project involves re-implementing and extending this solution using Javascript/Typescript. More details will be added as the project progresses.