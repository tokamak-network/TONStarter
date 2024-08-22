# Airdrop



## Available Tokens

```jsx
TON : 0x2be5e8c109e2197D077D13A82dAead6a9b3433C5
WTON : 0xc4A11aaf6ea915Ed7Ac194161d2fC9384F15bff2
TOS : 0x409c4D8cd5d2924b9bc5509230d16a61289c8153
LYDA : 0xE1B0630D7649CdF503eABc2b6423227Be9605247
DOC : 0x0e498afce58dE8651B983F136256fA3b8d9703bc
AURA : 0xaEC59E5b4f8DbF513e260500eA96EbA173F74149
```



## STOS 보유자에게 배분되는 에어드랍

- Contract: LockTOSDividendProxy [0x17332F84Cc0bbaD551Cd16675F406A0a2c55E28C](https://etherscan.io/address/0x17332f84cc0bbad551cd16675f406a0a2c55e28c)

### 에어드랍 하기(토큰 배분)

토큰을 배포하기 전에는 해당 토큰에서 **LockTOSDividendProxy 주소를 배분할 토큰 금액 만큼 승인(approve)을 미리 해야 합니다.**

- Function: [distribute](https://etherscan.io/address/0x17332f84cc0bbad551cd16675f406a0a2c55e28c#writeProxyContract#F5)
  - token: 토큰주소
  - amount: 배분할 토큰 양

### 에어드랍 가능한 금액 조회하기

- Function: [claimable](https://etherscan.io/address/0x17332f84cc0bbad551cd16675f406a0a2c55e28c#readProxyContract#F6)
  - _account: 에어드랍 받을 주소
  - _token: 토큰주소

### 에어드랍 청구하기

- Function: [claim](https://etherscan.io/address/0x17332f84cc0bbad551cd16675f406a0a2c55e28c#writeProxyContract#F2)
  - _token: 토큰주소



## 톤 스테이커를 위한 에어드랍

현재는 지원이 중지된 기능입니다. AURA 토큰이 이 컨트랙으로 두번의 에어드랍을 진행했습니다.  해당자는 클래임 함수를 통해 배포된 AURA를 청구할 수 있습니다.

- Contract : TokenDividendPoolProxy  [0x06245F89576536E9cF844C5804a8ad1CCeDb2642](https://etherscan.io/address/0x06245f89576536e9cf844c5804a8ad1ccedb2642)

### 에어드랍 가능한 금액 조회

- Function: [claimable](https://etherscan.io/address/0x06245f89576536e9cf844c5804a8ad1ccedb2642#readProxyContract#F5)
  - _token: 토큰주소 ( AURA의 경우, 0xaEC59E5b4f8DbF513e260500eA96EbA173F74149 )
  - _account: 에어드랍 받을 주소

### 에어드랍 청구하기

- Function: [claim](https://etherscan.io/address/0x06245f89576536e9cf844c5804a8ad1ccedb2642#writeProxyContract#F2)
  - _token: 토큰주소 ( AURA의 경우, 0xaEC59E5b4f8DbF513e260500eA96EbA173F74149 )