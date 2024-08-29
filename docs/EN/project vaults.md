# Launched Project’s Vaults

> The vault contracts of previously launched projects hold project tokens and vaults to be used for their respective purposes.


## Token Addresses by Project

|Token Symbol	|Token Address	|etherscan|
| -------- | -------- | -------- |
| LYDA | 0xE1B0630D7649CdF503eABc2b6423227Be9605247 | [link](https://etherscan.io/address/0xE1B0630D7649CdF503eABc2b6423227Be9605247) |
| AURA | 0xaEC59E5b4f8DbF513e260500eA96EbA173F74149 | [link](https://etherscan.io/address/0xaEC59E5b4f8DbF513e260500eA96EbA173F74149) |
| DOC | 0x0e498afce58dE8651B983F136256fA3b8d9703bc | [link](https://etherscan.io/address/0x0e498afce58dE8651B983F136256fA3b8d9703bc) |



## PublicSale Vault 

- AURA PublicSale: 0x3B75d3f628C29d357b484EA7d091faEd63419267 : [link](https://etherscan.io/address/0x3B75d3f628C29d357b484EA7d091faEd63419267#writeProxyContract#F4)
- DOC PublicSale: 0xBef737D725993847c345647ebA096500FdAE71c6 : [link](https://etherscan.io/address/0xBef737D725993847c345647ebA096500FdAE71c6#writeProxyContract#F4)
- LYDA PublicSale: 0x3ba5c96665960ABD931858b8D80Ec80f53F2A09c: [link](https://etherscan.io/address/0x3ba5c96665960ABD931858b8D80Ec80f53F2A09c#writeProxyContract#F5)

### Functions

### claim()
Claim tokens.
- Parameters
    - None
- Return value
    - None
***



## Liquidity Vault 

- LYDA Liquidity: 0xf972657e6331e19ffcD1424a275215f7ab1A8df5:  [link](https://etherscan.io/address/0x620c86FD58E40f534545Aa433f49eF0271755E17#writeProxyContract#F6)

### Functions
### mint(uint256 tosAmount)
Add liquidity
- Parameters
    - uint256 tosAmount : Input TOS amount (wei unit, 18 decimals)
- Return value
    - None

## TONStaker Vault

- LYDA TONStaker: 0x620c86FD58E40f534545Aa433f49eF0271755E17:  [link](https://etherscan.io/address/0xf972657e6331e19ffcD1424a275215f7ab1A8df5#writeProxyContract#F4)

### Functions
### claim()
Send tokens to the token distribution contract to airdrop tokens to TON Stakers.
- Parameters
    - None
- Return value
    - None
***

## TOSStaker Vault
- LYDA TOSStaker:  0xBb49719A0bC10bf9E8f0B5e2d0F74dEE830a0090 : [link](https://etherscan.io/address/0xBb49719A0bC10bf9E8f0B5e2d0F74dEE830a0090#writeProxyContract#F4)

### Functions
### claim()
Send tokens to the token distribution contract to airdrop tokens to TOS Stakers.
- Parameters
    - None
- Return value
    - None
***

## WTON-TOS LP Reward Vault

- LYDA's WTON-TOS LP Reward :  0xA31945830C5a6B225A81962a10E78D2e3793D72D : [link](https://etherscan.io/address/0xA31945830C5a6B225A81962a10E78D2e3793D72D#writeProxyContract#F8)

### Functions
### createProgram()
Create a program to provide rewards to LPs of the Uniswap V3 WTON-TOS pool.

- Parameters
    - None
- Return value
    - None
***

## LYDA-TOS LP Reward Vault

- LYDA's LYDA-TOS LP Reward : 0x45D08f522BF2b6455Fe7EeF0f4aDf865D76EaD08  : [link](https://etherscan.io/address/0x45D08f522BF2b6455Fe7EeF0f4aDf865D76EaD08#writeProxyContract#F8)

### Functions
### createProgram()
Create a program to provide rewards to LPs of the Uniswap V3 LYDA-TOS pool.
- Parameters
    - None
- Return value
    - None
***



## InitialContributor Vault

- LYDA InitialContributor : 0xD99c6726F967cc2f177246Fc854b343fd8EefD94  [link](https://etherscan.io/address/0xD99c6726F967cc2f177246Fc854b343fd8EefD94#writeProxyContract#F3)

### 함수 
### Functions
### claim(address _to, uint256 _amount)
Claim tokens.
- Parameters
    - address _to: Account address to receive tokens
    - address _amount: Amount of tokens to claim
- Return value
    - None

***

