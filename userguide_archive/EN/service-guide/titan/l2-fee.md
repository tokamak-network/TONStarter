---
description: >-
  This document outlines the calculation process for transaction fees on Titan,
  emphasizing their lower cost compared to Ethereum.
---

# L2 fee

Titan's transaction fees are determined by adding two components together:

* L2 execution fee
* L1 security fee

### L2 execution fee

```
tx.gasPrice * l2GasUsed
```

* The L2 execution fee refers to the fee incurred when a user's transaction is processed within the Titan layer2 network. It follows a calculation method shown above, identical to the standard Ethereum transaction fee computation. However, the distinction lies in the fact that the gas price on Titan is significantly lower compared to Ethereum.

### L1 security fee

```
l1_base_fee * (tx_data_gas + overhaed) * scalar
```

* The L1 security fee is an essential fee required in the context of Optimistic Rollup. With Optimistic Rollup, all L2 transactions are uploaded to L1 to ensure data availability.&#x20;
* To transmit these rollup transactions to L1, a portion of the L2 transaction fee is used for the L1 transaction fee. While the rollup transaction includes the `calldata` of all L2 transactions, it's important to note that L2 transactions are not directly executed in L1.&#x20;
* Consequently, only the intrinsic gas generated when incorporating the L2 transaction `calldata` into the rollup transaction is calculated. The term `tx_data_gas` mentioned earlier refers to this, and its calculation is as follows.

```
tx_data_gas = count_zero_bytes(tx_data) * 4 + count_non_zero_bytes(tx_data) * 16
```

* The `l1_base_fee` represents the base fee of L1, which is the amount of ETH required for the rollup transaction.&#x20;
* Titan continuously monitors the Ethereum base fee fluctuations; whenever there is a substantial change, a new `l1_base_fee` is stored in the L2 `OVM_GasPriceOracle` contract.
* The `overhead` is calculated in gas units and is assigned a relatively small value. `scalar` is the weight multiplied for the L1 security fee.
