Module 14: Consensus in Permissioned Networks – Complete Summary

This module covers:

Practical Byzantine Fault Tolerance (PBFT)
RAFT Consensus
SmartBFT
Why Consensus in Permissioned Networks?

Permissioned blockchains have:

Known participants
No mining
Enterprise control

Consensus is needed to:

✅ Agree on transaction order

✅ Prevent conflicting transactions

✅ Maintain a single ledger state

✅ Handle faulty nodes

1. Practical Byzantine Fault Tolerance (PBFT)
Definition

PBFT is a voting-based consensus algorithm introduced by:

Barbara Liskov
Miguel Castro (1999)

It solves the Byzantine Generals Problem.

Features
Voting-based
Byzantine Fault Tolerant
No mining
Fast transaction finality
Energy efficient
Formula

Total nodes required:

Where:

N = Total Nodes
f = Faulty Nodes

Votes required:

PBFT Phases
1. Pre-Prepare

Leader proposes block.

2. Prepare

Nodes vote on block.

3. Commit

Block added to blockchain.

View Change

If leader fails:

Old Leader

↓

View Change

↓

New Leader
Variants
RBFT

Used in Hyperledger Indy.

IBFT

Used in Hyperledger Besu and Quorum.

SBFT

Improved performance version.

2. RAFT Consensus
Definition

RAFT is a leader-based consensus algorithm developed by:

Diego Ongaro
John Ousterhout
Three Components
Leader Election

Selects leader.

Log Replication

Copies data to followers.

Safety

Maintains consistency.

Node States
Follower

↓

Candidate

↓

Leader
Working
Step 1

All nodes start as Followers.

Step 2

Timeout occurs.

Step 3

Node becomes Candidate.

Step 4

Majority voting.

Step 5

Leader elected.

Step 6

Leader replicates logs.

Features

✅ Simple

✅ Fast

✅ Fault Tolerant

✅ Strong Consistency

✅ Used in Hyperledger Fabric

3. SmartBFT
Definition

SmartBFT is a Byzantine Fault Tolerant consensus mechanism used in Hyperledger Fabric.

Based on:

BFT-SMART Protocol
Components
Request Pool

Stores incoming transactions.

Block Assembler

Creates blocks.

Synchronization Mechanism

Keeps nodes synchronized.

Working
Client

↓

Request Pool

↓

Block Assembler

↓

Consensus

↓

Synchronization

↓

Ledger Update
Features

✅ Byzantine Fault Tolerance

✅ Handles malicious nodes

✅ Transaction Verification

✅ Block Creation

✅ Anti-Censorship Protection

Comparison of Consensus Algorithms
Feature	PBFT	RAFT	SmartBFT
Type	Voting-Based	Leader-Based	Byzantine Fault Tolerant
Mining	No	No	No
Handles Malicious Nodes	Yes	No	Yes
Handles Node Failures	Yes	Yes	Yes
Complexity	Medium	Simple	High
Performance	Good	High	Moderate
Hyperledger Usage	Some Projects	Fabric	Fabric