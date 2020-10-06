---
layout: default
---
<br/>

## Safeguarding your Bitcoin

### Table of Contents

1.  [What is coldstorage?](#why-safeguard)
2.  [Easy](#easy)
3.  [More in-depth](#more-indepth)
4.  [Other options](#other-options)
5.  [Trade-offs](#trade-offs)


### Why safeguard?

So far all we have discussed are mobile wallets that favour convenience because they are internet connected devices that allow you quick and easy access to your bitcoin. The drawback with convenience is that interenet connected devices bring their own exposure which may not be desireable if you are storing larger amounts of bitcoin. So how can we safeguard that bitcoin in a more secure way?

Cold storage refers to a method of bitcoin storage that has never touched the internet. For most users this takes the form of a hardware wallet which is a dedicated device designed with one aim, to generate and secure your private keys. When looking for a cold storage method, look for 'air gapped' devices like the [Coldcard](https://coldcardwallet.com/) or [Cobo Vault](https://cobo.com/hardware-wallet/cobo-vault). These devices never need to be plugged into your *potentially* malware infected computer to sign transactions and allow you to spend your bitcoin, adding a huge layer of protection from attack.    

### Easy

**Specter + Bitcoin Core + Coldcard**

1.  Setup your [Coldcard](https://coldcardwallet.com/docs/quick)
2.  Download [Bitcoin Core](https://bitcoin.org/en/download)
2.  Open core, go to 'options' and edit the config file and add the line `server=1`
3.  Restart core, initital block download (IBD) will now recommence.
4.  Download [Specter Desktop](https://github.com/cryptoadvance/specter-desktop/releases)
5.  Select 'run local Specter server'
6.  Bitcoin core will be automatically detected
7.  In Specter press 'add new device' then give it a name and select the device type
8.  On your ColdCard export 'Electrum Wallet' to your Coldcard SD card and insert into your computer
9.  In Specter 'choose files' and select the **.JSON** file you just exported
10. Press continue and the device will be added
11. Press 'add new wallet', then 'single key'
12. Name the wallet, choose Segwit and select your Coldcard
13. Press continue then 'create wallet'
14. Wait for IBD to complete in core
15. Select your newly created wallet in Specter and press receive to see your first address

[Here](https://www.youtube.com/watch?v=4koKF2MDXtk) is a fantastic video version of the above steps.

### More in-depth 

Ronin + CC
myNode + CC?

### Other options 



### Trade-offs

Delivery to home address
Backup

  
  ***
  
Now you have obtained, secured, segregated, labelled and coinjoined your bitcoin into both mobile and hardware wallets that are backed by your own node, let's look at how to [spend](https://bitcoinprivacy.guide/spend.html) your bitcoin in a private way.
