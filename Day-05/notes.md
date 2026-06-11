# Day 05 - Transaction Flow

## Overview

This module explains how transactions are processed in traditional banking systems and blockchain networks. It also introduces the concept of **Consensus**, which helps maintain a single secure blockchain and prevents double spending.

---

# 1. Transaction Flow in Traditional Systems

## Definition

In a traditional banking system, a **Bank** acts as a trusted third party between the sender and the receiver.

### Example

Alice wants to send money to Bob.

```
Alice
   │
   ▼
Bank (Central Authority)
   │
Verification
Balance Check
Ledger Update
   │
   ▼
Bob
```

### Steps

1. Alice sends a transaction request.
2. Bank verifies Alice's identity.
3. Bank checks the account balance.
4. Bank updates the centralized ledger.
5. Bob receives the money.

### Characteristics

- Centralized Ledger
- Trusted Third Party
- Bank controls all transactions
- Prevents double spending
- Single Point of Failure

---

# 2. Transaction Flow in Blockchain Networks

## Definition

Blockchain transactions occur without a bank or central authority.

Instead, **network nodes verify and approve transactions**.

### Transaction Flow

```
Alice
   │
Create Transaction
   │
Sign with Private Key
   │
Broadcast to Network
   │
Nodes Verify
   │
Consensus
   │
Block Created
   │
Added to Blockchain
   │
Bob Receives Funds
```

### Steps

1. Alice creates a transaction.
2. Alice signs it using her Private Key.
3. Transaction is broadcast to all blockchain nodes.
4. Nodes verify the transaction.
5. Consensus is achieved.
6. Verified transactions are grouped into a block.
7. Block is added to the blockchain.
8. Bob receives the funds.

### Advantages

- Decentralized
- Secure
- Transparent
- Immutable
- No trusted third party required

---

# 3. Need for Consensus

## Definition

Consensus is the process by which blockchain nodes agree on which block should be added next.

### Simple Meaning

Consensus = Agreement among all nodes.

---

## Why is Consensus Needed?

Suppose a blockchain already contains:

**99 Blocks**

Every node receives new transactions and creates its own candidate block.

```
Node A → Block 100A

Node B → Block 100B

Node C → Block 100C
```

If every node adds its own block:

❌ Multiple blockchain versions will exist.

Consensus selects only **one winning block**.

---

## Consensus Process

```
Transactions

↓

Candidate Blocks

↓

Consensus

↓

Winning Block

↓

Added to Blockchain

↓

All Nodes Update
```

---

## Importance of Consensus

- Prevents multiple blockchain versions
- Prevents double spending
- Maintains consistency
- Selects one winning block
- Creates trust without a central authority

---

# 4. Types of Consensus

## A. Voting-Based Consensus

### Definition

Nodes vote to decide the next valid block.

### Characteristics

- Uses signed votes
- Less computationally intensive
- Common in Private/Permissioned Blockchains

### Examples

- PBFT (Practical Byzantine Fault Tolerance)
- RAFT

---

## B. Lottery-Based Consensus

### Definition

Nodes compete in a lottery-like process to become the leader.

### Characteristics

- Chance-based selection
- Common in Public/Permissionless Blockchains

### Examples

- Proof of Work (PoW)
- Proof of Stake (PoS)

---

# Voting-Based vs Lottery-Based Consensus

| Voting-Based | Lottery-Based |
|-------------|--------------|
| Uses voting | Uses lottery |
| Private blockchain | Public blockchain |
| PBFT, RAFT | PoW, PoS |
| Less computation | Competitive selection |

---

# Important Definitions

## Transaction

A message requesting an operation on the blockchain.

## Consensus

Agreement among blockchain nodes about the next valid block.

## Candidate Block

A proposed block created by a node.

## Winning Block

The block selected through consensus.

## Voting-Based Consensus

Consensus achieved through voting among nodes.

## Lottery-Based Consensus

Consensus achieved through chance-based leader selection.

---

# Key Takeaways

- Traditional systems rely on a bank to verify transactions.
- Blockchain networks use decentralized nodes instead of a central authority.
- Consensus ensures that every node agrees on the same valid block.
- Consensus prevents double spending and maintains a single, secure blockchain.
- Voting-based consensus is common in private blockchains, while lottery-based consensus is widely used in public blockchains.

---

# Summary

Blockchain transaction flow removes the need for intermediaries by allowing network nodes to verify transactions. Consensus mechanisms ensure that only one valid block is added to the blockchain, maintaining security, consistency, and trust across the decentralized network.