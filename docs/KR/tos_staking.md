# TOS 스테이킹 관련 함수

> StakingV2Proxy 컨트랙을 통해 스테이킹, 언스테이킹을 할 수 있습니다.
- Mainnet StakingV2Proxy : [etherscan link](https://etherscan.io/address/0x14fb0933ec45ece75a431d10afaa1ddf7bfee44c#readProxyContract)

![Write as Proxy 선택](https://github.com/tokamak-network/TONStarter/blob/develop/img/tos_staking_0.png)

위의 이더스캔 링크 페이지의 Write as Proxy 페이지에서 실행 가능한 함수를 확인하실 수 있습니다.



| 기능 | 설명 | 방법 |
| -------- | -------- | -------- |
| TOS 스테이킹 (락업기간 지정하지 않음)      | 토스 스테이킹 실행      |- 함수 stake(uint256 _amount) <br/>- 파라미터<br/>    ◦ uint256 _amount : 스테이킹 양 <br/>- 결과<br/>    ◦  uint256 stakeId : 스테이킹 아이디|
| 락업기간 지정해서, 스테이킹 하기      | 락업기간(스테이킹 종료일을) 설정하여 스테이킹 실행      | - 함수 stakeGetStos(uint256 _amount, uint256 _periodWeeks) <br/>- 파라미터<br/>    ◦uint256 _amount : 스테이킹 양 <br/>◦uint256 _periodWeeks : 락업기간(주단위)<br/>- 결과 uint256 stakeId: 스테이킹 아이디     |
| 추가 스테이킹 (종료일 없는 경우)      | 락업기간 지정하지 않고 스테이킹 한 경우의 토스 추가 스테이킹      | - 함수  function increaseAmountForSimpleStake(uint256 _stakeId, uint256 _amount)<br/>- 파라미터<br/>    ◦ _stakeId stake id<br/>    ◦ _amount  TOS amount<br/>      |
| 추가 스테이킹 ( 종료일이 있는 경우)      | 락업기간이 있는 스테이킹의 경우, 락업 기간 종료전에 추가 스테이킹 하기      | - 함수 resetStakeGetStosAfterLock(uint256 _stakeId, uint256 _addTosAmount, uint256 _periodWeeks)   <br/>- 파라미터<br/>    ◦ _stakeId     stake id<br/>◦ _addTosAmount   additional TOS to be staked<br/>◦ _periodWeeks lockup period |
| 스테이킹 ( 특정 스테이킹 아이디로 스테이킹)     | 락업종료일이 지났거나 없는 경우, 특정 스테이킹 아이디에 스테이킹 하기     | - 함수  increaseBeforeEndOrNonEnd(uint256 _stakeId, uint256 _amount, uint256 _unlockWeeks) <br/>- 파라미터<br/>    ◦_stakeId     stake id <br/> ◦ _amount      additional TOS to be staked<br/> ◦ _unlockWeeks additional lockup period<br/> |
| 언스테이킹     | 언스테이킹하여, 이자와 원금 인출하기     | - 함수  unstake(uint256 _stakeId) <br/>- 파라미터<br/>    ◦ _stakeIds stake id  |
| 클래임     | 이자 인출하기     | - 함수  claimForSimpleType(uint256 _stakeId, uint256 claimLtos) <br/>- 파라미터<br/>    ◦ _stakeId  stake id <br/> ◦ claimLtos amount of LTOS to claim<br/>|

