# LTOS 조회 방법

> LTOS는 TOS를 스테이킹 했을 때 발행되는 토큰입니다.
> StakingV2Proxy 컨트랙을 통해 LTOS 잔액을 조회할 수 있습니다.

- Mainnet StakingV2Proxy : [etherscan link](https://etherscan.io/address/0x14fb0933ec45ece75a431d10afaa1ddf7bfee44c#readProxyContract)

![Read as Proxy 선택](https://github.com/tokamak-network/TONStarter/blob/develop/img/query_ltos_0.png)

Read as Proxy 페이지의 함수를 통해 아래와 같은 기능을 실행할 수 있습니다.

| 기능 | 설명 | 방법 |
| -------- | -------- | -------- |
| LTOS 잔액 조회     | 특정 계정의 LTOS 잔액 조회     | - 함수 balanceOf(address _addr)<br/>- 파라미터<br/>    ◦ address _addr : 조회대상이 되는 계정주소<br>- return<br>    ◦ uint256 balance : LTOS 잔액     |
| LTOS를 TOS 변환     | 얼마의 LTOS를 TOS로 환산했을 때, TOS 양을 알 수 있습니다.       | - 함수   getLtosToTosPossibleIndex(uint256 ltos)<br/>- 파라미터 <br/>    ◦ uint256 ltos:  LTOS 양<br/>- 결과 uint256 : 변환된 TOS 양     |
| 스테이킹 아이디 목록 조회     | 특정 계정이 스테이킹한 스테이킹 아이디 목록을 조회합니다.      | - 함수  stakingOf(address _addr)<br/>- 파라미터<br/>    ◦ address _addr : 조회대상이 되는 계정주소<br/>- 결과<br/>    ◦ uint256[] memory : 아이디 배열을 리턴합니다.<br/>    ◦ 첫번째 인덱스는 락업기간이 없이 스테이킹한 아이디입니다. 락업기간을 정하지 않고 스테이킹한 것이 없는 경우, 첫번째 인덱스가 0이거나 null 입니다.     |
| 특정 스테이킹 아이디의 TOS 양 조회      | 특정 스테이킹 아이디가 보유하고 있는 TOS양을 조회합니다.      | - 함수  stakedOf(uint256 stakeId)<br/>- 파라미터<br/>    ◦ uint256 stakeId : 스테이킹 아이디<br/>- 결과<br/>    ◦ uint256 :  TOS 양     |
| 스테이킹된 총 LTOS 조회    | 스테이킹된 총 LTOS양을 조회합니다.      | - 함수 :  totalLtos()<br/>- 파라미터 : 없음<br/>- 결과 : 스테이킹된 총 LTOS 양     |
| 스테이킹된 총 TOS 양 조회     | 스테이킹된 총 TOS 양을 조회합니다.      | - 함수 :  stakedOfAll()<br/>- 파라미터 : 없음<br/>- 결과 : 스테이킹된 총 TOS 양     |



