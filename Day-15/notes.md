# Day 15 - Permissioned Blockchains

## Overview

This module introduces Permissioned Blockchains, LF Decentralized Trust (LFDT), Hyperledger Fabric, Corda, and their enterprise use cases.

---

# 1. Need for Permissioned Blockchains

## Why Permissioned Blockchains?

Public blockchains such as Bitcoin and Ethereum face several challenges:

- Low Transactions Per Second (TPS)
- High Transaction Fees
- Public Data Visibility
- Scalability Issues

Permissioned blockchains are designed to overcome these limitations.

---

## Benefits

✅ Business Compatibility

✅ Higher Throughput (TPS)

✅ Defined Governance

✅ Cost Effective

---

## Examples

- Hyperledger Fabric
- Hyperledger Sawtooth
- R3 Corda

---

# 2. LF Decentralized Trust (LFDT)

## Definition

LF Decentralized Trust (LFDT) is an open-source initiative under the Linux Foundation focused on blockchain and decentralized technologies.

---

## Goals

- Transparency
- Reliability
- Security
- Efficiency

---

## Provides

- Frameworks
- Tools
- Libraries
- Standards

---

# 3. Important LFDT Projects

## Hyperledger Fabric

Enterprise permissioned blockchain framework.

---

## Hyperledger Besu

Ethereum client written in Java.

---

## Hyperledger Indy

Digital identity platform.

---

## Hyperledger Aries

Credential management toolkit.

---

## Hyperledger Caliper

Blockchain benchmarking tool.

---

## Hyperledger Cacti

Blockchain integration tool.

---

## Hyperledger FireFly

Enterprise Web3 platform.

---

## Solang

Solidity compiler.

---

# 4. Hyperledger Fabric

## Definition

Hyperledger Fabric is an open-source permissioned blockchain framework originally contributed by IBM and Digital Asset.

---

## Features

- Permissioned Network
- Modular Architecture
- Chaincode Support
- Identity Management
- Pluggable Consensus

---

# Hyperledger Fabric Components

## Peer

Stores ledger data.

---

## Endorsing Peer

Approves and endorses transactions.

---

## Orderer

Creates and orders blocks.

---

## Client

Interacts with the blockchain network.

---

## MSP (Membership Service Provider)

Handles identity management.

---

## Channel

Private subnet used for confidential communication.

---

## Chaincode

Fabric's smart contract implementation.

---

# Hyperledger Fabric Transaction Flow

```
Client

↓

Endorsing Peer

↓

Orderer

↓

Block Creation

↓

Peers

↓

Ledger Update
```

---

# 5. Hyperledger Fabric Lab

## Practical Commands

### Create Network

```bash
./network.sh up createChannel
```

### Deploy Chaincode

```bash
./network.sh deployCC
```

### Initialize Ledger

```bash
peer chaincode invoke
```

### Query Ledger

```bash
peer chaincode query
```

### Shutdown Network

```bash
./network.sh down
```

---

# 6. Corda by R3

## Definition

Corda is a permissioned Distributed Ledger Technology (DLT) platform developed by R3.

---

## Key Difference

### Traditional Blockchain

```
Transactions

↓

Blocks

↓

Confirmation
```

### Corda

```
Transaction

↓

Verification

↓

Confirmation
```

No blocks.

No mining.

Real-time validation.

---

# 7. Features of Corda

## Privacy

Only involved parties can view transaction data.

---

## Transaction Finality

Immediate confirmation of transactions.

---

## Legal Identity

Uses X.500 Distinguished Names.

---

## Scalability

No blocks, resulting in better performance.

---

## Enterprise Integration

Easy integration with business applications.

---

# 8. Corda Components

## Node

Network participant.

---

## CorDapp

Corda Distributed Application.

---

## State

Represents an asset or piece of data.

---

## Contract

Contains transaction validation rules.

---

## Command

Represents an action performed.

---

## Attachment

Stores supporting legal documents.

---

## Notary ⭐

Prevents double spending.

---

## Ledger

Stores finalized transactions.

---

# Corda Transaction Flow

```
CorDapp

↓

Build Transaction

↓

State + Contract + Command

↓

Signatures

↓

Notary

↓

Finality

↓

Ledger
```

---

# Hyperledger Fabric vs Corda

| Hyperledger Fabric | Corda |
|-------------------|--------|
| Permissioned Blockchain | Permissioned DLT |
| Uses Blocks | No Blocks |
| Chaincode | CorDapp |
| Orderer Creates Blocks | Notary Validates Transactions |
| Channels for Privacy | Point-to-Point Privacy |
| IBM Contribution | R3 Contribution |

---

# Important Definitions

## Permissioned Blockchain

A blockchain where only authorized participants can join and perform actions.

---

## LFDT

Linux Foundation Decentralized Trust initiative.

---

## Hyperledger Fabric

Enterprise permissioned blockchain framework.

---

## Chaincode

Smart contract implementation in Hyperledger Fabric.

---

## MSP

Membership Service Provider responsible for identity management.

---

## Corda

Permissioned distributed ledger platform developed by R3.

---

## CorDapp

Application built on the Corda platform.

---

## Notary

Component that prevents double spending in Corda.

---

## Transaction Finality

Immediate and irreversible transaction confirmation.

---

# Important Exam Questions

## 2-Mark Questions

- What is a Permissioned Blockchain?
- What is LFDT?
- What is Hyperledger Fabric?
- What is Chaincode?
- What is MSP?
- What is a Channel?
- What is Corda?
- What is CorDapp?
- What is a Notary?
- What is Transaction Finality?

---

## 5-Mark Questions

- Explain the need for Permissioned Blockchains.
- Explain LFDT and its projects.
- Explain Hyperledger Fabric architecture.
- Explain Hyperledger Fabric lab workflow.
- Explain Corda by R3.
- Explain features of Corda.
- Explain Corda components and transaction flow.

---

# Super Revision Flow

```
Permissioned Blockchain

↓

LFDT

↓

Hyperledger Projects

↓

Hyperledger Fabric

(Peer, Orderer, MSP, Channel, Chaincode)

↓

Fabric Lab

↓

Corda

↓

Features of Corda

↓

CorDapp

↓

Notary

↓

Transaction Finality
```

---

# Memory Trick

**PFHFCN**

- P → Permissioned Blockchain
- F → LFDT Frameworks
- H → Hyperledger Fabric
- F → Fabric Lab
- C → Corda
- N → Notary

---

# Key Takeaways

- Permissioned blockchains are designed for enterprise environments.
- Hyperledger Fabric provides modular architecture, identity management, and private channels.
- Corda focuses on privacy, transaction finality, and real-time validation.
- Notary plays a crucial role in preventing double spending in Corda.
- LFDT supports multiple blockchain projects and enterprise solutions.

---

# Summary

Permissioned blockchains address the scalability, privacy, and governance challenges of public blockchains. Hyperledger Fabric and Corda are two major enterprise blockchain platforms. Fabric uses blocks, channels, and chaincode, while Corda uses CorDapps, Notaries, and direct transaction validation. Both are widely used in enterprise and business environments.