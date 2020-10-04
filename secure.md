---
layout: default
---
<br/>

# Securing your Bitcoin

### Table of Contents

1.  [Why secure your own bitcoin?](#why-secure-your-own-bitcoin)
2.  [Android?](#android)
3.  [iOS](#ios)
4.  [Other options](#other-options)
4.  [Backup](#backup)
5.  [Trade-offs](#trade-offs)


### Why secure your own bitcoin?

There goes a saying in Bitcoin, "not your keys, not your coins". What this essentially means is that, if you are not in control of your private keys (your recovery/seed words) then your are not in control of your bitcoin. Fortunately, if you are buying from a no-KYC source then you will almost certainly require your own wallet to conduct trades. From a privacy perspective if you do not control your own keys, for example if you have your bitcoin held with a custodian, then you essentially have zero privacy. Whoever controls those keys has the ability to not only see all of your funds, but spend them as they see fit.

[Here](https://www.bit-buy-bit.com/podcast-1/episode/26df4d37/ep35-bitcoin-podcast-with-itcoin-qa) is a podcast episode where I walk through in details the basics of bitcoin wallets.

### Android

1.  Download [Samourai Wallet](https://samouraiwallet.com/download)
2.  Select mainnet and enable tor
3.  Start new wallet
4.  Create a passphrase (*it is crucial that you secure this. Without this and your recovery words you cannot access your bitcoin*)
5.  Set a pin code
6.  Write down your recovery words (*it is crucial that you secure this backup. Without this and your passphrase you cannot access your bitcoin*)
7.  Tap the blue + and then press receive
8.  You will now see your first bitcoin address that you can receive to


### iOS

*Fully Noded requires your own node but is currently the only iOS wallet that offers coin control.*

1.  Download [Fully Noded](https://apps.apple.com/gb/app/fully-noded/id1436425586)
2.  Scan the connection QR provided by your node
3.  Press the Bitcoin logo followed by the + in the top corner 
4.  Select single sig
5.  Write down your recovery words (*it is crucial that you secure this. Without it you cannot access your bitcoin*)
7.  Press invoice
8.  You will now see your first bitcoin address that you can receive to


### Other options

- **Desktop Wallets**
  - [Bitcoin Core](https://bitcoincore.org/en/download/) (*has a built in node*)
  - [Specter Desktop](https://github.com/cryptoadvance/specter-desktop) (*requires your own node*)
  

### Backup 

Your bitcoin backup is your bitcoin. Anyone with access to it, has access to your bitcoin. Most people go for some form of [metal](https://jlopp.github.io/metal-bitcoin-storage-reviews/) storage.

You should ensure that your chosen method of backup is resistant to...

*  Theft/Loss
*  Fire/Water/Elements damage
*  Degredation
  
### Trade-offs

Unless your chosen wallet is backed by your own node, you are trusting someone elses. This means that your transactional data and wallet balances are being served by someone else, meaning they can theoretically eavesdrop on your on-chain activity. However, most users aren't likely to run a node **before** they even hold their own keys, the natural learning progression doesn't work that way. But dont panic, we will fix that in the next step!

Holding your own keys is a big responsibility, there are no refunds in Bitcoin.
  
  ***
  
  Now you know how to obtain secure privately, lets [segregate it](https://bitcoinprivacy.guide/coincontrol.html).
