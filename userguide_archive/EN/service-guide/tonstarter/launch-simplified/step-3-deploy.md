---
description: >-
  At this stage, the smart contract that reflects the previous settings is
  deployed, and the project is ready for launch at the end of this process.
---

# Step 3: Deploy

### 01. Deploy

Here are lists of contracts that need to be deployed:

* Project token: The process of deploying a smart contract that issues the total issuance (Max Supply) of the blockchain project token.
* Vesting vault: This vault contains the amount of funding invested in TON. It can be claimed by the project team in installments over a period of time.
* Initial liquidity vault: A vault containing pairs of project tokens and TOS tokens that will be sent to Uniswap to provide liquidity for transactions.
* Public sale: A vault containing project tokens that are offered to investors who funded with TON.
* Other vaults: The remaining vaults except for the above vaults.

For ease of deployment, we've made the following improvements to the feature.

* You can deploy smart contracts one at a time by checking the contents of the card and clicking the Deploy button to complete the deployment.
* When the deployment is complete, the next smart contract to be deployed will be displayed one after another in the form of a card.

To ensure a safe deployment, take note of the following points

1. Deployment is an expensive and time-consuming process.
2. To reduce the failure from deployment due to deployment cost or time, automatic check is done before initiating the deployment.

{% hint style="warning" %}
* **(Gas cost check)** There are a large number of contracts to be deployed. Before proceeding with the deployment, we will automatically check if your current ETH is sufficient to cover the gas cost and guide you to the modal window.
* **(Deadline check)** The deadline for deployment is 8 days before the snapshot. The amount of time remaining until this point is calculated and displayed at the top of the screen under the name deadline. If you don't meet this deadline, your project will fail to launch and you won't get your gas money back.
* **(Rescheduling)** If you save and reconnect while working, you may find that you have less than an hour left before the deployment deadline and the schedule is very tight. In this case, you will be directed to a modal window to reschedule your project so that it doesn't fail to launch.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (309).png" alt="" width="563"><figcaption><p>Deadline counter (top) for completing deployments on time</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (257).png" alt="" width="563"><figcaption><p>Various modal windows: from left to right, Reschedule, Check Gas Cost (Normal), Check Gas Cost (Warning)</p></figcaption></figure>

### 02. Publish your project (Listing on TONStarter)

Projects that have completed deployment appear as a list in My projects, as shown below.

1. **Edit**: If this is before you publish your project to TONStarter, you can modify the settings you made earlier.
2. **List on TONStarter** : You will publish your project on TONStarter, and the community will be free to invest according to a set schedule.

<figure><img src="../../../.gitbook/assets/image (172).png" alt="" width="563"><figcaption><p>Once you've completed the setup, your listing on TONStarter will be in a pending state and you can click the "List on TONStarter" button to complete your launch.</p></figcaption></figure>

