---
description: Bond를 구입하면 TOS를 할인된 가격에 구입할 수 있습니다.
---

# Bond

### 01. 개요

채권으로 TOS를 할인된 가격으로 구매하실 수 있습니다.

{% hint style="info" %}
* 최소 5일의 락업 기간이 있습니다.
* 대기 기간을 보상하기 위해 할인이 제공됩니다.
{% endhint %}

채권으로 구매된 모든 TOS는 채권 가치가 감소하지 않도록 자동으로 LTOS로 스테이킹됩니다.

{% hint style="info" %}
락업 기간이 1주일 이상인 경우 TONStarter의 거버넌스 토큰인 sTOS를 받으실 수 있습니다.
{% endhint %}

Bond 페이지에서 아래와 같은 3가지 항목을 볼 수 있습니다.

**(1) Treasury Balance**: 이는 보유하고 있는 TOS 이외의 현재 자산 총 가치를 보여줍니다. 유통 중인 모든 TOS는 보유 자산에 의해 보장됩니다.

**(2) TOS Price**: 현재 TOS의 시장 가격을 보여줍니다.

**(3) Bond List**: 채권 용량이 0이면 채권을 할 수 없을 수도 있습니다.

<figure><img src="../../../.gitbook/assets/image (208).png" alt=""><figcaption><p>TOSv2 Bond page</p></figcaption></figure>

### 02. Minting bonds v1.1

Bond List에서 원하는 Bond가 있다면, 해당 Bond버튼을 누릅니다 (위 그림에서 ⓷에 있는 'Bond 버튼'). 그러면 아래와 같이 구체적으로 Bond 구입시 설정하는 내용이 나타납니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (258).png" alt="" width="563"><figcaption></figcaption></figure>

#### ⓵ 구입조건 설정&#x20;

* 상기 그림에서는 Market Price보다 Bond Price가 13.79% 할인된 가격으로 제공되는 Bond 상품임을 보여주고 있습니다.&#x20;
* Min Bond : 구입에 따르는 수수료, 가스비 등을 고려했을 때에도 이익이 될 수 있는 Bond구입액의 최저한입니다. 이 금액보다 적은 금액으로 구입하면 할인으로 인한 이득보다 거래에 수반되는 수수료 등의 제반 비용이 더 커질 수 있어 권장하지 않습니다. &#x20;
* Max Bond : 한 번의 거래(transaction)에서 구입할 수 있는 최대금액을 의미합니다.&#x20;
* 따라서 구매하실 때에는 Min \~ Max 구간 이내에서 총구입금액을 결정합니다. (그림의 사례는 0.58 ETH로 설정)
* Lock-up Period : Bond 구입시점과 실제로 TOS를 받게되는 시점까지의 차이 기간을 의미합니다. 5 days Lock-up 박스에 체크를 하게 되면 TOS를 staking한 것과 마찬가지이므로, 그에 따른 sTOS를 추가로 받게 됩니다. sTOS는 TONStarter의 거버넌스토큰입니다. 5 days 보다 더 긴 기간을 Lock-up하고 싶다면, 최대 3년까지의 기간을 입력란에 직접 넣으면 됩니다 (상기 그림에서는 최대기간 설정 : 155weeks 6days 22:42 Max).&#x20;
* LTOS index : TOS를 unstaking이나 staking을 할 때 LTOS와의 교환비율을 의미합니다. 예를 들어 Lock-up이 종료되어도 unstaking이 자동으로 되는 것은 아닙니다. 고객님이 직접 unstaking을 해야만 TOS를 돌려 받는데, 이때 교환비율이 LTOS index입니다.&#x20;
* LTOS index 계산방식은 먼저, Lock-up을 설정한 TOS의 갯수만큼 LTOS 갯수가 책정이 되고. 이후 LTOS는 Lock-up period 기간 내에 복리이자를 붙어서 LTOS index라는 이름으로 원리금합계가 계속 증가됩니다.&#x20;
* 또한 staking할때도 LTOS index가 적용됩니다. 이때 LTOS index = 2TOS 인 경우, TOS 100개를 스테이킹 하면 100/2 = 50 LTOS를 받게 됩니다.
* 복리계산 주기 : LTOS index에 적용되는 복리계산은 하루 세 번(새벽 4시, 정오, 저녁 8시) 매 8시간마다 일어나며 그에 따라 LTOS index값도 갱신됩니다.&#x20;

#### ⓶ 설정결과 요약&#x20;

* 구입조건 설정의 결과를 간단히 요약한 부분으로서, 얼마의 금액으로 Bond를 구입했는지(You give), Lock-up이 종료되면 얼마를 받게 되는지(You will get), Lock-up은 언제 끝나는지(End-time) 각 보여주고 있습니다.



### 03. 구입

#### ⓵ 구입 최종승인

구입조건을 모두 확인한 후에, Bond 버튼을 누르면 MetaMask, Trezor 등 암호화폐 지갑이 나타납니다.&#x20;

* 암호화폐 지갑 내에서 '확인'버튼을 누르면 거래가 최종승인되어 실행됩니다.&#x20;

<img src="../../../.gitbook/assets/image (217).png" alt="" data-size="original">

#### ⓶ 구입결과 확인

거래 실행 후, 아래 그림에서 보듯이 방금 구입한 Bond가 앞쪽에 리스팅 되어 있습니다.

* 정렬기준을 recently added로 하면, 가장 최근에 구입한 내역이 가장 앞에 오게 됩니다.

<figure><img src="../../../.gitbook/assets/image (98).png" alt=""><figcaption><p>Bond 구입 시 5일이상 Lock-up기간을 설정하면, Stake화면에서도 해당 거래내역을 확인할 수 있다</p></figcaption></figure>
