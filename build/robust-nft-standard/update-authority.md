---
description: The who's your daddy of NFTs
---

# 👮 Update Authority

Update Authority is defined as who is allowed to update a NFT. In the case of the ⛽️ GasPump standard there could be Update Authority for the follwing robust NFT features

* Soul Bound Revocability: who is allowed to take a SBT back
* Metadata: who can change the metadata of a "dynamic" NFT

As part of of the standard their is a update\_authority view function for transparency that lets you know which address / smart contract is responsible for updating a NFT, and what can be udpated.

```rust
// snippet code of update authority function

fn view_udpate_authority( token id) {
} -> return ..... some list

```

* view function of who can update?
