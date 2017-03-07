---
layout: post
published: true
title: Cryptocurrency - The Bitcoin Blockchain
category: Blog
tags: 
  - Cryptocurrency
  - Bitcoin
---

The blockchain lies at the heart of bitcoin. An agreed upon history of bitcoin. The blockchain is a chain of blocks, or a series of recorded transactions which build upon one another. Every time a transaction is made, it gets included in a block which is added into the chain.

What are we referring to when we say block? Simply, it's a bunch of data. Included in that data is a list of transactions and some information about the previous block. Also, there is a puzzle of sorts.

An important part of bitcoin is that a cryptographic puzzle must be solved for a block to be added to the chain. This is what miners are doing - trying to solve the cryptographic puzzle that will allow them to add a block to the chain. As a reward for solving the puzzle, they get fees provided by the users making the transactions included in the block. There is also a number of bitcoin awarded to the successful miner. This reward decreases over time and eventually will go to zero. At that point, there are no more bitcoins to be mined and all miner profit comes from the fees on transactions.

How hard is the puzzle? The puzzle varies in difficulty depending on miner consensus. Bitcoin is set up so that a block is mined every 10 minutes. Miners will agree on how difficult the puzzle should be by looking at how long it took to mine previous blocks.

== Blockchain.info ==

Let's look at an example on [blockchain.info](https://blockchain.info).

== Caveats ==

What if two miners solve the puzzle at the same time? Other miners will mine on a certain branch which could be either miner's, but once one chain gets longer than the other, miners work on that chain and that chain becomes the "official" chain.

What are some things to keep in mind as a user? A transaction is only valid when it exists in the blockchain. This means that you must wait for a transaction to last through multiple blocks so that you know it made it to the longest chain.

Why can't someone modify the history of the blockchain? The blocks contain information which verify information about the previous block. The puzzle makes it difficult 
