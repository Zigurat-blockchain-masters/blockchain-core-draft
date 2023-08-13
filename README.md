#  Basic Blockchain Implementation in Python
This repository contains the Python code to implement basic blockchain operations. It is organized into several modules, each performing a specific functionality. We'll be re-implementing and extending this solution using Javascript/Typescript.

## Overview

The solution consists of various components that together create a simple blockchain structure:

### 1. Block Module (`Block.py`):
Defines the Block class, containing details such as previous block's hash, transactions, and nonce. The hashing functionality is included to create hash values for blocks.

### 2. Blockchain Module (`Blockchain.py`):
Manages the entire blockchain, including block insertion, validation, UTXO retrieval, and JSON serialization. It interacts with various other modules to validate transactions and blocks.

### 3. Configuration Module (`CONFIG.py`):
Stores constant values such as the mining target, used elsewhere in the code.

### 4. Cryptography Module (`crypto.py`):
Contains various cryptographic functions like key generation, password generation, signing, and verification using the RSA algorithm.

### 5. Genesis Module (`Genesis.py`):
Handles the genesis block creation and defines the creator's public key.

### 6. Hashing Module (`hashing.py`):
Provides hashing functions utilizing SHA-3_256.

### 7. Main Module (`Main.py`):
Coordinates the overall working by integrating wallet, miner, and blockchain operations.

### 8. Mempool Module (`Mempool.py`):
Manages the memory pool where transactions are held before being added to a block.

### 9. Miner Module (`Miner.py`):
Handles the mining process, including proof-of-work and rewards.

### 10. Transaction Module (`Transaction.py`):
Defines the structure and behavior of transactions within the blockchain. This module includes three classes: `Transaction`, `UnsignedTransaction`, and `Coinbase`.

- `Transaction`: Handles the creation and validation of signed transactions.
- `UnsignedTransaction`: Represents a transaction before it's signed.
- `Coinbase`: A special type of transaction used to reward miners.

### 11. UTXO Module (`UTXO.py`):
Manages Unspent Transaction Outputs (UTXO) which represent the output of a transaction that can be spent in future transactions.

- `UTXO`: Contains the transaction hash, public key, and a message. Utilizes hashing functions and provides methods for retrieving dictionary representations.


### 12. Wallet Module (`Wallet.py`):
Responsible for managing a user's wallet, including the creation of transactions and interaction with the memory pool.

Manages private and public keys, creates and signs transactions, and interacts with the blockchain and memory pool. It can save and load keys from files.


## Future Development

The next phase of this project involves re-implementing and extending this solution using Javascript/Typescript. More details will be added as the project progresses.


## License

This project is licensed under the GNU Affero General Public License v3.0. See the [LICENSE](./LICENSE) file for details, or you can visit [GNU Affero General Public License v3.0](https://www.gnu.org/licenses/agpl-3.0.en.html) for more information.