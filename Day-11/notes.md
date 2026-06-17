# Day 11 - Ethereum Virtual Machine (EVM)

## Overview

This module explains the Ethereum Virtual Machine (EVM), Ethereum Accounts, Ether (ETH), Gas, and the Account Balance Model used by Ethereum.

---

# 1. Ethereum Virtual Machine (EVM)

## Definition

The Ethereum Virtual Machine (EVM) is the runtime environment that executes Smart Contracts and processes transactions on the Ethereum blockchain.

---

## Working

```
User

↓

Digitally Signed Transaction

↓

Ethereum Network

↓

Ethereum Virtual Machine (EVM)

↓

Execute Smart Contract

↓

Blockchain Updated
```

---

## Functions of EVM

- Executes Smart Contracts
- Processes Transactions
- Creates Blocks
- Provides an Abstraction Layer
- Maintains Network Consistency

---

## Important Points

- Runtime environment for Ethereum
- Smart Contracts reside inside the EVM
- Executes verified transactions
- Creates abstraction between code and hardware

---

# 2. Ethereum Accounts

## Definition

An Ethereum Account stores ETH and allows users or smart contracts to perform transactions.

---

## Types of Accounts

### A) Externally Owned Account (EOA)

**Controlled By:** User

### Features

- Controlled using a Private Key
- No Smart Contract Code
- No Creation Cost
- Used by normal users

---

### B) Contract Account

**Controlled By:** Smart Contract Code

### Features

- Contains Smart Contract Code
- Requires Creation Cost
- Executes automatically when triggered

---

# Comparison of Accounts

| Externally Owned Account (EOA) | Contract Account |
|-------------------------------|------------------|
| User Controlled | Contract Controlled |
| Uses Private Key | Uses Smart Contract Code |
| No Creation Cost | Creation Cost Required |
| No Contract Code | Has Contract Code |

---

## Both Account Types Can

- Receive ETH
- Hold ETH and Tokens
- Send ETH
- Interact with Smart Contracts

---

# 3. Ether (ETH)

## Definition

Ether (ETH) is the native cryptocurrency of the Ethereum network.

---

## Uses of Ether

- Transaction Fees
- Smart Contract Execution
- Digital Payments

---

# Ether Denominations

| Unit | Value |
|---------|----------------|
| Wei | 1 |
| Kwei | 10³ Wei |
| Mwei | 10⁶ Wei |
| Gwei | 10⁹ Wei |
| Microether (Szabo) | 10¹² Wei |
| Milliether (Finney) | 10¹⁵ Wei |
| Ether | 10¹⁸ Wei |

---

## Important Formula

```
1 ETH = 10¹⁸ Wei
```

---

# 4. Gas

## Definition

Gas measures the computational work required to execute transactions and smart contracts.

Gas is often called the **Fuel of Ethereum**.

---

## Why Gas is Required

- Pays for computation
- Prevents infinite execution
- Protects the network from spam

---

## Standard ETH Transfer

```
Gas Limit = 21,000
```

---

# Old Transaction Fee Formula

```
Transaction Fee

=

Gas Limit × Gas Price
```

---

# New Fee Formula (London Upgrade)

```
Transaction Fee

=

Gas Limit × (Base Fee + Tip)
```

---

## Base Fee

- Minimum network fee
- Burned (Destroyed)

---

## Tip (Priority Fee)

- Paid to Validators
- Encourages faster transaction processing

---

# Gas Flow

```
User

↓

Gas Limit

↓

(Base Fee + Tip)

↓

Validator

↓

Base Fee Burned

↓

Tip Received
```

---

# 5. Account Balance Model

## Definition

Ethereum uses the **Account Balance Model** instead of Bitcoin's UTXO model.

---

# Record Keeping Models

### Bitcoin

UTXO Model

### Ethereum

Account Balance Model

---

# Working

A transaction is valid only if the sender has sufficient balance.

```
Sender

↓

Debit

↓

Receiver

↓

Credit

↓

Global State Updated
```

---

# Global State Stores

- Account Balance
- Smart Contract Code
- Internal Storage

---

# Benefits

## Simplicity

Easy to develop Smart Contracts.

---

## Efficiency

Only the sender's balance needs to be verified.

---

# UTXO vs Account Balance Model

| UTXO Model | Account Balance Model |
|------------|----------------------|
| Bitcoin | Ethereum |
| Inputs & Outputs | Debit & Credit |
| More Complex | Simpler |
| Balance = Sum of UTXOs | Direct Balance Stored |

---

# Complete Module Flow

```
Ethereum

↓

Ethereum Virtual Machine (EVM)

↓

Smart Contracts

↓

Ethereum Accounts

├── Externally Owned Account (EOA)

└── Contract Account

↓

Ether (ETH)

↓

Gas

↓

Gas Limit

↓

(Base Fee + Tip)

↓

Transaction

↓

Account Balance Model

↓

Debit Sender

↓

Credit Receiver

↓

Global State Updated
```

---

# Important Definitions

## Ethereum Virtual Machine (EVM)

Runtime environment that executes Smart Contracts.

---

## Externally Owned Account (EOA)

User-controlled account secured by a private key.

---

## Contract Account

Account controlled by Smart Contract code.

---

## Ether (ETH)

Native cryptocurrency of Ethereum.

---

## Wei

Smallest unit of Ether.

```
1 ETH = 10¹⁸ Wei
```

---

## Gas

Computational cost required to execute transactions.

---

## Base Fee

Minimum fee burned by the network.

---

## Tip (Priority Fee)

Fee paid to validators for faster transaction processing.

---

## Account Balance Model

Ethereum's record-keeping model using direct debit and credit.

---

# Key Takeaways

- EVM is the execution engine of Ethereum.
- Ethereum supports two account types: EOA and Contract Accounts.
- Ether (ETH) is used for transactions and Smart Contract execution.
- Gas prevents spam and pays for computation.
- Ethereum uses the Account Balance Model, making transaction processing simpler than Bitcoin's UTXO model.

---

# Summary

The Ethereum Virtual Machine (EVM) is the core execution environment of Ethereum, responsible for running Smart Contracts and processing transactions. Ethereum accounts store and transfer Ether (ETH), while Gas measures computational costs and secures the network. Unlike Bitcoin's UTXO model, Ethereum uses an Account Balance Model, making Smart Contract development and transaction management more efficient.