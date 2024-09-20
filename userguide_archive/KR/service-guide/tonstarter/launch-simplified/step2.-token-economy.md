---
description: 펀딩목표액, token의 총발행량(Total Supply), 다양한 용도별 token 배분 (Vault)등을 결정합니다.
---

# Step2. Token Economy

### 개요

Token Economy는 토큰을 얼마나 발행해서 어떤 용도로 사용할 것인지를 결정하는 과정으로서, 블록체인 프로젝트에 있어서 개발과정에 투입되는 자금, 개발팀에 대한 인센티브 제공, 마케팅 비용, 원활한 토큰 거래를 돕는 유동성 제공 등에 대한 지식이 필요합니다.&#x20;

하지만 TONStarter에서는 세 가지 질문에 답하면 Token Economy에 대한 설정이 간단히 완료됩니다. 가장 일반적으로 구성되는 토큰의 용도와 배분비율을 산정하여 미리 셋업을 해놓았기 때문입니다. 물론 이러한 기본설정을 따르지 않고 Adavnace mode로 진입하시면 상세하게 각 사항들을 조정할 수 있습니다.&#x20;

세 개의 질문은 다음과 같습니다.&#x20;

1. **( 펀딩목표액 설정)** How much do you want to raise ?
2. **(총발행량 및 토큰펀딩가격 설정)** Select your Total Supply & Token Funding Price.
3. **(토큰상장가격 설정)** To list on the DEX, your project token should have a listing price denominated in TOS calculated from the token funding price in TON as below. However, If you prefer, you can change it directly in the TOS input field.

### 01. 펀딩 목표액 설정

1. **(질문)** How much do you want to raise ?
   * (대답) 드롭다운 버튼을 누르면 자주 사용되는 펀딩목표액이 보기로 나옵니다. 이 가운데에서 목표로 하는 펀딩금액을 있으면 고르시면 됩니다.&#x20;
   * 원하는 목표금액이 없는 경우 $단위로 직접 입력하면 됩니다.
   * Funding target 입력이 완료되면 이 금액을 30%로 나눠서 Current Market Cap 금액이 자동으로 산출됩니다. 즉, 총발행량의 30%에 해당하는 토큰이 Funding target 조성에 참여한 투자자에게 지급되므로 이를 역산하여 Current Market Cap.을 구할 수 있는 것입니다.

{% hint style="info" %}
Current Market Cap. = Funding Target($) / 30%
{% endhint %}

2. Token Distribution 자동산정
   * 토큰의 총발행량은 다양한 목적에 따라 만들어진 vault에 정해진 비율대로 배분됩니다.

<table><thead><tr><th width="156.33333333333331">Vault</th><th width="264">Token Quota</th><th>Description</th></tr></thead><tbody><tr><td>Public</td><td>30%</td><td>Funding target에 해당하는 금액을 모으기 위해서 지불하는 프로젝트 토큰을 의미하며, 총발행량의 30%에 해당</td></tr><tr><td>Liquidity</td><td>15%</td><td></td></tr><tr><td>Ecosystem</td><td>35%</td><td></td></tr><tr><td>Team</td><td>15%</td><td></td></tr><tr><td>TONStarter</td><td>WTON-TOS LP reward (2.5%)</td><td>TON-TOS 교환을 위한 유동성 제공형태로 기여한 보유자에게 지급되는 토큰 </td></tr><tr><td></td><td>TON Staker (1.25%)</td><td>TON을 staking한 사용자에게 보상으로 지급되는 토큰</td></tr><tr><td></td><td>TOS Staker (1.25%)</td><td>TOS를 staking한 사용자에게 보상으로 지급되는 토큰</td></tr></tbody></table>

{% hint style="warning" %}
* 프로젝트 토큰의 총 발행량(Total Supply)과 생성하는 볼트의 토큰 할당량(Token Allocation)의 총 합(Sum)은 기본적으로 같도록 설정되어 있습니다.&#x20;
* 만일 Advance mode로 이동하여 토큰 할당량을 직접 배분하는 경우에도 합계는 같도록 설정해야 합니다.&#x20;
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (272).png" alt=""><figcaption><p>Funding Target 질문(좌상단), Token Distribution (우상단), Token Economy Summary(좌하단)</p></figcaption></figure>

### 02. 총발행량(Total Supply) 및 토큰펀딩가격(Token Funding Price) 설정

1. **(질문)** Select your Total Supply & Token Funding Price.
   * (대답) 드롭다운 버튼을 누르면 자주 사용되는 총발행량(Total Supply) 및 그에 상응하는 토큰펀딩가격(Token Funding Price)이 보기로 제시됩니다. 그 중에서 본 프로젝트의 성격에 맞는 것을 고르시면 됩니다.
   * 원하는 수준의 총발행량이 없다면 'Other'를 선택한 후, 공란에 직접입력하면 됩니다.&#x20;
   * 토큰펀딩가격은 총발행량의 크기에 따라서 자동으로 계산되어 각 보기마다 함께 제시됩니다.&#x20;
2. 토큰펀딩가격(Token Funding Price) 자동산정
   * Total Supply 물량 중 30%는 Public vault에 배정되는 물량으로서, 1번 질문에 의해 결정되는 펀딩목표금액만큼 투자유치가 이뤄지면,  그에 대응하여 투자자에게 배분됩니다.&#x20;
   * 따라서 아래와 같이 토큰의 단위가격, 즉 '토큰펀딩가격(Token Funding Price)'를 추산할 수 있습니다.
   * 투자자들의 펀딩은 TON으로 이뤄지므로 토큰펀딩가격의 단위도 $로 먼저 계산된 후, 아래와 같이 TON으로 환산됩니다.

{% hint style="info" %}
**Token Funding Price($)** = Funding Target($) / (Total Supply x 30%)\
\
Token Funding Price(TON) = TON Market Price($) / **Token Funding Price($)**
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (138).png" alt=""><figcaption></figcaption></figure>

### 03. 토큰상장가격(Token Listing Price) 설정

1. **(질문)** To list on the DEX, your project token should have a listing price denominated in TOS calculated from the token funding price in TON as below. However, If you prefer, you can change it directly in the TOS input field.
   * (대답) 현 시점의 TOS시장가격에 기초하여 아래와 같이 자동으로 계산되어 기본값으로 제시됩니다.&#x20;
   * 다만 현시점의 가격과 추후 상장시점의 가격이 달라질 가능성이 있으므로, 이를 감안하여 사용자는 이 가격을 직접 수정할 수 있습니다.&#x20;

{% hint style="info" %}
Token Listing Price(TOS) = Token Funding Price(TON) /  TOS Market Price(TON)
{% endhint %}

2. (참고) 토큰상장가격의 필요성
   * 프로젝트 토큰은 거래유동성을 높이기 위해서 Uniswap에 유동성 풀(liquidity pool)을 만드는 형태로 상장을 하게 됩니다.&#x20;
   * 이때 프로젝트 토큰과 TOS 토큰을 쌍을 이뤄서 유동성 풀을 만들게 되므로, 두 토큰 간의 가격비율, 즉 '토큰상장가격(Token Listing Price)'을 설정해야하며, 따라서 가격단위는 TOS가 되는 것입니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (160).png" alt=""><figcaption><p>토큰상장가격(Token Listing Price) : 0.4TOS로 자동산출된 사례(직접 수정가능)</p></figcaption></figure>
