# Day 10 - Programmable Blockchains (Ethereum)

## Overview

This module introduces Ethereum, a programmable blockchain platform that enables developers to build Smart Contracts and Decentralized Applications (DApps). It also covers Ethereum's consensus mechanisms and its evolution from Proof of Work to Proof of Stake.

---

# 1. Introduction to Ethereum

## Definition

Ethereum is a programmable blockchain platform that allows developers to build **Smart Contracts** and **Decentralized Applications (DApps)**.

---

## Creator

**Vitalik Buterin**

### Important Timeline

| Year | Event |
|---------|----------------------------|
| 2013 | Ethereum Whitepaper Published |
| 2015 | First Ethereum Test Network |

---

## Why Ethereum?

Ethereum was designed to overcome the limitations of Bitcoin.

### Bitcoin Limitations

- Lack of Turing Completeness
- Value Blindness
- Lack of State
- Blockchain-blindness

---

## Ethereum Concept

Ethereum is often called the **World Computer** because anyone can execute programs and applications on a decentralized network.

---

# 2. Ethereum World Computer

## Definition

A decentralized global computer where anyone can execute smart contracts and decentralized applications.

### Architecture

```
Users

↓

Ethereum Network

↓

Ethereum Virtual Machine (EVM)

↓

Smart Contracts

↓

Same Output Everywhere
```

---

## Ethereum Virtual Machine (EVM)

The EVM executes smart contracts on every Ethereum node.

---

## Properties of Ethereum World Computer

### Deterministic

Same input always produces the same output.

### Terminable

Programs stop after execution.

### Isolated

Programs are independent and are not affected by external factors.

---

# 3. Ethereum Features

## Main Features

### Adaptable & Flexible

Supports programmable smart contracts and custom business logic.

---

### User Authentication

Uses cryptographic signatures for secure identity verification.

---

### Easily Deployable Payment Logic

Payments can be executed without third-party services.

---

### Total DDoS Resistance

No single point of failure due to decentralization.

---

### Limitless Interoperability

Smart contracts can interact with each other.

---

### No Server Infrastructure

Uses a Peer-to-Peer decentralized network instead of centralized servers.

---

## Additional Facts

- Ethereum initially used Proof of Work (PoW).
- Average transaction time: **15–20 seconds**.
- Ethereum test networks may use:
  - Proof of Work (PoW)
  - Proof of Stake (PoS)
  - Proof of Authority (PoA)

---

# 4. Working of Proof of Stake (PoS)

## Definition

Proof of Stake is a consensus mechanism where validators are selected based on the amount of cryptocurrency they stake rather than computational power.

---

## Validator Selection Methods

### Randomized Block Selection

Selection based on:

- Lowest Hash
- Highest Stake

---

### Coin Age Selection

```
Coin Age = Number of Coins × Number of Days Held
```

---

## Ethereum PoS

Ethereum uses **RANDAO**, a pseudo-random validator selection mechanism.

---

## Time Structure

```
Epoch

↓

32 Slots

↓

Each Slot = 12 Seconds

↓

Validator Selected

↓

Committee Votes

↓

Block Added
```

---

## Committee

Minimum:

**128 Validators**

---

## Advantages of PoS

- Energy Efficient
- Random validator selection
- Reduced centralization
- Lower attack probability

---

## Disadvantage

### Nothing at Stake Problem

Validators may validate multiple blockchain branches simultaneously.

### Solution

Ethereum uses **Slashing**, where a validator loses part of its stake as punishment.

---

## Variants of PoS

- Delegated PoS
- Liquid PoS
- Bonded PoS
- Hybrid PoS

---

# 5. Proof of Authority (PoA)

## Definition

A reputation-based consensus mechanism mainly used in private blockchains.

Validators stake their reputation instead of cryptocurrency.

---

## Requirements

- Trusted identities
- Reputation at stake
- Equal validator selection

---

## Advantages

- Highly scalable
- No mining required
- No native currency needed
- Suitable for supply chain and logistics
- Better privacy

---

## Disadvantages

- More centralized
- Possibility of censorship
- Third-party manipulation

---

# 6. Roadmap to Ethereum Evolution

## Beacon Chain (2020)

- Dummy blockchain
- Introduced Proof of Stake
- Validators stake **32 ETH**

---

## The Merge (2022)

Merged the Beacon Chain with Ethereum Mainnet.

### Transition

```
Proof of Work

↓

Proof of Stake
```

### Result

Energy consumption reduced by:

**99.95%**

---

## Dencun Upgrade

### Original Plan

- Sharding
- 64 Shards
- Better scalability

### Updated Plan

**Proto-Danksharding**

Provides:

- Layer 2 Rollup Support
- Lower Data Storage Cost
- Better Scalability

---

# Complete Module Flow

```
Ethereum

↓

World Computer

↓

Ethereum Virtual Machine (EVM)

↓

Smart Contracts & DApps

↓

Proof of Stake (PoS)

↓

Validators

↓

Proof of Authority (PoA)

↓

Private Blockchain

↓

Beacon Chain (2020)

↓

The Merge (2022)

↓

PoW → PoS

↓

Dencun Upgrade

↓

Proto-Danksharding
```

---

# Important Definitions

## Ethereum

Programmable blockchain for Smart Contracts and DApps.

---

## EVM

Ethereum Virtual Machine that executes smart contracts.

---

## Deterministic

Same input always produces the same output.

---

## Proof of Stake (PoS)

Consensus mechanism based on validators' stake.

---

## Validator

Node selected to validate transactions.

---

## Coin Age

```
Number of Coins × Number of Days Held
```

---

## RANDAO

Pseudo-random validator selection method.

---

## Nothing at Stake Problem

Validators validate multiple branches simultaneously.

---

## Proof of Authority (PoA)

Consensus mechanism based on trusted identities and reputation.

---

## Beacon Chain

Proof of Stake blockchain introduced in 2020.

---

## The Merge

Ethereum's transition from Proof of Work to Proof of Stake in 2022.

---

## Proto-Danksharding

Ethereum scalability upgrade replacing traditional shard chains.

---

# Quick Revision

### Ethereum

- Creator: Vitalik Buterin
- Whitepaper: 2013
- Test Network: 2015

### Ethereum World Computer

- EVM
- Deterministic
- Terminable
- Isolated

### Proof of Stake

- Validators
- Stake
- RANDAO
- Epoch → 32 Slots → Committee

### Proof of Authority

- Trusted Identity
- Reputation-based
- Private Blockchain

### Ethereum Evolution

2020 → Beacon Chain

↓

32 ETH Stake

↓

2022 → The Merge

↓

PoW → PoS

↓

99.95% Less Energy

↓

Dencun Upgrade

↓

Proto-Danksharding

---

# Key Takeaways

- Ethereum extends blockchain functionality beyond digital currency.
- The Ethereum Virtual Machine executes smart contracts consistently across all nodes.
- Proof of Stake replaces mining with validators, making Ethereum more energy efficient.
- Proof of Authority is ideal for private enterprise blockchains.
- The Merge reduced Ethereum's energy consumption by approximately **99.95%**, making it significantly more sustainable.

---

# Summary

Ethereum is a programmable blockchain platform designed for Smart Contracts and DApps. Through the Ethereum Virtual Machine (EVM), developers can build decentralized applications that execute consistently across the network. Ethereum's transition from Proof of Work to Proof of Stake through The Merge significantly improved energy efficiency and scalability, while upgrades like Proto-Danksharding continue to enhance its performance and future growth.