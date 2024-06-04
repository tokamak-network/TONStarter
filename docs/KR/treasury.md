# Treasury

> TreasuryProxy 컨트랙을 통해, 본인이 보유하고 있는 TOS를 이더로 환전할 수 있습니다.



| 기능 | 설명 | 방법 |
| -------- | -------- | -------- |
| 환전     | 토스를 이더로 환전함     | - 함수 claim(uint256 tosAmount)<br/>- 파라미터<br/>    ◦ uint256 tosAmount : 토스양 (wei uint, 18 decimals)|
| 이더 환전 금액 조회     | 입력된 토스량 따른 이더 환산 량     | - 함수 claimableEther(uint256 tosAmount)<br/>- 파라미터<br/>    ◦ uint256 tosAmount: 토스양 (wei uint, 18 decimals) <br/>- 결과<br/>    ◦ 환전될때 받을 수 있는 이더량     |
| 1토스당 이더 환전 금액 조회     | 1토스당 환전 이더 양 조회     | - 함수 backingRateETHPerTOS()<br/>- 파라미터<br/>   - 결과 <br/>    ◦ 1토스당 환전되는 이더양  (wei uint, 18 decimals)    |
| 환전 중지/시작 실행 하기     | PolicyOwner 만 실행 가능한 함수임. 환전 기능을 중지 시키거나 재개하는 함수입니다.| - 함수 setClaimPause(bool _pause)<br/> - 파라미터<br/>     ◦ bool _pause : true면 환전중지, false면 환전가능     |
| 환전 시작 시간 설정 하기     | PolicyOwner 만 실행 가능한 함수임. 환전 시작 시간을 설정하는 함수입니다.     | - 함수 setClaimableStartTime(uint32 _startTime)<br/>- 파라미터<br/>    ◦ uint32 _startTime : 환전 시작시간     |

