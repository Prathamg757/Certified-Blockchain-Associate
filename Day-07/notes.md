# Day 07 - Bitcoin Blockchain Network

## Overview

This module introduces the Bitcoin Blockchain Network, different types of blockchains, Bitcoin fundamentals, and the various nodes that maintain the Bitcoin network.

---

# 1. Types of Blockchains

Blockchain networks are classified into three types:

```
Blockchain

│

├── Public Blockchain

├── Private Blockchain

└── Hybrid Blockchain
```

---

## A) Public Blockchain

### Definition

A Public Blockchain is an open and decentralized blockchain where anyone can participate.

### Features

- Open to everyone
- Fully decentralized
- Anyone can read and write data
- Anyone can create blocks
- Uses tokens as rewards
- High transparency

### Examples

- Bitcoin
- Ethereum

---

## B) Private Blockchain

### Definition

A Private Blockchain is a permissioned blockchain where only authorized users can participate.

### Features

- Permission required
- Transactions are private
- More centralized
- Controlled governance
- May or may not use tokens

---

## C) Hybrid Blockchain

### Definition

A Hybrid Blockchain combines the features of both Public and Private Blockchains.

### Features

- Combines transparency and privacy
- Flexible architecture
- Business friendly
- Secure

---

# Comparison of Blockchains

| Public | Private | Hybrid |
|---------|----------|---------|
| Open to everyone | Permission required | Combination of both |
| Fully decentralized | More centralized | Partially decentralized |
| Transparent | Private | Flexible |
| Bitcoin, Ethereum | Enterprise blockchain | Business applications |

---

# 2. What is Bitcoin?

## Definition

Bitcoin is a decentralized digital currency that enables peer-to-peer online payments without banks or governments.

---

## Introduced By

**Satoshi Nakamoto**

### Year

2008

### Whitepaper

**Bitcoin: A Peer-to-Peer Electronic Cash System**

---

## Purpose

- Direct online payments
- Remove intermediaries
- Create a decentralized financial system

---

## Features of Bitcoin

- Decentralized
- Peer-to-Peer (P2P)
- Digital Currency
- Transparent
- Secure
- Irreversible Transactions

---

## Maximum Supply

Bitcoin has a maximum supply of:

**21 Million Bitcoins**

No more than 21 million Bitcoins will ever exist.

---

## Bitcoin Transaction Flow

```
Alice

↓

Bitcoin Network

↓

Blockchain Verification

↓

Bob
```

No bank or central authority is involved.

---

# 3. Nodes in Bitcoin Network

## Definition

A Node is a computer that participates in the Bitcoin blockchain network.

---

# Types of Nodes

```
Bitcoin Network

│

├── Full Node

├── Lightweight Node

├── Miner Node

└── Router Node
```

---

## A) Full Node

### Definition

A Full Node stores the complete blockchain database.

### Functions

- Stores complete blockchain
- Independently verifies transactions
- Provides high security

---

## B) Lightweight Node

### Definition

A Lightweight Node stores only block headers instead of the complete blockchain.

Uses:

**SPV (Simplified Payment Verification)**

### Features

- Less storage required
- Faster synchronization
- Suitable for mobile devices

---

## SPV (Simplified Payment Verification)

SPV verifies transactions without downloading the complete blockchain.

It uses:

- Block Headers
- Merkle Path
- Merkle Root

---

## C) Miner Node

### Definition

A Miner Node performs mining operations and creates new blocks.

### Functions

- Collects transactions
- Mines blocks
- Adds blocks to blockchain
- Receives mining rewards

---

## D) Router Node

### Definition

A Router Node routes requests and transactions between different nodes.

### Function

Acts as a communication bridge within the network.

---

## Important Note

A single node can perform multiple roles.

Example:

```
Node

↓

Full Node

+

Miner Node

+

Router Node
```

---

# Comparison of Bitcoin Nodes

| Full Node | Lightweight Node | Miner Node | Router Node |
|------------|-----------------|------------|-------------|
| Complete blockchain | Block headers only | Performs mining | Routes requests |
| Independent verification | Uses SPV | Creates new blocks | Connects nodes |
| High storage | Low storage | High computation | Communication role |

---

# Important Definitions

## Blockchain

A decentralized distributed ledger that securely records transactions.

## Public Blockchain

An open blockchain where anyone can participate.

## Private Blockchain

A permissioned blockchain accessible only to authorized users.

## Hybrid Blockchain

A blockchain that combines features of public and private blockchains.

## Bitcoin

A decentralized digital currency introduced by Satoshi Nakamoto.

## Node

A computer participating in the blockchain network.

## Full Node

Stores and verifies the complete blockchain.

## Lightweight Node

Stores only block headers and verifies transactions using SPV.

## Miner Node

Creates new blocks through mining.

## Router Node

Routes requests and connects blockchain nodes.

## SPV (Simplified Payment Verification)

A method of verifying transactions without downloading the complete blockchain.

---

# Key Takeaways

- Blockchain networks can be Public, Private, or Hybrid.
- Bitcoin is the first decentralized digital currency.
- Bitcoin removes the need for banks by enabling peer-to-peer transactions.
- Different types of nodes perform different functions in maintaining the Bitcoin network.
- Lightweight nodes use SPV for efficient transaction verification.

---

# Summary

Bitcoin is a decentralized peer-to-peer digital currency that operates on a public blockchain. The Bitcoin network is maintained by different types of nodes, including Full Nodes, Lightweight Nodes, Miner Nodes, and Router Nodes. Together, these nodes ensure security, transparency, decentralization, and reliable transaction processing.