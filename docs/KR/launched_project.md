# Launched Project’s Vaults

> 기존의 런칭된 프로젝트의 볼트 컨트랙은 각 목적에 맞게 사용되기 위해 프로젝트 토큰과 볼트를 보유하고 있습니다.

## 프로젝트별 토큰 주소

|토큰 심볼	|토큰 주소	|etherscan|
| -------- | -------- | -------- |
| LYDA | 0xE1B0630D7649CdF503eABc2b6423227Be9605247 | [link](https://etherscan.io/address/0xE1B0630D7649CdF503eABc2b6423227Be9605247) |
| AURA | 0xaEC59E5b4f8DbF513e260500eA96EbA173F74149 | [link](https://etherscan.io/address/0xaEC59E5b4f8DbF513e260500eA96EbA173F74149) |
| DOC | 0x0e498afce58dE8651B983F136256fA3b8d9703bc | [link](https://etherscan.io/address/0x0e498afce58dE8651B983F136256fA3b8d9703bc) |


## LYDA 볼트 주소 및 함수

|컨트랙 이름	|Address	|etherscan|
| -------- | -------- | -------- |
|PublicSale	|0x3ba5c96665960ABD931858b8D80Ec80f53F2A09c	|[link](https://etherscan.io/address/0x3ba5c96665960ABD931858b8D80Ec80f53F2A09c)|
|Liquidity|	0x620c86FD58E40f534545Aa433f49eF0271755E17	|[link](https://etherscan.io/address/0x620c86FD58E40f534545Aa433f49eF0271755E17)|
|TONStaker|	0xf972657e6331e19ffcD1424a275215f7ab1A8df5|	[link](https://etherscan.io/address/0xf972657e6331e19ffcD1424a275215f7ab1A8df5)|
|TOSStaker|	0xBb49719A0bC10bf9E8f0B5e2d0F74dEE830a0090|	[link](https://etherscan.io/address/0xBb49719A0bC10bf9E8f0B5e2d0F74dEE830a0090)|
|WTON-TOS LP Reward|	0xA31945830C5a6B225A81962a10E78D2e3793D72D	|[link](https://etherscan.io/address/0xA31945830C5a6B225A81962a10E78D2e3793D72D)|
|LYDA-TOS LP Reward|0x45D08f522BF2b6455Fe7EeF0f4aDf865D76EaD08 |[link](https://etherscan.io/address/0x45D08f522BF2b6455Fe7EeF0f4aDf865D76EaD08)|
|InitialContributor|0xD99c6726F967cc2f177246Fc854b343fd8EefD94|[link](https://etherscan.io/address/0xD99c6726F967cc2f177246Fc854b343fd8EefD94)|


## AURA PublicSale
|컨트랙 이름	|Address	|etherscan|
| -------- | -------- | -------- |
|PublicSale	|0x3B75d3f628C29d357b484EA7d091faEd63419267	|[link](https://etherscan.io/address/0x3B75d3f628C29d357b484EA7d091faEd63419267)|


## DOC PublicSale
|컨트랙 이름	|Address	|etherscan|
| -------- | -------- | -------- |
|PublicSale	|0xBef737D725993847c345647ebA096500FdAE71c6	|[link](https://etherscan.io/address/0xBef737D725993847c345647ebA096500FdAE71c6)|



## 함수


| 컨트랙(볼트) | 기능 | 방법 |
| -------- | -------- | -------- |
| PublicSale     | 클래임     |- 함수 function claim()      |
| Liquidity     | 유동성 추가하기     |- 함수function mint(uint256 tosAmount)<br/>- 파라미터 <br/>    ◦ uint256 tosAmount : 입력 토스 양 (wei unit, 18 decimals)|
| TONStaker     | 클래임     |- 함수 function tgeClaim(address _account) <br/>- 파라미터 <br/>    ◦ address _account: 계정 주소|
| TOSStaker     | 클래임     |- 함수 function tgeClaim(address _account) <br/>- 파라미터 <br/>    ◦ address _account: 계정 주소|
| LP Reward     | 리워드 프로그램 생성하기      | Text     |
| InitialContributor     | 클래임     |- 함수 function tgeClaim(address _account) <br/>- 파라미터 <br/>    ◦ address _account: 계정 주소|

