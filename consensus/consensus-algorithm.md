---
description: Quick overview of consensus algorithms
---

# Consensus algorithm

## Basic definition

Blockchains face 3 main types of problems:

1. **Correctness** \(ability to make the difference between a correct and fraudulent transaction, to guarantee the transaction really comes from where it claims to be\)
2. **Agreement** \(maintaining a global truth\)
3. **Utility** \(the system has to be useful, minimize latency\)

If you think of a blockchain as a data storage and management application on top of a peer-to-peer like technology, it becomes clear real quick that the method that adds a block to the blockchain without compromising data integrity is a key component to the blockchain and it’s security. This method is called a consensus algorithm.

{% hint style="info" %}
A consensus algorithm can be seen as a verification and validation protocol in the absence of an administrator. Its purpose it to bring all nodes in agreement in an environment where nodes don’t know and don’t trust each other.
{% endhint %}

## Core properties

Core problem of multi-agent systems: a number of agents of the system need to reach an agreement on some value.

Since agents may fail or lie, a consensus protocol has to be fault tolerant.

1. Termination \(at some point each correct cides on a value\);
2. Integrity \(correct agents answer correct vaues\);
3. Agreement \(every correct agent must agree on the same value\)

## Consensus algorithm families

{% page-ref page="proof-of-work-pow/" %}

{% page-ref page="proof-of-weight-powe/" %}

{% page-ref page="../practical-byzantine-fault-tolerance-pbft/" %}

{% page-ref page="../snow-protocol/" %}

{% page-ref page="../proof-of-stake-pos/" %}

{% page-ref page="../proof-of-history-poh/" %}

{% page-ref page="../proof-of-capacity-proof-of-space/" %}

{% page-ref page="../proof-of-authority-poa/" %}



## Comparison



| Algorithm | Snow | Proof-of-Weight | Byzantine | Proof-of-Stake |
| :--- | :--- | :--- | :--- | :--- |
| Project | Avalanche | Algorand | Tendermint |  |
| Permissioned | Hybrid | No |  |  |
| Leaderless |  | No |  |  |
| Committee \(size\) |  | Yes \(1,000\) |  |  |
| Max block size \(MB\) |  | 1 |  |  |
| Transaction per second |  | 1,200  |  |  |
| Instant finality |  | Yes |  |  |
| Block time \(seconds\) |  | 5 |  |  |
| Sybil attacks |  | OK \(up to 2/3\) |  |  |
| DDoS |  | OK |  |  |
| Network partitioning |  | OK |  |  |
| Incentivization |  |  |  |  |
| Censorship resilient |  |  |  |  |
| Liveness |  |  |  |  |
| Selective censorship |  |  |  |  |
| Poisoning threshold |  |  |  |  |
| Objective/Subjective | Subjective |  |  |  |

