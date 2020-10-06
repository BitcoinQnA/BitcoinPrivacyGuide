---
layout: default
---
<br/>

# Segregating your Bitcoin

### Table of Contents

1.  [What is segregation?](#what-is-segregation)
2.  [Address re-use](#address-re-use)
3.  [Android](#android)
4.  [iOS](#ios)
5.  [Trade-offs](#trade-offs)


### What is segregation?

By segregation I simply mean having the ability to keep your different 'chunks' of bitcoin separate from one another. Why would we want to do this? Let's imagine that your wallet holds 1 BTC split between 2 UTXOs that are 0.5 BTC each and you want to send me 0.6 BTC. This transaction would result in your wallet combining those two UTXO's together to create an output that pays me 0.6 BTC and you would have a change output of around 0.4 BTC less any fees. 

So what I hear you say! Well now lets imagine that one of your 0.5 BTC was a change output from a 'frowned upon' service or source and the person you're paying is a regulated entity that is actively perfomring chain analysis. They could refuse access to their service, block your account or even report you to the authorities. This is just one example designed to demonstrate that one transaction could leak a lot of information about you and your transactional history, not good for your privacy!

So how do we mitigate against such a privacy leak? By using a [wallet](https://bitcoinprivacy.guide/secure.html) that offers coin control and labelling. Coin cointrol is a simply the ability to select which UTXOs are used to construct any given transaction. Ensuring that your UTXO's are effectively labelled will enable you to decide which UTXOs you want to include in future transactions. You can label any way you'd like but it is generally good practice to include the source of the funds in a format that suits you.

Sadly, there are very few mobile wallets that offer this functionality and you should bear this in mind when using a wallet without coin control. Desktop wallets like [Specter](https://github.com/cryptoadvance/specter-desktop) or [Bitcoin Core](https://bitcoin.org/en/download) generally offer more in this regard but are obviously not a portable solution. 

### Address re-use

99% of bitcoin wallets that exist today will automatically serve you a new receive address every time the previous one receives any funds. All you need to be aware of is not sharing the same one twice with different entities as you can leak some privacy for the same reason as outlined in the example above. Remember, addresses are free and infinite.

### Android

#### Samourai - Coin Control

1.  Press the 3 dots in the top right corner
2.  Show unspent outputs
3.  Long press on the UTXO(s) you want to use to create the transaction
4.  Press the send arrow in the top right
5.  Enter the recipient address and amount
6.  Send

#### Samourai - Labelling

1.  Press the 3 dots in the top right corner
2.  Show unspent outputs
3.  Double tap the UTXO(s) you want to label
4.  Press add note

### iOS

#### Fully Noded - Coin Control

1.  Tap the active wallet tab
2.  Tap the "utxo's" button
3.  Tap a utxo(s) to select it for a spend
4.  Tap the 🔗 button to create the transaction
5.  Enter the amount
6.  FN will check if you have an address copied to cliplboard, if not you can scan a QR to select the recipient address
7.  Send

#### Fully Noded - Labelling

*FN does labelling via addresses and not UTXOs so you should avoid address manual address reuse* 

1.  Tap the active wallet tab
2.  Press advanced
3.  Hit import address
4.  You can now add or overwrite and address label
  
### Trade-offs

The only real tradeoff with labelling your UTXO's and practicing coin control is the minimal extra steps required to do each one. Just remember, if you do not specify which UTXO's to spend in a transaction, your wallet will do it for you with no regard for each chunk of bitcoins previous history.

  
  ***
  
  Now you have obtained, secured, segregated and labelled your bitcoin to maximise your privacy, lets work on [scrutinising](https://bitcoinprivacy.guide/scrutinise.html) your transactions.
