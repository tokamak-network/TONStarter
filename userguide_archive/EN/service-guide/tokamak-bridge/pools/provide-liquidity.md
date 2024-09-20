---
description: >-
  Liquidity Providers (LP) can concentrate their capital within custom price
  ranges, providing greater amounts of liquidity at desired prices.
---

# Provide Liquidity

{% hint style="warning" %}
Liquidity Providers will only earn fees from trading volume on the network they are providing liquidity.&#x20;

* If you provide liquidity on Titan: receive swap fee for trading activties on Titan network
* If you provide liquidity on Ethereum: receive swap fee for trading activities on Ethereum network
{% endhint %}

Tokamak Bridge allows LPs to optionally concentrate capital in the price range they believe will generate the highest return. For a more in-depth discussion of concentrated liquidity, please refer to the [Uniswap V3 announcement post](https://blog.uniswap.org/uniswap-v3).

To Provide liquidity on Tokamak Bridge follow these steps:

1. Click the Add Liquidity button

<figure><img src="../../../.gitbook/assets/image (50).png" alt=""><figcaption></figcaption></figure>

2. Select Network

{% hint style="info" %}
Network fees associated with pair creation, deposits, and withdrawals will be significantly cheaper on Titan than Ethereum. As a result, active management strategies such as rebalancing or reinvesting fees will be more cost effective for LPs on Titan.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (366).png" alt=""><figcaption></figcaption></figure>

3. Select a Fee Tier

<figure><img src="../../../.gitbook/assets/image (52).png" alt=""><figcaption></figcaption></figure>

* Every pair of tokens offers four fee tiers:
  * **0.01% fee tier:** Best for very stable pairs
    * The 0.01% fee tier is ideal for token pairs that typically trade at a fixed rate, such as stablecoin-stablecoin token pairs (e.g. USDC-USDT). LPs take on minimal price risk in these pools, and traders expect to pay minimal fees.
  * **0.05% fee tier:** Best for stable pairs
    * The 0.05% fee tier is ideal for token pairs that typically trade at a fixed or highly correlated rate, such as stablecoin-stablecoin token pairs.
  * **0.3% fee tier:** Best for most pairs
    * The 0.3% fee tier is best suited for less correlated token pairs such as the ETH-TON token pair, which are subject to significant price movements both to the upside and downside. This higher fee is more likely to compensate LPs for the greater price risk that they take on relative to stablecoin LPs.
  * **1.0% fee tier:** Best for exotic pairs
    * The 1.00% fee tier is designed for exotic assets, where LPs take on extreme price risk. Relevant assets are those that are particularly subject to monotonic price movements.

4. Select Pair

<figure><img src="../../../.gitbook/assets/image (53).png" alt=""><figcaption></figcaption></figure>

* You can select which pair of tokens you wish to provide as liquidity.
* Any pair of [ERC-20](https://eips.ethereum.org/EIPS/eip-20) tokens on Titan is valid, but each pair has different characteristics. You may wish to consider factors such as TVL, trading volume, and your assessment of the risk that these token prices diverge in the future.

5. Set Price Range

<figure><img src="../../../.gitbook/assets/image (54).png" alt=""><figcaption></figcaption></figure>

* Next you need to choose a price range in which to provide liquidity.
* **When making a price range decision, you should consider the degree to which you think prices will move over the course of your position's lifetime.** You should also consider your willingness to actively manage the position as the market evolves, and the economics of transactions required to actively manage a position.
* If the price moves outside your specified range, then your position will be concentrated in one of the two assets and not earn trading fees until the price returns to their range.
* See the visualizations in this [uniswap blog post](https://uniswap.org/blog/uniswap-v3) to observe how your assets are affected when the current price moves out of range.

{% hint style="info" %}
Note that your price will snap to the nearest tick. Don't worry if you're unable to type in a nice round number! This is expected because of how ticks work in Uniswap v3.
{% endhint %}

* Instead of picking a price range, you can provide liquidity across the Full Range by clicking the Full Range button. However, please note your rate of return will be significantly lower than a similar position with a more narrow price range.

6. Deposit Amounts

<figure><img src="../../../.gitbook/assets/image (55).png" alt=""><figcaption></figcaption></figure>

* With your fee tier, pair, and price range selected, you can now decide how much capital to contribute to this position. Enter a value in one of the two fields and the other value will be automatically populated the corresponding amount.
* The ratio of these two fields is based on the position of your price range around the market price. If your price range skews more toward one side of the market price, then you will provide more of that asset.
* This can be okay -- it is not necessary to target a 50/50 ratio though some strategies may choose that ratio. In many cases, it is not possible to balance exactly 50/50 due to the logarithmic spacing between price ticks.
* You can adjust your ratio by resetting the price range. The deposit amount that you typed in will remain fixed, while the second asset amount will adjust to the new ratio based on your new price range.
* If you select a price range that does not include the current market price, then you'll only need to provide a [single asset](https://support.uniswap.org/hc/en-us/articles/7423759991821) instead of both.

<figure><img src="../../../.gitbook/assets/image (56).png" alt=""><figcaption></figcaption></figure>

7. Approve and Add

<figure><img src="../../../.gitbook/assets/image (58).png" alt=""><figcaption></figcaption></figure>

* Finally, you are ready to submit the transaction. First, you can press Preview button and review the transaction details.

<figure><img src="../../../.gitbook/assets/image (59).png" alt=""><figcaption></figcaption></figure>

* You may need to approve the Manager contract to spend tokens on your behalf. This is only necessary the first time you provide liquidity with a token.
* Once the approve transaction has been confirmed, click Add to trigger the transaction in your wallet.
* Congrats! Once that transaction confirms, your assets now providing liquidity to traders and your position is earning fees. You can monitor and manage your position on the Pool page.

8. Pools page information

<figure><img src="../../../.gitbook/assets/image (63).png" alt=""><figcaption></figcaption></figure>

* **Earning Fees:** The position's current price is within the price range that you provided liquidity, so fees are being accumulated.
* **Not Earning Fees:** The position's current price is outside the price range that you provided liquidity so fees are not being accumulated.
* **Closed**: All liquidity has been removed from the position. It is still possible to increase liquidity.
* **No market data**: Token price from [Coingecko](https://www.coingecko.com/) is not available.&#x20;

