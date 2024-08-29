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

모든 TON Mining 컨트랙은  톤 스테이킹 할 수 있는 기간이 종료되었습니다. 
TON Mining 컨트랙은 이자 (TOS) 클래임과 TON 원금을 인출 할 수 있는 기능을 제공합니다.



## 실행함수

### withdraw()

마이닝 종료 블록이 지난 후에 스테이킹 한 톤과 운영이익(레이어2의 시뇨리지로 받은 TOS)을 인출한다.

- 파라미터
  - 없음
- 결과값
  -  없음

***

### claim() 

마이닝 종료 블록이 지난 후에 이자 TOS를 인출한다.

- 파라미터
  - 없음
- 결과값
  -  없음

***



## 조회함수

### canRewardAmount(address account, uint256 specificBlock) 

받을 수 있는 이자를 조회한다.

- 파라미터
  - address account: 조회하려는 계정 주소
  - uint256 specificBlock: 조회하려는 시점의 블록 번호
- 결과값
  -  uint256: 받을 수 있는 이자 (wei unit, 18 decimals)

***

### userStaked(address account) 

계정의 스테이킹 정보 확인

- 파라미터
  - address account: 조회하려는 계정 주소 
- 결과값
  - uint256 amount  입금한 톤 양 (wei unit, 18 decimals)
  - uint256 claimedBlock 클래임한 블록 
  - uint256 claimedAmount  클래임한 금액 (wei unit, 18 decimals) 
  - uint256 releasedBlock  인출한 블록 
  - uint256 releasedAmount 인출한 톤 양 
  - uint256 releasedTOSAmount 인출한 토스 양 (wei unit, 18 decimals) 
  - bool released   true이면 인출완료. false이면 인출안함

***

### totalStakers()  

총 스테이킹한 계정 수 조회

- 파라미터
  - 없음
- 결과값
  -  uint256: 총 스테이킹한 계정 수

***

### totalStakedAmount()

총 스테이킹한 계정 수 조회

- 파라미터
  - 없음
- 결과값
  -  uint256: 총 스테이킹된 양 (wei unit, 18 decimals)

***

### startBlock()

마이닝 시작블록 조회

- 파라미터
  - 없음
- 결과값
  -  uint256: 시작블록 번호

***

### endBlock()

마이닝 종료블록 조회

- 파라미터
  - 없음
- 결과값
  -  uint256: 종료블록 번호

***

