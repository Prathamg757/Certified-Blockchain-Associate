# Day 08 - Bitcoin Working (Part 1)

## Overview

This module explains how Bitcoin transactions are processed using Memory Pools, UTXO, Proof of Work (PoW), and Cryptographic Puzzles.

---

# 1. Transactions and Memory Pools

## Definition

When a user sends a Bitcoin transaction, it is first verified by network nodes and then stored temporarily in a **Memory Pool (Mempool)** before being added to a block.

## Transaction Flow

```
Wallet

↓

Nodes

↓

Verification

↓

Memory Pool (Mempool)

↓

Block

↓

Blockchain
```

## Key Points

- Mempool is a temporary storage area.
- It stores verified transactions.
- Miners select transactions from the mempool to create new blocks.

---

# 2. UTXO (Unspent Transaction Output)

## Definition

UTXO is the record-keeping model used by Bitcoin.

It works similarly to cash transactions.

## Example

```
₹500

↓

Pay ₹100

↓

Receiver → ₹100

Sender → ₹400 (New UTXO)
```

## Key Points

- Bitcoin uses the UTXO model.
- The remaining balance becomes a new UTXO.
- UTXOs can be used in future transactions.

---

# 3. UTXO in Bitcoin

## Definition

Every Bitcoin transaction contains:

- Input = Bitcoins spent
- Output = Bitcoins received

The output becomes a new UTXO.

## Example

```
Input → 5 BTC

↓

Alice → 4 BTC

Bob → 1 BTC (Change UTXO)
```

## Advantages

- Prevents double spending
- Easy balance calculation
- Easy transaction validation
- Easy to trace Bitcoin history

## Balance Formula

```
Balance = Sum of all UTXOs
```

---

# 4. Proof of Work (PoW)

## Definition

Proof of Work (PoW) is the leader election consensus algorithm used in Bitcoin.

Miners compete to solve a cryptographic puzzle.

The first miner to solve it becomes the leader and creates the new block.

---

## Proof of Work Flow

```
Transactions

↓

Miners

↓

Solve Puzzle

↓

Leader Selected

↓

New Block

↓

Blockchain

↓

Bitcoin Reward
```

---

## Key Points

- Bitcoin uses Proof of Work.
- Miners solve cryptographic puzzles.
- The first miner to solve the puzzle wins.
- The winner receives a Bitcoin reward.

---

# 5. Cryptographic Puzzle

## Definition

A cryptographic puzzle requires miners to find a hash value that is below a predefined threshold.

---

## Mining Process

```
Block Header

↓

Hash

↓

Hash < Threshold ?

↓

No → Change Nonce

↓

Hash Again

↓

Yes → Publish Block
```

---

## Nonce

### Definition

A Nonce is a random number that miners repeatedly change until they generate a valid hash.

---

## Avalanche Effect

A very small change in the nonce produces a completely different hash value.

---

## Important Facts

- Average Bitcoin mining time = **10 minutes**
- Hard to solve
- Easy to verify
- This process is called **Proof of Work**

---

# Relationship Between Topics

```
Wallet

↓

Transaction

↓

Verification

↓

Memory Pool

↓

Miner Selects Transaction

↓

Proof of Work

↓

Cryptographic Puzzle

↓

Leader Selected

↓

New Block

↓

Blockchain

↓

UTXO Updated
```

---

# Important Definitions

## Memory Pool (Mempool)

Temporary storage area for verified transactions before they are added to a block.

---

## UTXO

Unspent Transaction Output used as Bitcoin's record-keeping model.

---

## Input

Bitcoins spent in a transaction.

---

## Output

Bitcoins received in a transaction.

---

## Proof of Work (PoW)

Consensus algorithm where miners solve cryptographic puzzles to create new blocks.

---

## Miner

A node that solves PoW puzzles and creates new blocks.

---

## Cryptographic Puzzle

A puzzle requiring miners to find a hash value below a given threshold.

---

## Nonce

A random number changed repeatedly until a valid hash is generated.

---

# Key Takeaways

- Transactions are temporarily stored in the Mempool.
- Bitcoin uses the UTXO model instead of account balances.
- Proof of Work selects the miner who creates the next block.
- Miners repeatedly change the nonce until a valid hash is found.
- The mining process keeps the Bitcoin network secure and prevents double spending.

---

# Summary

Bitcoin transactions are first verified and stored in the Memory Pool. Miners then select these transactions and compete using the Proof of Work algorithm to solve a cryptographic puzzle. The winning miner creates a new block, which is added to the blockchain, and the UTXO database is updated. This process ensures security, transparency, and decentralized trust in the Bitcoin network.