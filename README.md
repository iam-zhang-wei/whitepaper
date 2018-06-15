Andromeda Project
=================

[Zhang Wei](mailto:iam_zhang_wei@protonmail.com)


## Introduction

Cryptocurrency and smart contracts are changing the world economy. From a currency perspective, what was previously impossible in most of the world – transferring money globally in an instant – is now not only possible, it’s safe, fast, easy and almost frictionless.

We want to create a cryptocurrency that is useful for all people for day-to-day usage. A system that can allow non-technical users to be easily be a part of the new digital money world. Our goal and principle is to keep things simple and easy with value for everybody.

### Goals

* Create a brand new blockchain with smart contract capabilities
* The blockchain aims mass adoption by allowing free transactions with smart contracts.
* The network supports Masternodes to make things faster to process.

### Executive Summary

Andromeda is a standalone blockchain with smart contract support. It's built upon an improved Etherereum codebase which improves capacity and introduces _free_ smart contracts interactions. Users in the Andromeda network does not need ownership of the native coin (Perseus) in order to interact with existing smart contracts, making smart contract open and free for anyone to interact.

In order to improve speed Andromeda will have masternodes. A masternode is a primary node in the network that will not only relay transactions (making it safe to trust unconfirmed transactions).

Hosting a masternode will generate additional Perseus for its owner. The amount of Perseus to receive will vary due the current number of masternodes online on the network and their daily uptime.

Anybody can run a masternode! The pre-requisites are:
 * 10,000 Perseus
 * Static Public IP Address

The pre-requisites may change in the future when the community voting system (a dApp) is finished and implemented. After the voting system is implemented, the number of Perseus needed as collateral to run a masternode will be decided by the community. The voting mechanism is intended to be added so that anyone with at least 1 Perseus can vote.
    
### Specification

 * Algorithm: Ethash
 * Time between blocks: 13 sec
 * Total block reward: 12 Perseus
 * Miner reward: 10 Perseus / Block (plus all the transaction fees)
 * Masternode reward: 2 Perseus/ Block

## Implementation

Andromeda is based on the Ethereum codebase with masternodes and the ability to interact _freely_ with smart contracts.

### What is _free_?

Any interaction with smart contract costs 0 Perseus and does not requires that the address owns any Perseus, thus, giving the freedom to anyone to interact with smartcontract with the ultimate goal of making blockchain and decentralized application truly mainstream.

It will be possible to create ERC-20 tokens in the Andromeda network and addresses and the token holders won't need to own any Perseus to pay for the 'gas'.

### What is not free?

Any activity in the economic layer requires a fee that is paid in Perseus. Moving funds (Perseus) from one address to another and creating a smart contract in the network also pays a fee in Perseus.

### Preventing spam

Interacting with a smart contract is not necessarily     free, to avoid spam attacks a Andromeda has a throttle mechanism in place. Each transaction with a smart contract must include a tiny Proof-of-Work. A proof of work is a piece of data which is difficult (costly, time-consuming) to produce but easy for others to verify and which satisfies certain requirements. Producing a proof of work can be a random process with low probability so that a lot of trial and error is required on average before a valid proof of work is generated.

The proof-of-work required to interact with smart contract in the Andromeda network would take a modern CPU 10 to 20 seconds to calculate.

Alternately the user may decide to pay the 'gas' price in Perseus to avoid performing the PoW.

### Incentivizing miners to process _free_ transactions

Miners must be economically incentive to process the _free_ transactions the same way do process transactions that pays a _fee_. In order to archive that, the miners can redeem the proof of work included in the free transactions and convert them in Perseus. The more _free_ transaction miners includes in a block, higher the block reward they take.


## Roadmap

 * Q4 2018: Test-network launch
   This testing blockchain will be used for testing mining, wallets and tuning the PoW algorithms (For the _Free_ transactions).
 * Q1 2019: Main-net launch.
 * Q2 2019: Launch the voting dApp to let everyone decide the future of Andromeda.
