# TOS Mining
> 톤스타터 > TOS Mining 메뉴에서는 톤을 스테이킹하고 토스를 마이닝하는 락업 상품이 5개 존재합니다.

## TOS Mining 컨트랙 주소

| 이름 | address | etherscan|
| -------- | -------- | -------- |
| TON #1     | 0x9a8294566960Ab244d78D266FFe0f284cDf728F1     | [link](https://etherscan.io/address/0x9a8294566960Ab244d78D266FFe0f284cDf728F1#readProxyContract)     |
| TON #2     | 0x7da4E8Ab0bB29a6772b6231b01ea372994c2A49A     | [link](https://etherscan.io/address/0x7da4e8ab0bb29a6772b6231b01ea372994c2a49a#readProxyContract)       |
| TON #3     | 0xFC1fC3a05EcdF6B3845391aB5CF6a75aeDef7CeA     | [link](https://etherscan.io/address/0xfc1fc3a05ecdf6b3845391ab5cf6a75aedef7cea#readProxyContract)       |
| TON #4     | 0x9F97b34161686d60ADB955ed63A2FC0b2eC0a2a9     | [link](https://etherscan.io/address/0x9f97b34161686d60adb955ed63a2fc0b2ec0a2a9#readProxyContract)       |
| TON #5     | 0x21Db1777Dd95749A849d9e244136E72bd93082Ea     | [link](https://etherscan.io/address/0x21Db1777Dd95749A849d9e244136E72bd93082Ea#readProxyContract)       |


## 함수
모든 TON Mining 컨트랙은  톤 스테이킹 할 수 있는 기간이 종료되었습니다.
TON #1은 마이닝은 20165180 Block 까지 진행됩니다.
TON Mining 컨트랙은 이자 (TOS) 클래임과 TON 원금을 인출 할 수 있는 기능(withdraw())을 제공합니다.


| 기능 | 설명 | 방법 |
| -------- | -------- | -------- |
| 총 스테이킹된 양 조회     | the total staked amount     | - 함수 totalStakedAmount()     |
| 토스 마이닝 시작블록 조회     | the staking start block, once staking starts, users can no longer apply for staking.     | - 함수 startBlock()     |
| 토스 마이닝 종료블록 조회     | endBlock()     | - 함수 endBlock()     |
| 스테이킹한 상태의 계정 수     | 총 스테이킹한 계정 수 조회     | - 함수 totalStalers()     |
| 스테이킹 정보 확인     | 계정의 스테이킹 정보 확인     | - 함수 userStaked(address account)<br/>- 파라미터<br/>- 결과 <br/>     ◦ uint256 amount  입금한 톤 양 <br/>     ◦ uint256 claimedBlock 클래임한 블록<br/>     ◦ uint256 claimedAmount  클래임한 금액<br/>     ◦ uint256 releasedBlock  인출한 블록<br/>     ◦ uint256 releasedAmount 인출한 톤 양<br/>     ◦ uint256 releasedTOSAmount 인출한 토스 양<br/>     ◦ bool released   true이면 인출완료. false이면 인출안함     |
| 이자 조회     | 받을 수 있는 이자 조회     | -  함수  canRewardAmount(address account, uint256 specificBlock)     |
| 인출     | 마이닝 종료 블록이 지난수, 스테이킹 한 톤과 이자 토스를 인출한다.     | -  함수  withdraw()     |
