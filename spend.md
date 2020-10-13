---
layout: default
---
<br/>

## Spending your Bitcoin

### Table of Contents

1.  [Spending considerations](#spending-considerations)
2.  [Android](#android)
3.  [iOS](#ios)

### Spending considerations

Spending your bitcoin can be a tricky task to get right from a privacy perspective. Fortunately if you have followed the previous steps you are in a perfect position to nail it. We have already covered off many of the pitfalls such as merging UTXOs, particularly those from 'conflicting' sources such as KYC and no-KYC but here is a breif rundown of things to consider when spending bitcoin (even to yourself).

* Check your labels before spending
* Avoid merging UTXOs where possible
* Label your change outputs
* Make every spend a coinjoin (*see below*)


### Android 

**Samourai Wallet Postmix Tools**

* Stonewall

Stonewall builds your transaction in a unique way to increase the deniability of links between the sender and recipient. Once the spending conditions are met the wallet will create this type of transaction automatically and will display the level of entropy the proposed transaction will have. Stonewall is actually a 'fake' mini coin join using only your own UTXOs. STONEWALL can be created from your deposit or postmix accounts, but the algorithm will never mix UTXOs from those accounts together.

**Useful for** - Any type of spend

* Stonewall X2

Stonewall X2 creates a mini coin join with another Samourai user. It mixes some of both Samourai users UTXOs when paying to any third party to create a high entropy transaction. You don't even need to be in the same room as your fellow Samourai user to create a Stonewall X2 as you can simply share QR codes via encrypted chat.

**Useful for** - Any type of spend

* Stowaway

Stowaway is Samourai's implementation of Payjoin. When paying another trusted Samourai user it creates a transaction that looks just like any other Bitcoin transaction on chain but it's actually a form of mini coin join. The most powerful thing about Stowaway is that the amount being sent will never actually be visible to anyone looking at the blockchain. Stowaway also uses sender AND recipient UTXOs on the input side of the transaction which completely destroys the common-input ownership heuristic for chain analysis firms. Just like Stonewall X2, Stowaway can be constructed in person or remotely.

**Useful for** - Spending to another Samourai user


* Ricochet

Ricochet creates additional 'hops' or 'distance' between your Samourai wallet activity and the recipient address. This can be beneficial if you are sending to a service such as an exchange who may want to pry into the history of your UTXO’s.

**Useful for** - Spending to centralised entities that may be using chain analysis


### iOS

There are currently no iOS wallets that have privacy preserving spend tools. This section will be updated if that changes. 

Recommended course of action is to follow the basic steps outlined [here](#spending-considerations). 

Or...

* Buy a cheap android phone
* Install Samourai Wallet
* Follow steps above
  
  ***
  
Now you have obtained, secured, segregated, labelled and coinjoined your bitcoin into both mobile and hardware wallets that are backed by your own node and learned how to spend in a privacy focused way. Let's look at some of the [supplementary](https://bitcoinprivacy.guide/supplementary.html) tools available to further lock down your Bitcoin related privacy.
