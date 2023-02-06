---
description: Reap the benefits of renting out a NFT without loosing custody
---

# 🏚 Renting

Renting a NFT denotes allowing another person to use a NFT while still retaining ownership.&#x20;

The main reason to standardize this is so marketplaces can properly display which NFTs are being rented out to faciliate rents within marketplaces. This may also affect evaluations as property indexing this information and have proper flags and events will capture hot property that may not otherwise be listed on the markets.



## High Level Overview

In our implementation each NFT can only 1 user set at a time can be set as a renter. If a NFT is transferred, renters are unaffected. However only the owner at that time can rent their NFT to a "user"&#x20;

{% hint style="info" %}
A **user** denotes someone **renting** a NFT.
{% endhint %}

## Specification

```rust
fn setUser (
    Token_id: string
    account_id: string
    expiry_date: uint64
)
```

* Sets the user address and when user expires
* Expires set as UNIX timestamp
* If a user is already a renter if a user is already added
* Should emit an error if not a valid token or expiry date (in the past)
* Emits user\_add event (see below)
* The user will automatically lose role after the expiry\_date
* Emits user\_add event is also emitted upon expiry

```json
// user_add event
{
    "standard": "fuelXXX",
    "event": "renter_is_added",
    "data": {owner_id, user.id, expiry}
}
```

```rust
fn user_of {
    token_id: string
} -> string
```

* The following function gets the user address of an NFT
* The zero address indicates that there is no user or the user is expired
* tokenId The NFT to get the user address for
* Return The user address for this NFT

```rust
fn user_expire {
    token_id: string
}-> u64
```

* Get the user expires of an NFT
* The zero value indicates that there is no user
* tokenId The NFT to get the user expires for
* Returns The user expiration date for this NFT

## Questions We Asked Ourselves

* How many people can rent 1 NFT?
* Should we separate out renting into a custodial proxy contract or should we mimic similar implementations as found on Ethereum?
* What happens when a a NFT is being rented and the owner sells the NFT? Should we prohibit transfers during rental periods
* Should all NFTs by default be rentable or should this be a setting? If it is a setting should it be update-able?

## Use Cases

* Renting in Game Assets
* Renting membership passes
* Real estate



## Other Inspirations
