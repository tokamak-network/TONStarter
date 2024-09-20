---
description: 앞선 설정사항들이 반영된 smart contract가 배포되는 단계로서, 이 과정이 종료되면 프로젝트 론칭준비가 완료됩니다.
---

# Step3. Deploy

### 01. 배포(Deploy)

배포(Deploy) 해야할 Vault는 아래와 같습니다.

* Project token : 당해 블록체인 프로젝트 토큰의 총발행량(Max Supply)을 발행하는 스마트 컨트랙트를 배포하는 과정입니다.&#x20;
* Vesting vault : TON으로 투자받은 펀딩금액이 들어있는 vault입니다. 일정기간 동안 나눠서 claim 하는 형태로 프로젝트 팀에서 가져갈 수 있습니다.&#x20;
* Initial liquidity vault : Uniswap에 거래를 위한 유동성 제공용도로 보내질 프로젝트 토큰 및 TOS 토큰의 쌍(pair)가 들어있는 vault입니다.&#x20;
* Public sale : TON으로 펀딩해준 투자자들에게 제공하는 프로젝트 토큰이 들어있는 Vault입니다.&#x20;
* Other vaults : 상기 vault를 제외한 나머지 vault입니다.

손쉬운 배포를 위해서 기능을 아래와 같이 개선하였습니다.&#x20;

* 한번에 하나씩 Smart contract를 배포며, 카드형태로 제시된 내용을 확인하고 Deploy 버튼만 누르면 배포가 완료됩니다.&#x20;
* 배포가 완료되면 다음으로 배포될 Smart contract가 카드형태로 차례대로 나오게 됩니다.&#x20;

안전한 배포를 위해 아래와 같은 사항에 주의해주십시오.

1. 배포는 상당한 비용과 시간이 소요되는 과정입니다.&#x20;
2. 이러한 진행과정 중에 비용과 시간 부족으로 인해 프로젝트론칭이 불발되는 상황이 발생하지 않도록, TONStatert에서는 아래와 같이 자동으로 체크해드리오니 잘 확인하셔서 진행하여 주시기 바랍니다.&#x20;

{% hint style="warning" %}
* **(가스비용 체크)** 배포해야할 contract의 숫자가 많습니다. 배포를 진행하기에 앞서, 현재 보유하신 ETH가 가스비용으로 충분한지 자동으로 체크하여 모달창(modal window)로 안내 해드립니다.&#x20;
* **(마감기한 체크)** 배포 마감시한은 Snapshot 시점을 기준으로 8일전까지 입니다. 이 시점까지 남은 시간이 얼마인지를 deadline이라는 명칭으로 계산하여 화면상단에 보여주고 있습니다. 이 기한내에 완료하지 못할 경우, 프로젝트 론칭은 실패하게 되며, 그동안 투입한 가스비용도 돌려받을 수 없게 됩니다.&#x20;
* **(일정 재조정)** 작업도중 임시저장을 하고, 재접속을 하는 경우, 배포마감시한까지 1시간 미만이 남아 일정이 매우 촉박한 경우가 발생할 수 있습니다. 이 경우에는 스케줄을 재조정하도록 하여 프로젝트 론칭이 불발이 되지 않도록 모달창(modal window)로 안내해드립니다.&#x20;
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (152).png" alt=""><figcaption><p>마감기한내 배포완료를 위한 Deadline 카운터 (상단)</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (82).png" alt=""><figcaption><p>다양한 안내창(modal window) : 좌에서 부터 일정재조정, 가스비용체크(정상), 가스비용체크(경고)</p></figcaption></figure>

### 02. 프로젝트 게시 (Listing on TONStarter)

Deploy를 완료한 프로젝트는 아래와 같이 My project에 목록으로 나타나납니다.&#x20;

1. Edit : TONStarter에 프로젝트를 게시하기 전이라면, 앞서 설정한 내용을 수정할 수 있습니다.&#x20;
2. Listing on TONStarter : TONStarter에 프로젝트를 게시하게 되는 것이며 ,정해진 일정에 따라 커뮤니티에서 자유로이 투자가 진행됩니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (224).png" alt=""><figcaption><p>셋업을 완료하면 TONStarter에 리스팅을 대기중인 상태로 바뀌며 "Listing on TONStarter" 버튼을 누르면 론칭이 완료됨</p></figcaption></figure>

