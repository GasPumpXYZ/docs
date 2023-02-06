---
description: Ability to mint a group of related NFTs
---

# 📂 Collection Mint

In our implementation for collections mint indiivudla NFTs are nested within. There will be a mint function. Mint order can be randomized or set in a sequential order

A colection has the following fields that must be defined

* Collection name
* Collection description
* Number of tokens

In this first rendition the number of tokens are set and cannot be changed. If a changing qunaity of a NFT collection is needed (for example, an artist adding to a collection over time) this can be set in the next version of GasPump's standard.&#x20;

* From mint page, define collection functions&#x20;
* Whitelist: only predefined list of addresses can mint. Whitelist authority, ability fo whitelist admin(s) to update list -> Can be configured based on token holder proxy contract for token gated mints.
* Mint all to address
* Mint to address list (maybe custom for this)
* Require payment for mint
