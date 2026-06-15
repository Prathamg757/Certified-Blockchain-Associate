# Day 09 - Bitcoin Working (Part 2)

## Overview

This module explains:

- Bitcoin Mining
- Difficulty Level
- Mining Pools
- Fork Resolution
- Hard Fork vs Soft Fork
- Bitcoin Limitations

---

# 1. Bitcoin Mining

## Definition

Bitcoin Mining is the process of solving cryptographic puzzles to create new blocks and add them to the blockchain.

---

## Mining Flow

```
Transactions

↓

Miner

↓

Solve Cryptographic Puzzle

↓

New Block

↓

Blockchain

↓

Bitcoin Reward
```

---

## Key Points

- Miners solve cryptographic puzzles.
- The first miner to solve the puzzle creates the new block.
- Mining rewards started at **50 BTC**.
- Rewards are reduced by half every **4 years (Halving)**.
- Current reward (as per course notes): **6.25 BTC**.
- Maximum Bitcoin supply = **21 Million BTC**.
- After the year **2140**, miners will receive only **transaction fees**.

---

# 2. Difficulty Level and Mining

## Definition

Difficulty determines how hard it is for miners to solve the cryptographic puzzle.

### Goal

Maintain:

**1 Block Every 10 Minutes**

---

## Difficulty Adjustment

Difficulty is automatically adjusted after:

**Every 2016 Blocks**

---

### If Mining is Too Fast

```
More Miners

↓

Blocks Created Faster

↓

Difficulty Increases
```

---

### If Mining is Too Slow

```
Fewer Miners

↓

Blocks Created Slower

↓

Difficulty Decreases
```

---

# Mining Pool

## Definition

A Mining Pool is a group of miners who combine their computational power to solve puzzles together.

---

## Mining Pool Flow

```
Miner 1

Miner 2

Miner 3

↓

Mining Pool

↓

Solve Puzzle

↓

Reward Shared
```

---

## Advantages

- Higher chance of earning rewards
- Shared computational power
- Rewards distributed among participants

---

# 3. Fork Resolution

## Definition

A Fork occurs when two miners create valid blocks at the same time.

---

## Example

```
Block 99

↓

100A      100B
```

Two versions of the blockchain temporarily exist.

---

# Longest Chain Rule

The blockchain with the **highest cumulative work (Longest Chain)** is accepted.

```
100A

↓

101A

↓

Longest Chain Wins

↓

100B Discarded
```

---

# 4. Hard Fork vs Soft Fork

## Hard Fork

### Definition

A permanent protocol change that creates two separate blockchains.

### Features

- Permanent split
- Not backward compatible
- Two independent blockchains continue

---

## Soft Fork

### Definition

A temporary protocol change that is backward compatible.

### Features

- Temporary split
- Longest chain rule applied
- Only one blockchain survives

---

# Stale Block

## Definition

A valid block that is discarded because it is not part of the longest chain.

### Important

- No mining reward is given.

---

# Orphan Block

## Definition

A block that does not have a valid parent block.

---

# Bitcoin Confirmation Rule

For maximum security,

Wait for:

**6 Block Confirmations**

before considering a transaction final.

Approximate confirmation time:

**6 × 10 minutes = 1 hour**

---

# Hard Fork vs Soft Fork

| Hard Fork | Soft Fork |
|------------|------------|
| Permanent split | Temporary split |
| Not backward compatible | Backward compatible |
| Creates separate blockchains | One chain survives |
| Protocol change | Longest chain rule |

---

# 5. Bitcoin Limitations

## A) Expensive Infrastructure

- Requires ASIC mining hardware
- High setup and maintenance cost

---

## B) Electronic Waste (E-Waste)

- Mining hardware becomes outdated quickly
- Produces electronic waste

---

## C) Useless Computations

Mining calculations only secure Bitcoin.

They cannot be reused for other applications.

---

## D) 51% Attack

### Definition

If an attacker controls **51% of the network's computing power**, they can:

- Control block generation
- Reverse transactions
- Receive most mining rewards

---

## E) Slow Transaction Time

- Average block time = **10 minutes**
- 6 confirmations recommended
- Final confirmation ≈ **1 hour**

---

## F) High Energy Consumption

- ASIC miners consume large amounts of electricity
- Leads to high operational cost
- Environmental concerns

---

## G) Limited Programmability

Bitcoin mainly supports:

- Digital cash transactions

It has:

- Limited scripting capabilities
- Limited support for Decentralized Applications (DApps)

---

# Relationship Between Topics

```
Transactions

↓

Bitcoin Mining

↓

Difficulty Level

↓

Mining Pool

↓

Block Created

↓

Fork (if two blocks are created)

↓

Longest Chain Rule

↓

Hard/Soft Fork Resolution

↓

Common Blockchain

↓

Bitcoin Limitations
```

---

# Important Definitions

## Bitcoin Mining

Process of solving cryptographic puzzles to create new blocks.

---

## Difficulty Level

Measure of how difficult it is to mine a valid block.

---

## Mining Pool

Group of miners sharing computational power and rewards.

---

## Fork

Situation where two valid blocks are created at the same time.

---

## Longest Chain Rule

Rule that accepts the blockchain with the highest cumulative work.

---

## Hard Fork

Permanent protocol change resulting in two separate blockchains.

---

## Soft Fork

Backward-compatible protocol change where one chain survives.

---

## Stale Block

Valid block discarded because it is not part of the longest chain.

---

## Orphan Block

Block without a valid parent block.

---

## 51% Attack

Attack where an entity controls more than 51% of the network's computing power.

---

# Key Takeaways

- Bitcoin mining secures the network through Proof of Work.
- Difficulty adjusts every 2016 blocks to maintain a 10-minute block time.
- Mining pools improve the chances of earning rewards.
- Forks are resolved using the Longest Chain Rule.
- Hard forks create permanent splits, while soft forks are temporary.
- Bitcoin has limitations such as high energy consumption, slow transactions, and limited programmability.

---

# Summary

Bitcoin maintains security through mining, Proof of Work, and automatic difficulty adjustment. Forks are resolved using the longest chain rule, ensuring network consistency. Although Bitcoin provides a secure decentralized payment system, it faces challenges such as high energy usage, expensive infrastructure, slow transaction speed, and limited programmability.