---
description: >-
  Deposit or withdraw assets between Ethereum and Titan using bridge
  functionality.
---

# Bridge

{% hint style="info" %}
Bridge is the core functionality of Tokamak Bridge; it offers a secure way to move assets between Ethereum and Titan.&#x20;
{% endhint %}

"Deposit" allows users to move asset from Ethereum to Titan. It will take 5 minutes for the deposit from Ethereum to be propagated to Titan. The wait time ensures that Titan is not minting any new assets in case there is a block reorganization on Ethereum.&#x20;

"Withdraw" moves asset from Titan to Ethereum. Based on the 7 days fraud proof window, withdraw is expected to take 7 days from the point when the withdraw transaction is rolled up to L1.&#x20;

* [How to perform a Deposit](deposit.md)
* [How to perform a Withdraw](withdraw.md)
