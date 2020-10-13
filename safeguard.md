---
layout: default
---
<br/>

## Safeguarding your Bitcoin

### Table of Contents

1.  [What is cold storage?](#why-safeguard)
2.  [Desktop node](#desktop-node-version)
3.  [Plug + Play node](#plug-play-node-version)
3.  [DIY node](#diy-node-version)
4.  [Other options](#other-options)
5.  [Trade-offs](#trade-offs)


### Why safeguard?

So far all we have discussed are mobile wallets that favour convenience because they are internet connected devices that allow you quick and easy access to your bitcoin. The drawback with convenience is that interenet connected devices bring their own exposure which may not be desireable if you are storing larger amounts of bitcoin. So how can we safeguard that bitcoin in a more secure way?

Cold storage refers to a method of bitcoin storage that has never touched the internet. For most users this takes the form of a hardware wallet which is a dedicated device designed with one aim, to generate and secure your private keys. When looking for a cold storage method, look for 'air gapped' devices like the [Coldcard](https://coldcardwallet.com/) or [Cobo Vault](https://cobo.com/hardware-wallet/cobo-vault). These devices never need to be plugged into your *potentially* malware infected computer to sign transactions and allow you to spend your bitcoin, adding a huge layer of protection from attack.    

### Desktop Node Version

**Bitcoin Core + Specter Desktop + Coldcard**

1.  Set up your [Coldcard](https://coldcardwallet.com/docs/quick)
2.  Download [Bitcoin Core](https://bitcoin.org/en/download)
2.  Open Core, go to 'options' and edit the config file to add the line `server=1`
3.  Restart Core, initital block download (IBD) will now recommence.
4.  Download [Specter Desktop](https://github.com/cryptoadvance/specter-desktop/releases)
5.  Select 'run local Specter server'
6.  Bitcoin Core will be automatically detected
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

### Plug + Play Node Version

**myNode One + Specter + ColdCard**

1.  Setup your [Coldcard](https://coldcardwallet.com/docs/quick)
2.  Setup your [myNode One](http://mynodebtc.com/guide/getting_started)
3.  Wait for initital block download (IBD) to complete
4.  Enable and open Specter from your myNode dashboard
5.  In Specter press 'add new device' then give it a name and select the device type
6.  On your ColdCard export 'Electrum Wallet' to your Coldcard SD card and insert into your computer
7.  In Specter 'choose files' and select the **.JSON** file you just exported
8.  Press continue and the device will be added
9.  Press 'add new wallet' then 'single key'
10. Name the wallet, choose Segwit and select your Coldcard
11. Press continue then 'create wallet'
12. Wait for IBD to complete in Core
13. Select your newly created wallet in Specter and press receive to see your first address

### DIY Node Version

**RoninDojo + Electrum Desktop + Coldcard**

1.  Set up your [Coldcard](https://coldcardwallet.com/docs/quick)
2.  Assemble your RoninDojo node [hardware](https://wiki.ronindojo.io/en/hardware)
3.  Flash SD card then insert into device
4.  Complete Manjaro setup
5.  SSH into the device and install RoninDojo, ensuring you say 'yes' to installing Electrum Rust Server (electrs)
6.  Wait for IBD and Electrs compaction to complete
7.  Download [Electrum](https://electrum.org/#download) desktop wallet
8.  [Connect](https://wiki.ronindojo.io/en/gui-setup/step5) Electrum wallet to your Electrum Rust Server
9.  On your ColdCard export 'Electrum Wallet' to your Coldcard SD card and insert into your computer
10. In Electrum wallet press 'choose' then select the **.JSON** file that you just exported to the SD card and press next 
11. Wallet will load and you should see a warning asking you to connect your Coldcard, ignore this message and press no
12. Press receive to see your first address


### Other options 

There are plenty of other hardware wallet and node combinations, most will require some form of Electrum Server to act as a bridge between the underlying bitcoin software on your node and desktop wallet which the most commonly used hardware wallet interface.


### Trade-offs

* As touched on in the [secure](https://bitcoinprivacy.guide/secure.html) page, your backup **is** your bitcoin. This is no different for mobile or hardware wallets. Guard it with your life.

* If you have just coinjoined some of your bitcoin and are keen to get it sent off to cold storage, be mindful of how you construct your transaction. Merging UTXO's shows common ownership to anyone watching on chain.

* When getting any form of bitcoin related hardware delivered you are suceptible to supply chain attack. This means that an attacker could intercept the package and swap it out with a malicious device designed to steal your bitcoin. Whilst this is unlikely, it is something worth taking into account when setting up your devices. Ensure you follow the check procedures outlined by the product manufacturer when you receive. 

* Another thing worth considering is your payment method and delivery address. You can buy no-KYC bitcoin in cash from a meetup for maximum privacy, but if you buy a Coldcard from Coinkite (a public bitcoin company) using your credit card and have it delivered to your home address you certainly giving away some clues!

  
  ***
  
Now you have obtained, secured, segregated, labelled and coinjoined your bitcoin into both mobile and hardware wallets that are backed by your own node, let's look at how to [spend](https://bitcoinprivacy.guide/spend.html) your bitcoin in a private way.
