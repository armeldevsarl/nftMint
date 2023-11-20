# nftMint
## MyToken Smart Contract

### Introduction

This smart contract implements an ERC721 token with the following features:

* Pausable: The contract can be paused by the owner to prevent minting or transfers.
* Minting: The contract supports public minting and allowlist minting.
* Allowlist: The owner can add addresses to the allowlist to allow them to mint tokens during the allowlist minting period.
* Withdrawal: The owner can withdraw the balance of the contract.

### Usage

**Deployment**

To deploy the contract, you will need to compile it using a Solidity compiler and then deploy it to an Ethereum blockchain.

**Public Minting**

To mint a token during the public minting period, send 0.01 ether to the contract address.

**Allowlist Minting**

To mint a token during the allowlist minting period, send 0.001 ether to the contract address. You must also be on the allowlist.

**Pausing**

The owner can pause the contract to prevent minting or transfers. To pause the contract, call the `pause()` function.

**Unpausing**

The owner can unpause the contract to allow minting and transfers. To unpause the contract, call the `unpause()` function.

**Withdraw**

The owner can withdraw the balance of the contract to the specified address. To withdraw the balance, call the `withdraw()` function with the address of the recipient.

**Adding to the Allowlist**

The owner can add addresses to the allowlist to allow them to mint tokens during the allowlist minting period. To add an address to the allowlist, call the `setAllowList()` function with an array of addresses.

### License

MIT
