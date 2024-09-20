---
description: >-
  Decisions are made regarding the funding goal, total supply of tokens, and
  distribution of tokens for various purposes (Vault).
---

# Step 2: Token Economy

## Overview

Token Economy is the process of determining how many tokens to issue and for what purpose, including funding for development in blockchain projects, providing incentives for development teams, marketing costs, and providing liquidity to facilitate token trading.&#x20;

However, in TONStarter, Token Economy settings can be easily completed by answering three questions. The purpose and distribution ratio of tokens, which are most commonly configured, are set up in advance. Of course, if you enter Advance mode and do not follow these basic settings, you can adjust each item in detail.&#x20;

The three questions are as follows:

1. **(Setting Funding Target Amount)** How much do you want to raise?&#x20;
2. **(Setting Total Supply & Token Funding Price)** Select your Total Supply & Token Funding Price
3. **(Setting Token Listing Price)** To list on the DEX, your project token should have a listing price denominated in TOS calculated from the token funding price in TON as below. However, If you prefer, you can change it directly in the TOS input field.

### 01. Setting Funding Target Amount

1. **(Question)** How much do you want to raise?
   * **(Answer)** When you click the dropdown button, frequently used funding target amounts are displayed. You can choose the goal amount from these options. If the desired target amount is not available, you can enter the amount directly in dollars.&#x20;
   * Once the Funding target input is completed, this amount is automatically divided by 30% to calculate the Current Market Cap. In other words, the tokens equivalent to 30% of the total issuance are distributed to investors who participate in the Funding, making it possible to calculate the Current Market Cap. by reversing this process.&#x20;

{% hint style="info" %}
Current Market Cap. = Funding Target($) / 30%
{% endhint %}

2. Token Distribution is automatically calculated
   * The total issuance of tokens is distributed in the ratio set by the vault created for various purposes.

<table><thead><tr><th width="156.33333333333331">Vault</th><th width="264">Token Quota</th><th>Description</th></tr></thead><tbody><tr><td>Public</td><td>30%</td><td>Project tokens distributed to public investors to raise funding</td></tr><tr><td>Liquidity</td><td>15%</td><td></td></tr><tr><td>Ecosystem</td><td>35%</td><td></td></tr><tr><td>Team</td><td>15%</td><td></td></tr><tr><td>TONStarter</td><td>WTON-TOS LP reward (2.5%)</td><td>Project tokens distributed to holders who contributed liquidity in the form of TON-TOS exchange</td></tr><tr><td></td><td>TON Staker (1.25%)</td><td>Project tokens distributed as a reward to users who have staked TON</td></tr><tr><td></td><td>TOS Staker (1.25%)</td><td>Project tokens distributed as a reward to users who have staked TOS</td></tr></tbody></table>

{% hint style="warning" %}
* The total supply of project tokens and the total allocation of tokens for vault creation are set to be the same by default.
* Even if you move to Advance mode and distribute token allocations directly, the total sum must still be set to be the same.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (237).png" alt=""><figcaption><p>Funding Target Question (top left), Token Distribution (top right), Token Economy Summary (bottom left)</p></figcaption></figure>

### 02. Setting the Total Supply and Token Funding Price

1. **(Question)** Select your Total Supply & Token Funding Price.
   * **(Answer)** When you press the drop-down button, the commonly used Total Supply and the corresponding Token Funding Price will be displayed. You can choose the one that suits the nature of your project.
   * If you don't have the total number of tokens you're looking for, you can select "Other" and type it in the blank.
   * The token funding price is automatically calculated based on the size of the total issuance and presented together in each view.
2. Automated Token Funding Price Calculation
   * 30% of the total supply will be allocated to the public vault and will be distributed to investors when the funding target amount determined by question 1 is met.
   * Therefore, we can estimate Token Funding Price which means the unit price of the token as shown below.
   * Since investors are funded in TON, the unit of the token funding price is first calculated in $ and then converted to TON as shown below.

{% hint style="info" %}
**Token Funding Price($)** = Funding Target($) / (Total Supply x 30%)\
\
Token Funding Price(TON) = TON Market Price($) / **Token Funding Price($)**
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (316).png" alt="" width="563"><figcaption></figcaption></figure>

### 03. Setting the Token Listing Price

1. **(Question)** To list on the DEX, your project token should have a listing price denominated in TOS calculated from the token funding price in TON as below. However, If you prefer, you can change it directly in the TOS input field.
   * **(Answer)** Based on the current market price of TOS, it is automatically calculated and presented as a default value as shown below.
   * However, it is possible that the price at this time will be different from the price at a future listing, so you can edit this price yourself to account for that.

{% hint style="info" %}
Token Listing Price(TOS) = Token Funding Price(TON) /  TOS Market Price(TON)
{% endhint %}

2.  (Note) The need for a token listing price

    * The project token will be listed on Uniswap in the form of a liquidity pool to increase trading liquidity.
    * Since we are creating a liquidity pool by pairing project tokens with TOS tokens, we need to set a price ratio between the two tokens, called the 'Token Listing Price', and the price unit will be TOS.

    <figure><img src="../../../.gitbook/assets/image (302).png" alt="" width="563"><figcaption><p>Auto-calculated case with Token Listing Price of 0.4 TOS (can be manually modified)</p></figcaption></figure>
