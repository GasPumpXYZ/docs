---
description: >-
  Our NFT standard has everything you need to build complex use cases on top of
  your digital assets.
---

# 📝 Robust NFT Standard

{% hint style="danger" %}
&#x20;**Deployed on Testnet:** Our contract is deployed on testnet and still has not been audited.&#x20;
{% endhint %}

## 🔌  Functionality

Our NFT contract has the following functionalities. We are designing functionality to be modular, that is key functionality is not required.&#x20;

{% hint style="info" %}
Not required functionality is denoted as _italicized._&#x20;
{% endhint %}

| Functionality               | Description                                                                                                                                                                                                                                                                                                                                    |
| --------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🖼️ NFT                     | Unique digital asset                                                                                                                                                                                                                                                                                                                           |
| 🔥 Burn                     | NFT can be discarded                                                                                                                                                                                                                                                                                                                           |
| :bell: Events               | Events emit a view function for others to understand changes that have happened regarding a NFT without constantly spending resources indexing a NFT checking for changes. This combined with flags can optimize an NFT indexer significantly by understand the nature of a NFT and optimizing for the type of behaviors that can be emitted.  |
| ⿵ Metadata                  | Metadata describes the accompanying information about a NFT usually pinned on a decentralized storage solution like Arweave or IPFS                                                                                                                                                                                                            |
| ⛳️ Flags                    | Flags are attributes that represent  values that allow indexers to understand the behavior of an NFT before spending extra bandwidth actually looking inside of a NFT's metadata. Examples of flags include, Rich Media, Dynamic, Non Transferability, Storage                                                                                 |
| _🥚 Evolution / Devolution_ | New NFTs, with cardinality 1 to 1, insterad of pieces-> whole and whole to pieces as defined in composability.  Instead of dynamic NFT this is new tokens.                                                                                                                                                                                     |
| _🧩  Composability_         | NFTs defined as "pieces" that can be rendered into a bigger "whole" set metadata render type. For more on composability.                                                                                                                                                                                                                       |
| _📚 Collection Mint_        | Minting a group of associated NFTs as opposed to a standalone 1 of 1                                                                                                                                                                                                                                                                           |
| _🪪 Update Authority_       | Whether NFT(s) can be updated and who can update them. Excluding update authority means NFT cannot be recovered or changed.                                                                                                                                                                                                                    |
| _🔐 Soul Bound_             | Soul bound                                                                                                                                                                                                                                                                                                                                     |
| _🏠 Renting_                | Allowing a NFT to have a use with an expiry date.                                                                                                                                                                                                                                                                                              |

## Learn More About All Functionality Here

{% content-ref url="composability.md" %}
[composability.md](composability.md)
{% endcontent-ref %}

{% content-ref url="soul-bound.md" %}
[soul-bound.md](soul-bound.md)
{% endcontent-ref %}

{% content-ref url="events.md" %}
[events.md](events.md)
{% endcontent-ref %}

{% content-ref url="flags.md" %}
[flags.md](flags.md)
{% endcontent-ref %}

{% content-ref url="update-authority.md" %}
[update-authority.md](update-authority.md)
{% endcontent-ref %}

{% content-ref url="collection-mint.md" %}
[collection-mint.md](collection-mint.md)
{% endcontent-ref %}

{% content-ref url="renting.md" %}
[renting.md](renting.md)
{% endcontent-ref %}

## Source Code

{% content-ref url="source-code.md" %}
[source-code.md](source-code.md)
{% endcontent-ref %}

