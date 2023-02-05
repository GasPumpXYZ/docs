---
description: >-
  NFT Composability allows you to assemble NFTs into one and break them back
  down like puzzle pieces.
---

# 🧩 What is Composability?

## What Is & Isn't NFT Composability

Composaiblity in the context of NFTs is defined as NFTs that can be combined together and subsequently be broken down. This means when pieces are combined into a whole, the pieces cannot be used (transferred).&#x20;

In this case composability is not referring to being able to break up smart contract code into modular components.&#x20;

This is different a multitoken gated mint that allows a NFT to be minted by having "pre-requisite" NFTs. This is also different than 1 NFT acting a token gate for multiple token whitelists. The main difference here different NFTs are prerequisites for acquiring another rather that combining and disassembling NFTs.&#x20;

## :books: Terms

One might refer to NFTs that combine together into a bigger NFT as children, however we viewed the Children-Parent terminology not suitable as something that can be encompassed by something else doesn't mean it came from that bigger part, like a child does from a parent. So we are using the following terms

**Piece** and **whole**.

Something that is a a bunch of pieces can be made into whole and can also be a piece in a bigger whole.&#x20;

This is composability.&#x20;

## Types of Composability

* Layers: taking from existing assets&#x20;
* Predetermined outcomes: already existing whole assets uploaded that only point when "piece" conditions are met
* Request for Composition: where after composition and request for media file is made based on metadata conditions is passed in

## :thinking: Questions We Asked Ourself

* Should we define composability within a NFT or with a separate proxy contract? How does a NFT know if it belongs to something bigger?&#x20;
* Should we burn a NFT (how do we get it back), should we long piece NFT
* Should type of composability or the way something is rendered be defined on part or whole level?&#x20;
* Can metadata be dynamic for pieces and how will dynamic metadata for pieces effect the composition of whole NFTs?
* Can ownership of pieces still be used for token gated functionality? Does a user still own a piece when combined into a whole? Does ownership of a whole exists if peices have not been combined yet?
* Should the cardinality of composability only be Many->1, is 1->1  composability defined by something else like a evolving NFT? (Wouldn't be a dynamic NFT" because token-id would be different that a dynamic NFT which commonly denotes the same token's metadata changing.&#x20;

## Our Implementation

## Use Cases

For overall GasPump use cases

{% content-ref url="../../overview/our-features/use-cases.md" %}
[use-cases.md](../../overview/our-features/use-cases.md)
{% endcontent-ref %}



## Looking At Other Ecosystems

Metaplex Fusion (lucking the same dev who wrote this is working on this)

{% embed url="https://docs.metaplex.com/programs/fusion/" %}

Sui Capsules

Ethereum?

## Why?

There are certains things we left out but we decided that composability is essnetial must have. Learn more in the ideas page

{% content-ref url="../../overview/our-features/ideas.md" %}
[ideas.md](../../overview/our-features/ideas.md)
{% endcontent-ref %}

