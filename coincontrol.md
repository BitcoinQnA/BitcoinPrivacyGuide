---
layout: default
---
<br/>

# Segregating your Bitcoin

### Table of Contents

1.  [What is segregation?](#what-is-segregation)
2.  [Coin control](#coin-control)
3.  [Labelling](#labelling)
4.  [Trade-offs](#trade-offs)


### What is segregation?

By segregation I simply mean having the ability to keep your different 'chunks' of bitcoin separate from one another. Why would we want to do this? Let's imagine that your wallet holds 1 BTC split between 2 UTXOs that are 0.5 BTC each and you want to send me 0.6 BTC. This transaction would result in your wallet combining those two UTXO's together to create an output that pays me 0.6 BTC and you would have a change output of around 0.4 BTC less any fees. 

So what I hear you say! Well now lets imagine that one of your 0.5 BTC was a change output from a 'frowned upon' service or source and the person you're paying is a regulated entity that is actively perfomring chain analysis. They could refuse access to their service, block your account or even report you to the authorities. This is just one example designed to demonstrate that one transaction could leak a lot of information about you and your transactional history, not good for your privacy!

So how to we mitigate against such a privacy leak? By using a [wallet](https://bitcoinprivacy.guide/secure.html) that offers coin control and labelling. Coin cointrol is a simply the ability to select which UTXOs are used to construct any given transaction. Ensuring that your UTXO's are effectively labelled will enable you to decide which UTXOs you want to include in future transactions based. You can label any way you'd like but it is generally good practice to include the source of the funds somehow.

Sadly, there are very few mobile wallets that offer this functionality and those without it should be used with caution if you value your transactional privacy. Desktop wallets generally offer more in this regard but come with their own tradeoffs.

### Coin control

#### Samourai

1.  Press the 3 dots in the top right corner
2.  Show unspent outputs
3.  Long press on the UTXO(s) you want to use to create the transaction
4.  Press the send arrow in the top right
5.  Enter the recipient address and amount
6.  Send

#### Fully Noded

**INSERT FN INSTRUCTIONS**



### Labelling

#### Samourai

1.  Press the 3 dots in the top right corner
2.  Show unspent outputs
3.  Double tap the UTXO(s) you want to label
4.  Press add note

#### Fully Noded

**INSERT FN INSTRUCTIONS**
  
### Trade-offs

  
  ***
  
  Now you have obtained, secured, segregated and labelled your bitcoin to maximise your privacy, lets [scrutinise it](https://bitcoinprivacy.guide/node.html).
