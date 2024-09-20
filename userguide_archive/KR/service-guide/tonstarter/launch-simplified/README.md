---
description: >-
  Launch 매뉴를 이용하면 누구나 Tokamak Network기반의 프로젝트 토큰을 생성하고 토큰 생태계를 창조할 수 있는 기능을
  제공합니다. 프로젝트 론칭에 필요한 주요 설정사항이 기본값(default)으로 설정되어 프로젝트를 쉽고 빠르게 론칭할 수 있습니다.
---

# Launch (Simplified)

### 1. Launch 준비

먼저 아래와 같이 TONStarter Launch 페이지로 진입합니다.

<figure><img src="../../../.gitbook/assets/image (151).png" alt=""><figcaption></figcaption></figure>

**암호화폐 지갑연결**

Launch 화면에서 우상단에 Connect Wallet 버튼을 눌러 암호화폐 지갑부터 연결하세요.&#x20;

향후 펀딩받은 토큰이 보내지는 주소가 현재 연결된 암호화폐지갑주소가 됩니다. 이에 동의하는지 물어보는 경고창이 나타납니다. 지갑주소를 확인하고 동의하시면 confirm 버튼을 누릅니다.&#x20;

{% hint style="warning" %}
연결된 암호화폐 지갑주소로 향후 펀딩금액이 전송되므로 원하는 올바른 지갑주소가 맞는지 반드시 확인해야 합니다. &#x20;
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (132).png" alt=""><figcaption><p>경고창 (현재 연결된 지갑주소가 향후 펀딩된 토큰을 받을 지갑주소가 맞는지 확인)</p></figcaption></figure>

이용약관(Terms of Use)을 담은 창이 나타납니다. 읽어본 후 동의하시면 체크하시고 confirm 버튼을 누릅니다.

<figure><img src="../../../.gitbook/assets/image (58).png" alt=""><figcaption><p>이용약관 모달창</p></figcaption></figure>

### 2. **론칭 절차 및 기본값에 대한 이해**

프로젝트는 3단계 절차를 통해 론칭되며, 각 단계마다 프로젝트 론칭에 필요한 다양한 파라메타를 설정해줘야 합니다.&#x20;

⓵ **3단계 론칭절차**

1.  [**Project & Token** ](step1-project-and-token.md)

    Project와 Token의 이름, 펀딩 스케줄 등 기본적인 사항을 입력합니다.
2.  [**Token Economy**](step2.-token-economy.md)

    펀딩목표액, token의 총발행량(Total Supply), 다양한 용도별 token 배분 (Vault)등을 결정합니다.
3.  [**Deploy**](step3.-deploy.md)

    상기의 설정사항들이 반영된 smart contract가 배포되는 단계로서, 이 과정이 종료되면 프로젝트 론칭준비가 완료됩니다.

{% hint style="warning" %}
프로젝트 생성은 총 3단계로 이뤄지고 Step 별로 저장(Save) 버튼이 있어 중간 저장이 가능합니다. 저장을 하지 않고 새로 고침을 하면 입력 값이 사라질 수 있으니 주의해주세요.
{% endhint %}



**⓶ 기본값(default)**&#x20;

프로젝트를 론칭하려면 여러가지 설정을 해줘야 합니다. TONStarter Launch에서는 신속한 프로젝트 론칭을 돕고자, 가장 많이 설정되는 값을 기본값(default)으로 이미 입력이 되어 있습니다.&#x20;

{% hint style="warning" %}
기본값을 사용하지 않고 프로젝트의 성격에 맞게 파라메타를 세밀하게 설정하고자 한다면 Advanced mode 버튼을 클릭하면 됩니다. 다만 이렇게  Advance mode로 옮겨서 프로젝트 설정을 진행하는 경우에는 default mode로는 돌아올 수 없습니다.&#x20;
{% endhint %}

기본값(default)으로 설정된  프로젝트 론칭 파라메타 값들은 아래와 같습니다.&#x20;

<table><thead><tr><th width="203.33333333333331">설정 단계</th><th width="219">파라메타</th><th>기본값(default)</th></tr></thead><tbody><tr><td>01. Project &#x26; Token</td><td>Token Type <br>(변경불가)</td><td><strong>Type A</strong> </td></tr><tr><td></td><td>토큰펀딩가격<br>(Token Funding Price, 단위: TON)</td><td>No default (just user input field)</td></tr><tr><td></td><td>토큰상장가격<br>(Token Listing Price,  단위: TOS)</td><td>No default (just user input field)</td></tr><tr><td></td><td>Initial Liquidity Pool </td><td><strong>펀딩받은 TON의 10%</strong></td></tr><tr><td>02. Token Economy</td><td>Vaults and Toke Allocation <br>(변경불가)</td><td><p><strong>Public(30%) Ecosystem(35%) Team(15%) Liquidity(15%)</strong></p><ul><li>Initial Liquidity(3.0%)</li><li>Token-TOS LP Reward(12.0%) </li></ul><p></p><p><strong>TONStarter(5%)</strong> </p><ul><li> WTON-TOS LP reward : 2.5% </li><li>TON Staker : 1.25% </li><li>TOS Staker : 1.25%</li></ul></td></tr><tr><td></td><td>Snapshot<br>(변경가능) </td><td>현재 시간보다 11일 이후로 넉넉히 설정되어 있으며, 이를 직접 변경할 경우에도 현재시간보다 최소 8일 이후로 설정해야 합니다.</td></tr><tr><td></td><td>Whitelist <br>(변경불가)</td><td>Snapshot 시점에서 1초 이후 ~ Public sale 시점 1초 전까지 (단, 이 기간은 최소 2일 이상이어야 합니다.)</td></tr><tr><td></td><td>Public Sale 1, 2 토큰배분 <br>(변경불가)</td><td>Public Sale 1 : 50% <br>Public Sale 2 : 50%</td></tr><tr><td></td><td>Public Sale 1 <br>(변경가능)</td><td>Whitelist 시점이후 2일간</td></tr><tr><td></td><td>Public Sale 2 <br>(변경가능)</td><td>Public sale 1 마감이후 2일간</td></tr><tr><td></td><td>Vesting Round 1 <br>(변경불가)</td><td><ul><li>Public sale 2 마감이후 언제든지 클레임 가능</li><li>클레임 한도: 펀딩받은 금액의 최대 40%까지</li></ul></td></tr><tr><td></td><td>Vesting Round 2~4 <br>(변경불가)</td><td><ul><li>이전 라운드 종류후 360일 경과이후 언제든지 클레임 가능</li><li>클레임 한도: 각 라운별로 펀딩받은 금액의 최대 20%까지</li></ul></td></tr><tr><td></td><td>Send Tokens to Initial Liquidity <br>(변경불가)</td><td>Public sale 2 마감이후 언제든지 </td></tr><tr><td></td><td>토큰 locking 해제일 (TGE <strong>:</strong> Token Generation Event) <br>(변경불가)</td><td>Public sale 2 마감 직후 시점</td></tr><tr><td>03. Deploy - Initialize each vaults</td><td>클레임 일정 (claim schedule : 각 vault 당 7 라운드)<br>(변경불가)</td><td>참조: <a href="https://drive.google.com/file/d/1YF5K6cmx4_6D3vVaCfGtWc9HpU16ZmzU/view?usp=sharing">각 vault 상세 스케줄 </a></td></tr></tbody></table>

{% hint style="info" %}
token 타입은 아래와 같이 세 종류가 있습니다.&#x20;

1. Type A : Burnable, approveAndCall, Snapshot, Permit, Non mintable
2. Type B: Burnable, Snapshot, Mintable
3. Type C: Burnable, Mintable
{% endhint %}

**(참고 1) Deploy 및 론칭 이후의 Vesting & Claim 상세절차**&#x20;

Deploy단계는 다양한 스마트컨트랙트가 배포되는 과정이며, 세부적으로는 아래 그림과 같이 스마트컨트랙트가 배포되는 Deploy, 각각의 vault로 프로젝트 토큰이 송금되는 Send, 각 Vault를 초기화해주는 Initialize 등 3단계로 다시 구분됩니다.&#x20;

{% hint style="info" %}
TONStarter에서는 이러한 절차를 하나씩 버튼만 클릭하면 누구나 손쉽게 진행할 수 있도록 UX/UI를 마련해놓았습니다.&#x20;
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (159).png" alt=""><figcaption><p>Flow Diagram of Deploy, Vesting, and Claim</p></figcaption></figure>

이 과정이 완료되면 프로젝트 론칭을 위한 준비작업이 모두 완료된 것입니다. 이후에 프로젝트가 오픈되고 이후에 펀딩까지 완료되면 다음과 같이 Vesting 및 Claim 절차가 뒤따릅니다.&#x20;

*   **(Vesting)**  프로젝트 팀 입장에서는 TON으로 조달된 펀딩금액을 일정기간에 걸쳐 나눠서 지급받는 Vesting 절차가 개시됩니다. 이는 성실한 프로젝트의 진행을 장려하기 위한 것으로서 3년에 걸쳐 총 4회에 나눠서 오픈됩니다.&#x20;

    회차별 Vesting 비율 : 1회(40%), 2회\~4회(각 20%). 1회의 비율은 최대 50%이며, 총 4회에 걸친 회차를 증가시킬 수는 있어도 감소할 수는 없습니다.&#x20;
* **(Claim)** 프로젝트에 투자한 투자자입장에서도 프로젝트 토큰을 자신의 암호화폐 지갑으로 일정기간에 걸쳐 나눠서 가져올 수 있는 Claim 절차가 개시됩니다. 3년에 걸쳐서 총 7회에 나눠서 오픈됩니다. 일정에 맞게 오픈이 되었으나 claim 하지 않은 분량은 언제든지 claim 할 수 있으며, 다음 회차에서 함께 claim을 진행해도 됩니다.&#x20;

{% embed url="https://drive.google.com/file/d/1YF5K6cmx4_6D3vVaCfGtWc9HpU16ZmzU/view?usp=sharing" %}
Claim 및 Vesting 일정표
{% endembed %}

