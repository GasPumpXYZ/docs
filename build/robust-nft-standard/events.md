---
description: Blockchains be talking back
---

# 🔔 Events

Events are defined as JSON outputs emitted when certain state is changed within a NFT onto the the block explorer

## Types of Events Supported

| Event Name            | When                                         | JSON Format                                                                                                                                                                                                                        |
| --------------------- | -------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| nft\_metadata\_update | when NFT metadata for dynamic nft is udpated | <p>{</p><p>      newURI: URI</p><p>      tokenID: fuel token ID</p><p>      time: UNIX timestamp</p><p>      updateAuthority: fuelAddress</p><p></p><p>}</p>                                                                       |
| nft\_sbt\_revoke      | when an update authority revokes someone nft | <p>{</p><p>      revoker: fuelAddress</p><p>      priorOwner: fuelAddress</p><p>      time: UNIX timestamp</p><p>      newOwner: fuelAddress</p><p></p><p>}</p>                                                                    |
| nft\_assemble         | when nfts pieces composed together           | <p>{</p><p>      composabilityType: ENUM</p><p>      piecesAddress: fuel token IDs</p><p>      time: UNIX timestamp</p><p>      wholeTokenID: fuel token ID</p><p>}</p>                                                            |
| nft\_dissasemble      | when NFT whole is decomposed into pieces     | <p>{</p><p>      composabilityType: ENUM</p><p>      piecesAddress: fuel token IDs</p><p>      time: UNIX timestamp</p><p>      wholeTokenID: fuel token ID</p><p>}</p>                                                            |
| nft\_burn             | when a NFT token is discared                 | <p>{</p><p>      owner: fuelAddress</p><p>      user: fuelAddress</p><p>      tokenID: fuel token ID</p><p>      expiryDate: UNIX timestamp</p><p>      paymentAmount: {optional} - probably should be included</p><p></p><p>}</p> |
| nft\_rented           |                                              | <p>{</p><p>      owner: fuelAddress</p><p>      user: fuelAddress</p><p>      tokenID: fuel token ID</p><p>      expiryDate: UNIX timestamp</p><p>      paymentAmount: {optional} - probably should be included</p><p></p><p>}</p> |
| nft\_rent\_expired    | when NFT expiration date is reached          | <p>{</p><p>      user: fuelAddress</p><p>      tokenID: fuel token ID</p><p>      expiryDate: UNIX timestamp</p><p>}</p>                                                                                                           |
| nft\_evolved          | when a NFT token evolves into new token      | <p>{</p><p>      user: fuelAddress</p><p>      formerTokenID: fuel token ID</p><p>      newTokenID: fueltokenID</p><p>      proxyContract: contractAddress</p><p></p><p>} </p>                                                     |
| nft\_opened           | When unlockable content is redeemed          | <p>{</p><p>      redeemer: userAddress</p><p>      tokenID: fuel token ID</p><p>} </p>                                                                                                                                             |

{% hint style="info" %}
Explain how rent expiry event will be emitted
{% endhint %}
