# Day 04 - Designing a Decentralized Communication

## Overview

This module explains how users securely communicate and perform transactions in a blockchain network using:

- Private Keys
- Public Keys
- Blockchain Addresses
- Wallets
- Digital Signatures

These technologies ensure security, ownership, and trust in blockchain systems.

---

# 1. Introduction

A **transaction** is a message sent to the blockchain network.

## Types of Transactions

- Asset Records
- Payment Details
- Property Agreements

### Traditional System

- Uses a centralized ledger
- Controlled by a single authority

### Blockchain System

- Uses a distributed ledger
- Every participant maintains a copy
- Consensus prevents double spending
- Transactions become immutable after recording

---

# 2. Keys to Interact

Blockchain uses two cryptographic keys.

## Private Key

### Definition

A secret key used to authorize and sign transactions.

### Characteristics

- Similar to a bank account password
- 256-bit number in Bitcoin
- Must never be shared
- Used to create digital signatures

---

## Public Key

### Definition

A key generated from the private key using Elliptic Curve Cryptography (ECC).

### Characteristics

- Similar to a bank account number
- Safe to share
- Used to verify digital signatures

---

## Key Generation

Private Key

↓

ECC Algorithm

↓

Public Key

---

# 3. Blockchain Address

## Definition

A Blockchain Address is a unique identifier used to send and receive cryptocurrency transactions.

It works like a bank account number.

---

## Address Generation

Private Key

↓

Public Key

↓

Hashing

↓

Blockchain Address

---

## A Transaction Contains

- From Address
- To Address
- Value
- Transaction Hash

### Note

Transaction hashes are later combined into a **Merkle Tree** to generate the **Merkle Root**.

---

# 4. Safeguarding Wallets

## Blockchain Wallet

A Blockchain Wallet stores and manages:

- Private Keys
- Public Keys
- Account Balance

### Important Point

There is **no "Forgot Private Key" option**.

If the private key is lost, access to the account is permanently lost.

---

## Types of Wallets

### Hot Wallets (Online)

- Web Wallet (MetaMask, MyEtherWallet)
- Desktop Wallet (Exodus, Bitcoin Core)
- Mobile Wallet (Trust Wallet)

### Advantages

- Easy to use
- Fast access
- Convenient for daily transactions

---

### Cold Wallets (Offline)

- Hardware Wallet (Ledger Nano S, Trezor)
- Paper Wallet

### Advantages

- Higher security
- Better protection against hackers

---

## Hot Wallet vs Cold Wallet

| Hot Wallet | Cold Wallet |
|------------|------------|
| Online | Offline |
| Convenient | More Secure |
| Faster Access | Better Protection |

---

# 5. Digital Signature – Trust Layer

## Definition

A Digital Signature is a cryptographic proof that verifies the authenticity and ownership of a transaction.

It ensures that the transaction was created by the legitimate owner.

---

## Blockchain Trust Factors

Blockchain provides four important trust factors:

- Identity
- Ownership
- Security
- Verification

Because of these features, Blockchain is known as a **Trust Machine**.

---

## Transaction Process

Alice Creates Transaction

↓

Signs with Private Key

↓

Digital Signature Created

↓

Sends Transaction + Public Key

↓

Network/Bob Verifies using Public Key

↓

Transaction Accepted

---

## Remember

### Private Key

Creates the Digital Signature.

### Public Key

Verifies the Digital Signature.

---

## Bitcoin Digital Signature Algorithm

Bitcoin uses:

**ECDSA (Elliptic Curve Digital Signature Algorithm)**

to create and verify digital signatures.

---

# Important Definitions

## Transaction

A message sent to the blockchain network.

## Private Key

A secret key used to authorize and sign transactions.

## Public Key

A key generated from the private key and used for verification.

## Blockchain Address

A unique address used to send and receive transactions.

## Blockchain Wallet

Software or hardware used to store and manage private keys.

## Digital Signature

Cryptographic proof of authenticity and ownership.

## ECDSA

Elliptic Curve Digital Signature Algorithm used in Bitcoin.

---

# Summary

Blockchain enables secure communication using cryptographic keys and digital signatures. A private key signs transactions, while a public key verifies them. Blockchain wallets securely store keys, and blockchain addresses allow users to send and receive transactions. These mechanisms provide security, ownership, authenticity, and trust in decentralized networks.