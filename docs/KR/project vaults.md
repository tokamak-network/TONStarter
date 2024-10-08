# Launched Project’s Vaults

> 기존의 런칭된 프로젝트의 볼트 컨트랙은 각 목적에 맞게 사용되기 위해 프로젝트 토큰과 볼트를 보유하고 있습니다.

## 프로젝트별 토큰 주소

|토큰 심볼	|토큰 주소	|etherscan|
| -------- | -------- | -------- |
| LYDA | 0xE1B0630D7649CdF503eABc2b6423227Be9605247 | [link](https://etherscan.io/address/0xE1B0630D7649CdF503eABc2b6423227Be9605247) |
| AURA | 0xaEC59E5b4f8DbF513e260500eA96EbA173F74149 | [link](https://etherscan.io/address/0xaEC59E5b4f8DbF513e260500eA96EbA173F74149) |
| DOC | 0x0e498afce58dE8651B983F136256fA3b8d9703bc | [link](https://etherscan.io/address/0x0e498afce58dE8651B983F136256fA3b8d9703bc) |



## PublicSale Vault 

- AURA PublicSale: 0x3B75d3f628C29d357b484EA7d091faEd63419267 : [link](https://etherscan.io/address/0x3B75d3f628C29d357b484EA7d091faEd63419267#writeProxyContract#F4)
- DOC PublicSale: 0xBef737D725993847c345647ebA096500FdAE71c6 : [link](https://etherscan.io/address/0xBef737D725993847c345647ebA096500FdAE71c6#writeProxyContract#F4)
- LYDA PublicSale: 0x3ba5c96665960ABD931858b8D80Ec80f53F2A09c: [link](https://etherscan.io/address/0x3ba5c96665960ABD931858b8D80Ec80f53F2A09c#writeProxyContract#F5)

### 함수 

### claim()

 토큰을 청구한다. 

- 파라미터
  - 없음
- 결과값
  -  없음

***



## Liquidity Vault 

- LYDA Liquidity: 0xf972657e6331e19ffcD1424a275215f7ab1A8df5:  [link](https://etherscan.io/address/0x620c86FD58E40f534545Aa433f49eF0271755E17#writeProxyContract#F6)

### 함수 

### mint(uint256 tosAmount)

 유동성 추가하기

- 파라미터
  - uint256 tosAmount : 입력 토스 양 (wei unit, 18 decimals)
- 결과값
  -  없음

***



## TONStaker Vault

- LYDA TONStaker: 0x620c86FD58E40f534545Aa433f49eF0271755E17:  [link](https://etherscan.io/address/0xf972657e6331e19ffcD1424a275215f7ab1A8df5#writeProxyContract#F4)

### 함수 

### claim()

 TON Staker에게 토큰을 에어드랍하기 위해 토큰 배분 컨트랙트에 토큰을 보낸다. 

- 파라미터
  - 없음
- 결과값
  -  없음

***



## TOSStaker Vault

- LYDA TOSStaker:  0xBb49719A0bC10bf9E8f0B5e2d0F74dEE830a0090 : [link](https://etherscan.io/address/0xBb49719A0bC10bf9E8f0B5e2d0F74dEE830a0090#writeProxyContract#F4)

### 함수 

### claim()

 TOS Staker에게 토큰을 에어드랍하기 위해 토큰 배분 컨트랙트에 토큰을 보낸다. 

- 파라미터
  - 없음
- 결과값
  -  없음

***



## WTON-TOS LP Reward Vault

- LYDA's WTON-TOS LP Reward :  0xA31945830C5a6B225A81962a10E78D2e3793D72D : [link](https://etherscan.io/address/0xA31945830C5a6B225A81962a10E78D2e3793D72D#writeProxyContract#F8)

### 함수 

### createProgram()

 유니스왑V3 WTON-TOS 풀의 LP 에게 리워드를 제공하는 프로그램을 생성한다. 

- 파라미터
  - 없음
- 결과값
  -  없음

***



## LYDA-TOS LP Reward Vault

- LYDA's LYDA-TOS LP Reward : 0x45D08f522BF2b6455Fe7EeF0f4aDf865D76EaD08  : [link](https://etherscan.io/address/0x45D08f522BF2b6455Fe7EeF0f4aDf865D76EaD08#writeProxyContract#F8)

### 함수 

### createProgram()

 유니스왑V3 LYDA-TOS 풀의 LP 에게 리워드를 제공하는 프로그램을 생성한다.

- 파라미터
  - 없음
- 결과값
  -  없음

***



## InitialContributor Vault

- LYDA InitialContributor : 0xD99c6726F967cc2f177246Fc854b343fd8EefD94  [link](https://etherscan.io/address/0xD99c6726F967cc2f177246Fc854b343fd8EefD94#writeProxyContract#F3)

### 함수 

### claim(address _to, uint256 _amount)

 토큰을 청구한다.

- 파라미터
  - address _to: 토큰을 받을 계정주소
  - address _amount:  청구하는 토큰 양 
- 결과값
  -  없음

***

