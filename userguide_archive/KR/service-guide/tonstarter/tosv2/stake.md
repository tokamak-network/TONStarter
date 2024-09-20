---
description: >-
  LTOS를 얻기 위해서는 TOS를 스테이킹해야하며, LTOS와 sTOS를 얻기위해서는 일정기간동안 Lock-up을 해야 합니다. LTOS는
  인덱스 토큰(indexed token)으로서 TOS와 swap되며, swap ratio는 LTOS index 값에 의해 결정됩니다.
---

# Stake

### 01. 개요

TOSv2 좌측의 매뉴에서 Stake를 클릭하면 아래와 같은 화면이 나옵니다.

* ⓵ Total Value Staked : 현재까지 스테이킹된 TOS의 총금액($)입니다.
* ⓶ TOS APY : LTOS의 이자계산주기(rebase)인 8시간마다 증가되는 이자율을 연간복리로 환산한 수익률로서, TOS를 스테이킹 할 경우, 기대되는 연이자율입니다.
* ⓷ LTOS Index : TOS를 스테이킹(staking) 혹은 언스테이킹(unstaking) 할 경우 LTOS와 TOS간의 스왑비율(swap ratio)을 의미합니다. LTOS Index는 LTOS 보유자에게 이자를 지급할 수 있도록 하루 세 번, 매 8시간마다 복리로 계산되므로 계속 상승합니다(한국시간 기준(UTC+9): 오전 4시, 정오, 오후 8시).&#x20;

{% hint style="info" %}
LTOS index 계산원리

* 예를 들어, LTOS index = 2.0 TOS 이라고 가정해봅니다.
* 이 때 100 TOS를 스테이킹(staking) 하는 경우, 100/2 = 50 LTOS를 얻게 됩니다.&#x20;
* 이후 LTOS index = 3.0으로 증가했다고 가정해봅니다.
* 이 때 보유하신 50 LTOS를 언스테이킹(unstaking) 하고 TOS로 돌려받는 경우, 3\*50 = 150 TOS를 받게 됩니다.  이렇게 되면 100 TOS를 스테이킹 하여 50 TOS의 이익이 생긴 것입니다. &#x20;
{% endhint %}

* ⓸ Stake : TOS를 stake 하면 복리이자에 해당하는 LTOS를 얻게 됩니다. 추가적으로 sTOS를 얻기위해서는 lock-up 기간도 설정하셔야 합니다.&#x20;
* ⓹ List selection : 스테이킹이 완료된 리스트가 카드형태로 리스트업 되는데, All / Bond / Stake를 각각 선택하여 해당 부분만 리스트업이 되도록 조절할 수 있습니다.&#x20;
* ⓺ Manage : lock-up 기간이 아직 끝나지 않은 상태라면, sTOS를 더 받기 위하여 추가적으로 lock-up될 TOS 물량이나 lock-up 기간 등을 증가시킬 수 있습니다.
* ⓻ Rebase time : 스테이킹된 TOS의 복리이자를 계산하는 LTOS index는 8시간마다 하루 세 번 계산됩니다(오전 4시, 정오, 오후 8시). 다음 복리이자 계산시점까지 남은 시간이 여기에 표시됩니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (107).png" alt=""><figcaption></figcaption></figure>

### 02. Stake 실행절차

상기 화면에서 ⓸ Stake 버튼을 누르면, 아래와 같이 상세설정 화면이 나옵니다.

* 보유한 TOS물량 중에서 스테이킹 하시기를 원하는 물량만큼 입력합니다. (아래 그림에서는 20 TOS를 입력한 사례)
* Lock-up기간을 설정하면 sTOS를 받을 수 있습니다. (아래 그림에서는 4주를 입력한 사례). Lock-up기간이 종료되면, LTOS를 언스테이킹(unstaking) 할 수 있습니다. &#x20;
* No Lock-up 박스를 선택하면 언제든지 LTOS를 언스테이킹(unstaking) 할 수 있는 대신, sTOS는 받지 못합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (174).png" alt=""><figcaption></figcaption></figure>

* Stake버튼을 누르면 MetaMask, Trezor 등 암호화폐 지갑이 나타나고 승인을 누르면, 거래(transaction)가 최종처리될 때까지 아래 그림처럼 각 영역에서 회전하는 동그라미를 볼 수 있습니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (270).png" alt=""><figcaption></figcaption></figure>

* 블록체인 네트워크를 통해 거래(transaction) 처리가 완료되면 아래와 같이 성공메시지가 나옵니다.

<figure><img src="../../../.gitbook/assets/image (263).png" alt=""><figcaption></figcaption></figure>

### 03. Manage

Lock-up 기간이 종료되지 않았다면, 스테이킹 물량의 증가 혹은 Lock-up 기간을 증가시켜 sTOS를 증가할 수 있습니다.

<figure><img src="../../../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

* 아래 사례의 경우 30 TOS를 추가하고, 20주로 기간을 증가 시켰습니다. 현재 락업(lock-up) 기간은 녹색, 추가된 기간은 파란색 막대기로 표시됩니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (223).png" alt=""><figcaption></figcaption></figure>

* Update버튼을 누르면 manage 내용이 적용 됩니다.&#x20;
* 적용된 Manage 결과는 Stake page에서 확인이 가능합니다

<figure><img src="../../../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

### 04. How to relock

Lock-up 기간이 종료되면, 새로운 lock-up 기간을 설정하여 LTOS를 재락업(relock) 함으로써 더 많은 sTOS를 얻을 수 있습니다.

* Lock-up기간이 종료되면 "Manage" 버튼이 "Relock"버튼으로 바뀝니다.&#x20;
* sTOS를 더 많이 얻으시려면 'Relock' 버튼을 클릭하여 주십시오.&#x20;

<figure><img src="../../../.gitbook/assets/image (153).png" alt=""><figcaption></figcaption></figure>

* Relock을 하고자 하는 sTOS물량을 입력하여 주십시오. 일부만 Relock을 하게 되면 잔여물량은 TOS로 교환됩니다.
* Relock 기간을 새로 설정하여 주십시오.&#x20;
* 'Update' 버튼을 클릭하여 relock을 실행합니다.&#x20;
* Relock 하고자 하는 LTOS 물량을 입력하여 주십시오. Relock 하지 않은 잔여 LTOS는 TOS로 반환되어 들어옵니다.&#x20;
* Update버튼을 누르면 Relock 내용이 적용 됩니다.&#x20;
* 적용된 Relock 결과는 Stake page에서 확인이 가능합니다.

<figure><img src="../../../.gitbook/assets/image (212).png" alt=""><figcaption></figcaption></figure>

* 만약 Relock을 실행함에 있어서 추가적으로 TOS를 더 락업(lock-up)하여 실행하고자 한다면, Lock additional TOS box에 체크해주시면 됩니다.

<figure><img src="../../../.gitbook/assets/image (105).png" alt=""><figcaption></figcaption></figure>

