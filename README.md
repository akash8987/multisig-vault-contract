# Multisig Vault Contract

A minimalist yet highly secure Multi-Signature Wallet (Multisig) smart contract built with Solidity. This repository serves as a professional-grade reference for managing shared crypto assets.

## Overview
This contract allows a group of owners to manage funds collectively. A transaction is only executed if it receives a predefined number of required confirmations ($m$ of $n$ signatures).

### Key Features
* **Safe Multi-ownership:** Add multiple addresses as authorized signers.
* **Configurable Threshold:** Set the specific number of confirmations needed to move funds.
* **Transaction Lifecycle:** Submit, confirm, execute, and revoke transaction flows.
* **Native ETH Support:** Built to handle and store Ether securely.

## Technical Stack
* **Language:** Solidity ^0.8.20
* **Framework:** Compatible with Hardhat, Foundry, or Remix.
* **License:** MIT

## Getting Started
1. Deploy the contract by passing an array of owner addresses and the required number of confirmations to the constructor.
2. Submit a transaction using `submitTransaction`.
3. Other owners can call `confirmTransaction`.
4. Once the threshold is met, any owner can call `executeTransaction`.
