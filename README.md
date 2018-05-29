Andromeda Project
================

[Zhang Wei](mailto:iam_zhang_wei@protonmail.com)

## What is Andromeda

Andromeda is a next generation platform for the development and distribution of applications on a blockchain. Andromeda has two layers, the economic layer, where the native currency (Perseus) lives, and an execution layer, where each smart contract has their own separated and independent blockchain.

## Why?

Andromeda has an ambitious goal, to make blockchain technology truly mainstream. In order to achieve that goal Andromeda allows _free_ interactions in the execution layer. The currency _Perseus_ is needed to create smart contracts but every interaction/function call is performed without the need of paying a _fee_ in the _Perseus_ currency, thus allowing developers to create applications that utilizes their blockchain as an append-only database for their applications, without requiring their users/customers to own or spend any _Perseus_.

## How?

Andromeda forked off the Ethereum go codebase, with two fundamental changes:

1. Each smart contract will start their own blockchain.
2. Each function call to a smart contract will be 'free'.

### Why having many blockchains?

Having a separated blockchain for each smart contract has advantages:

1. The main chain is smaller.
2. Each blockchain is well scoped
    1. Calculate the global state of smart contract is simpler and faster.z
    2. Busy/popular smart contracts will have longer chains, while the main chain growth at a predictable pace.

The blocks in the main chain will have references to the newest blocks created in the side chains. That means that the side chains are going to be secure through the main chain, simplifying things for consensus (which is happening only in the main chain).

![Blockchains](https://github.com/iam-zhang-wei/whitepaper/raw/master/graph-chains.png)

In the graphic we can see how the main chain consensus also secures all the sub chains. Because the blocks in the main chains are read only, a reference to newer blocks in the subchains are also read only.

### Free transactions

#### Preventing spam

Because interaction with smart contracts are free of charge, there should be a mechanism in place to prevent spamming the network. To prevent spam the client must perform a tiny proof of work calculation that must be included in the transaction. The PoW difficulty will be translated as gas by the miners.

#### How to incentive miners?

Miners should be economically incentive to process the _free_ transactions the same way do process transactions that pays a _fee_ (all transactions in the economic layers must pay a _fee_). In order to archive that, the miners can redeem the proof of work included in the free transactions. Think of it like the proof-of-work performed by the clients are coupons that the miners can redeem and for native currency that will be included in the block rewards (like a regular *fee*).

Thus, the interaction with the smart contracts are not free, the gas required to execute the smart contract is paid as proof of work.

### Why Ethereum?

It's a battle tested, mature project with a great community behind. I'm also happened to be a Golang/C developer myself.

I think Solidity is an OK language with an execution environment and I see there are many talented developers already.

## Donations

This is a part-time project right now, I need some donations in order to pause other work, so I can focus full time and work on Andromeda.

Every donation will be paid back with Perseus once the main net is launched. Do not send donations from exchanges or wallets where you don't own the private key.

This native currency will be minable, just like Ethereum, it will be premined to pay back the donations, the developer(s) behind the project won't have any Perseus unless they buy or mine it.

* Ethereum: 0xEb6235CCF2C52774af4C0fb3861b6c84f45d4EB8
* Bitcoin: 1zhangfnD6GZF5K5mzZ5Nt7mmXHBNzsCT
