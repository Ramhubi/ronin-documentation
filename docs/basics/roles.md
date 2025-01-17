---
title: Roles
description: Who are delegators, validators, and bridge operators, and what they do.
---

## Delegator

A delegator is an individual that delegates their stake to a validator and earns rewards in return. By delegating their stake, delegators can participate in the network and be rewarded without the technical expertise or resources required to run a validator node themselves.

### Stake RON

In Ronin, token holders can choose validators based on various factors such as the performance of the validators and their commission rate.

After choosing the validators, the RON holders can follow the steps in [Stake RON](./../delegators/onboarding/become-delegator.mdx).

## Validator

A validator is someone who runs a *validator node* on the Ronin chain to validate transactions and generate blocks.

### Validator categories

There are three categories of validators:

* **Validator Candidate.** After registering as a validator on Ronin, you'll become a Validator Candidate and have a chance to be selected as a Standard Validator on the next day.
* **Standard Validator.** Every day, 10 Validator Candidates with the highest amount staked are selected as Standard Validators. The system records your total staking amount at 00:00 UTC every day for the selection process.
* **Governing Validator.** The validators chosen by the community and Sky Mavis to ensure network security. Governing Validators are validators by default, and they account for more than half of the total validator pool.

### Become a validator

For instructions on becoming a validator, see [Register as a validator](./../validators/onboarding/become-validator.mdx).

### RON requirements for validators

Each Ronin validator is required to stake 250,000 RON.

### Validator selection

The validators are selected using Delegated Proof of Stake (DPoS). Beside the 12 Governing Validators, top 10 Validator Candidates with the highest staked amount are selected as Standard Validators.

### Validator responsibilities

Validators are in charge of the following:

* Generating blocks.
* Operating a validator node.
* Operating a governor (Governing Validators only).

#### Block generation

Whenever a block is generated, the next validator has to validate incoming transactions and generate a new block.

The block generated by the designated validator has a larger difficult weight. If the designated validator can not produce a block, the other validators generate a new block. In this case, that block has a smaller difficult weight. These difficult weights help nodes have additional facilities to reorganize in case the chain is forked.

#### Running a validator node

Validators operate a validator node and keep the node's software up to date.

#### Governance

Governing Validators can propose and vote for changes, such as adding or removing Governing Validators, upgrading smart contracts, and changing thresholds.

### Slashing rules

Validators who fail to fulfill their responsibilities are subject to [slashing](./../validators/slashing.mdx).

## Bridge operator

A bridge operator is someone who runs a *bridge operator node* to manage deposit and withdrawal events on Ronin Bridge. The purpose of Ronin Bridge is facilitating asset transfers between Ronin and other Ethereum Virtual Machine (EVM)-based chains. 

### Bridge operator responsibilities

Bridge operators are in charge of the following:

* Operating a bridge operator node.
* Governing Ronin Bridge.

#### Operating a bridge operator node

Bridge operators run a bridge operator node and keep the node's software up to date.

### Governance

Bridge operators can propose and vote on changes to Ronin Bridge, such as pausing the bridge and adding or removing other bridge operators.

### Slashing rules

Bridge operators who fail to fulfill their responsibilities are subject to [slashing](./../bridge-operators/slashing.md).