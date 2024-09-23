---
description: TONStarter sets default values to make launching your project quick and easy.
---

# Launch (Simplified)

### 1. Prepare to Launch

First, enter the TONStarter Launch page as shown below.

<figure><img src="../../../.gitbook/assets/image (317).png" alt="" width="375"><figcaption></figcaption></figure>

**Connecting a crypto wallet**

On the Launch screen, tap the Connect Wallet button in the upper right corner to connect your cryptocurrency wallet first.

The address to which future funded tokens will be sent will be the address of your currently linked crypto wallet. A warning window will appear asking you to agree to this. Confirm the wallet address and press the confirm button if you agree.

{% hint style="warning" %}
Future funding will be sent to the associated cryptocurrency wallet address, so make sure it's the correct one you want.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (195).png" alt="" width="369"><figcaption><p>Warning window (confirms that the currently linked wallet address is the one that will receive future funded tokens)</p></figcaption></figure>

A window will appear with the Terms of Use. Read it, check if you agree, and hit the confirm button.

<figure><img src="../../../.gitbook/assets/image (340).png" alt="" width="375"><figcaption><p>Terms of Use modal window</p></figcaption></figure>

### 2. Understanding the launch process and default values

Projects are launched in a three-step process, each step requiring you to set various parameters for the project to launch.

**⓵ 3 Steps to Launch**

1.  [**Project & Token** ](broken-reference)

    Enter the basics: the name of your project and token, and your funding schedule.
2.  [**Token Economy**](broken-reference)

    Determine the funding goal, the total supply of tokens, and the allocation of tokens for various purposes (Vault).
3.  [**Deploy**](broken-reference)

    This is the stage where the smart contract that reflects the above settings is deployed, and the project is ready for launch at the end of this process.

{% hint style="warning" %}
Creating a project consists of 3 steps, and each step has a Save button to allow you to save between steps. Please note that if you refresh without saving, your input values may be lost.
{% endhint %}



**⓶ Default values**&#x20;

To launch a project, you need to make a number of settings. To help you launch your project quickly, TONStarter Launch has already filled in the most common values as defaults.

{% hint style="warning" %}
If you don't want to use the default values and want to fine-tune the parameters to suit the nature of your project, you can click the Advanced mode button. However, once you move to Advanced mode and proceed with the project settings, you cannot return to the default mode.
{% endhint %}

The project launch parameter values that are set to default are shown below.

<table><thead><tr><th width="203.33333333333331">Step</th><th width="219">Parameter</th><th>Default values</th></tr></thead><tbody><tr><td>01. Project &#x26; Token</td><td>Token Type <br>(not adjustable)</td><td><strong>Type A</strong> </td></tr><tr><td></td><td>Token Funding Price<br>(in TON)</td><td>No default (just user input field)</td></tr><tr><td></td><td>Token Listing Price <br>(in TOS)</td><td>No default (just user input field)</td></tr><tr><td></td><td>Initial Liquidity Pool </td><td><strong>10% of Funded TON</strong></td></tr><tr><td>02. Token Economy</td><td>Vaults and Toke Allocation <br>(not adjustable)</td><td><p><strong>Public(30%) Ecosystem(35%) Team(15%) Liquidity(15%)</strong></p><ul><li>Initial Liquidity(3.0%)</li><li>Token-TOS LP Reward(12.0%) </li></ul><p></p><p><strong>TONStarter(5%)</strong> </p><ul><li> WTON-TOS LP reward : 2.5% </li><li>TON Staker : 1.25% </li><li>TOS Staker : 1.25%</li></ul></td></tr><tr><td></td><td>Snapshot </td><td>At least 11 days later than the current time - If adjusted, Snapshot should be 8 days or more later than the current time</td></tr><tr><td></td><td>Whitelist <br>(not adjustable)</td><td>1 second after Snapshot ~ 1 second before Public Sale 1. (But this duration should be at least 2 days or more.)</td></tr><tr><td></td><td>Token Allocation between Public Sale 1, 2 <br>(not adjustable)</td><td>Public Sale 1 : 50% Public Sale 2 : 50%</td></tr><tr><td></td><td>Public Sale 1 (adjustable)</td><td>1 second after Whitelist has finished ~ 2 days</td></tr><tr><td></td><td>Public Sale 2 (adjustable)</td><td>1 second after Public sale 1 has finished ~ 2 days</td></tr><tr><td></td><td>Vesting Round 1 <br>(not adjustable)</td><td><ul><li>1 second after the end of the Public Sale 2 </li><li>Claim limit : 40% </li></ul></td></tr><tr><td></td><td>Vesting Round 2~4 <br>(not adjustable)</td><td><ul><li>360 days after the previous round</li><li>Claim limit : Round 2 (20%),  Round 3 (20%) , Round 4 (20%)</li></ul></td></tr><tr><td></td><td>Send Tokens to Initial Liquidity <br>(not adjustable)</td><td>1 second after the end of the Public Sale 2</td></tr><tr><td></td><td><strong>Token Generation Event</strong> (TGE <strong>:</strong> The time to Unlock Vaults Starts) <br><br>(not adjustable)</td><td>1 second after the end of the <mark style="color:red;">Public Sale 2</mark></td></tr><tr><td>03. Deploy - Initialize each vaults</td><td><strong>Claim schedule</strong> (49 rounds) for each vaults</td><td><a href="https://drive.google.com/file/d/1YF5K6cmx4_6D3vVaCfGtWc9HpU16ZmzU/view?usp=sharing">schedule file </a></td></tr></tbody></table>

{% hint style="info" %}
There are three types of tokens&#x20;

1. Type A : Burnable, approveAndCall, Snapshot, Permit, Non mintable
2. Type B: Burnable, Snapshot, Mintable
3. Type C: Burnable, Mintable
{% endhint %}

#### **(Note 1) Vesting & Claim details after deployment and launch**

The Deploy phase is a process in which various smart contracts are deployed, and it is further divided into three phases: **Deploy**, where smart contracts are deployed, **Send**, where project tokens are sent to each vault, and **Initialize**, where each vault is initialized, as shown in the figure below.

{% hint style="info" %}
At TONStarter, we have prepared a UX/UI that makes it easy for anyone to go through these steps one by one with the click of a button.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (221).png" alt=""><figcaption><p>Flow Diagram of Deploy, Vesting, and Claim</p></figcaption></figure>

Once this is complete, you're all set to launch your project. Once your project is open and subsequently funded, the vesting and claiming process will follow, as follows.

* **(Vesting)**  For the project team, the vesting process begins, where the funding raised by the TON is spread out over a period of time. This is to incentivize diligent project progress and will be opened in four installments over three years. Vesting rate per installment: 1 time (40%), 2-4 times (20% each). The one-time vesting rate is up to 50%, and can be increased but not decreased over a total of four rounds.&#x20;
* **(Claim)** Investors who have invested in the project will also be able to claim their project tokens to their crypto wallets in installments over a period of time. There will be seven installments over three years. You can claim the unclaimed portion at any time, and you can claim together in the next round.

{% embed url="https://drive.google.com/file/d/1YF5K6cmx4_6D3vVaCfGtWc9HpU16ZmzU/view?usp=sharing" %}
Claims and vesting timeline
{% endembed %}

