# Day 14 - Ethereum Hands-On

## Overview

This module introduces the practical tools used for Ethereum Smart Contract development, deployment, and testing.

Topics Covered:

- Remix IDE
- Solidity Compiler
- Deploy & Run Transactions
- MetaMask
- Etherscan
- Ethereum Test Network (Sepolia)
- Ganache (Deprecated)

---

# 1. Remix IDE File Explorer & Code Editor

## Definition

Remix IDE is an open-source browser-based development environment used for Ethereum Smart Contract development.

### Supported Languages

- Solidity
- Vyper

---

## Features

- Code
- Compile
- Test
- Debug
- Deploy

---

## Sample Files

- Storage.sol
- Owner.sol
- Ballot.sol
- Ballot_test.sol

---

## File Explorer Options

- New File
- Open File
- Connect Localhost
- Import from GitHub
- Import from IPFS
- Import from Gist

---

# 2. Remix IDE Compiler Tab

## Purpose

The Compiler Tab compiles Solidity code and detects syntax errors before deployment.

---

## Required Plugins

- Solidity Compiler
- Deploy & Run Transactions

---

## Important Compiler Options

- Compiler Version
- Language
- EVM Version
- Auto Compile
- Enable Optimization
- Hide Warnings

---

## Compilation Output

### ABI (Application Binary Interface)

Used by applications and wallets to interact with Smart Contracts.

### Bytecode

Compiled machine-readable code deployed to the Ethereum Virtual Machine (EVM).

### Metadata

Contains additional information about the compiled contract.

---

# 3. Remix IDE Deploy & Run Transactions

## Purpose

Used to deploy and execute Smart Contracts.

---

## Environment Options

- Remix VM
- Injected Provider (MetaMask)
- External HTTP Provider
- Hardhat
- Ganache
- Foundry

---

## Deployment Options

- Account
- Gas Limit
- Value

---

## Button Colors

### 🔵 Blue Button

- Read Only Function
- No Gas Required

### 🟠 Orange Button

- Changes Blockchain State
- Gas Required

---

## At Address

Used to connect and interact with an already deployed Smart Contract.

---

# 4. MetaMask

## Definition

MetaMask is a browser extension wallet (Light Client) used to interact with Ethereum networks.

---

## Features

- Create Wallet
- Import Wallet
- Send ETH
- Receive ETH
- Manage Multiple Accounts
- Connect to Mainnet & Testnets

---

## Seed Phrase

A recovery phrase used to restore wallet access.

**Important:** Never share your Seed Phrase with anyone.

---

## Supported Networks

- Ethereum Mainnet
- Sepolia Test Network

---

## Faucet

Provides free Test Ether (Test ETH) for development and testing.

---

# 5. Etherscan

## Definition

Etherscan is a blockchain explorer and analytics platform for Ethereum.

---

## Search Options

- Blocks
- Transactions
- Wallet Addresses
- Smart Contracts

---

## Important Facts

### Genesis Block

Block Number:

```
0
```

### Transaction Hash

A unique identifier assigned to every Ethereum transaction.

---

# 6. Interacting with Ethereum Test Network (Sepolia)

## Deployment Steps

1. Compile Smart Contract
2. Open Deploy & Run Transactions
3. Select **Injected Provider – MetaMask**
4. Connect Sepolia Account
5. Grant Permission
6. Click Deploy
7. Confirm Transaction in MetaMask
8. Wait approximately 2 minutes
9. Contract appears under **Deployed Contracts**
10. Interact with contract functions

---

# 7. Ganache (Deprecated)

## Definition

Ganache is a local Ethereum blockchain simulator used for Smart Contract development and testing.

---

## Purpose

- Test Smart Contracts
- Execute Transactions
- Inspect Blockchain State

---

## Workspace Options

- QuickStart
- New Workspace

---

## Configuration Tabs

- Workspace
- Server
- Accounts & Keys
- Chain
- Advanced

---

## Information Displayed

- Current Block
- Gas Price
- Gas Limit
- Network ID
- RPC Server
- Mining Status

---

## Default Configuration

- 10 Test Accounts
- Preloaded Test Ether

---

## Ganache Tabs

- Accounts
- Blocks
- Transactions
- Contracts & Events
- Logs

---

## Connect Ganache with Remix

Environment:

```
Web3 Provider
```

Example RPC Endpoint:

```
http://127.0.0.1:7545
```

---

# Complete Module Flow

```
Ethereum Hands-On

│

├── Remix IDE
│      ├── File Explorer
│      ├── Code Editor
│      ├── Compiler
│      └── Deploy & Run Transactions
│
├── MetaMask Wallet
│
├── Etherscan
│
├── Ethereum Test Network (Sepolia)
│
└── Ganache Blockchain Simulator
```

---

# Important Definitions

## Remix IDE

Browser-based IDE for Ethereum Smart Contract development.

---

## ABI (Application Binary Interface)

Interface used to communicate with deployed Smart Contracts.

---

## Bytecode

Compiled code deployed to the Ethereum Virtual Machine.

---

## MetaMask

Browser wallet used to interact with Ethereum networks.

---

## Seed Phrase

Recovery phrase used to restore wallet access.

---

## Etherscan

Blockchain explorer for viewing Ethereum transactions and accounts.

---

## Sepolia

Ethereum Proof-of-Stake Test Network used for Smart Contract testing.

---

## Faucet

Service that provides free Test ETH.

---

## Ganache

Local Ethereum blockchain simulator for development and testing.

---

# Key Takeaways

- Remix IDE provides an all-in-one environment for coding, compiling, testing, and deploying Smart Contracts.
- MetaMask connects users and developers to Ethereum networks.
- Etherscan helps monitor blocks, transactions, and wallet addresses.
- Sepolia Testnet allows developers to test applications using free Test ETH.
- Ganache enables local blockchain simulation without using public networks.

---

# Summary

Ethereum Hands-On tools simplify Smart Contract development and testing. Remix IDE provides a browser-based development environment, MetaMask manages wallets and transactions, Etherscan offers blockchain analytics, Sepolia provides a safe testing network, and Ganache enables local blockchain simulation for rapid development and debugging.