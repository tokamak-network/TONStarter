# TOS Mining
> TONStarter > In the TOS Mining menu, there are 5 lock-up products for staking TON and mining TOS.
## TOS Mining contract addresses

| name | address | etherscan|
| -------- | -------- | -------- |
| TON #1     | 0x9a8294566960Ab244d78D266FFe0f284cDf728F1     | [link](https://etherscan.io/address/0x9a8294566960Ab244d78D266FFe0f284cDf728F1#readProxyContract)     |
| TON #2     | 0x7da4E8Ab0bB29a6772b6231b01ea372994c2A49A     | [link](https://etherscan.io/address/0x7da4e8ab0bb29a6772b6231b01ea372994c2a49a#readProxyContract)       |
| TON #3     | 0xFC1fC3a05EcdF6B3845391aB5CF6a75aeDef7CeA     | [link](https://etherscan.io/address/0xfc1fc3a05ecdf6b3845391ab5cf6a75aedef7cea#readProxyContract)       |
| TON #4     | 0x9F97b34161686d60ADB955ed63A2FC0b2eC0a2a9     | [link](https://etherscan.io/address/0x9f97b34161686d60adb955ed63a2fc0b2ec0a2a9#readProxyContract)       |
| TON #5     | 0x21Db1777Dd95749A849d9e244136E72bd93082Ea     | [link](https://etherscan.io/address/0x21Db1777Dd95749A849d9e244136E72bd93082Ea#readProxyContract)       |

The staking period for all TON Mining contracts has ended. TON Mining contracts provide functions to claim interest (TOS) and withdraw TON principal.

## How to Execute Functions through MyCrypto
Since the functions below do not appear on Etherscan for the above contracts, I will explain how to execute these functions through the MyCrypto site.

After logging into the MyCrypto site, go to [TOOLS > Contracts](https://app.mycrypto.com/interact-with-contracts), and you will see the following screen:

![MyCrypto Tools > Contracts](../img/tos-mining-0.png)

- Contract: Enter the address of the relevant contract above.
- ABI/JSON Interface: If there is existing data, delete it and enter the content below.
  ```
  [
    {
        "inputs": [],
        "name": "withdraw",
        "outputs": [],
        "stateMutability": "nonpayable",
        "type": "function"
      },
      {
        "inputs": [],
        "name": "claim",
        "outputs": [],
        "stateMutability": "nonpayable",
        "type": "function"
      },
      {
        "inputs": [
          {
            "internalType": "address",
            "name": "account",
            "type": "address"
          },
          {
            "internalType": "uint256",
            "name": "specificBlock",
            "type": "uint256"
          }
        ],
        "name": "canRewardAmount",
        "outputs": [
          {
            "internalType": "uint256",
            "name": "",
            "type": "uint256"
          }
        ],
        "stateMutability": "view",
        "type": "function"
      },
      {
        "inputs": [
          {
            "internalType": "address",
            "name": "",
            "type": "address"
          }
        ],
        "name": "userStaked",
        "outputs": [
          {
            "internalType": "uint256",
            "name": "amount",
            "type": "uint256"
          },
          {
            "internalType": "uint256",
            "name": "claimedBlock",
            "type": "uint256"
          },
          {
            "internalType": "uint256",
            "name": "claimedAmount",
            "type": "uint256"
          },
          {
            "internalType": "uint256",
            "name": "releasedBlock",
            "type": "uint256"
          },
          {
            "internalType": "uint256",
            "name": "releasedAmount",
            "type": "uint256"
          },
          {
            "internalType": "uint256",
            "name": "releasedTOSAmount",
            "type": "uint256"
          },
          {
            "internalType": "bool",
            "name": "released",
            "type": "bool"
          }
        ],
        "stateMutability": "view",
        "type": "function"
      },
      {
        "inputs": [],
        "name": "totalStakers",
        "outputs": [
          {
            "internalType": "uint256",
            "name": "",
            "type": "uint256"
          }
        ],
        "stateMutability": "view",
        "type": "function"
      },
      {
        "inputs": [],
        "name": "totalStakedAmount",
        "outputs": [
          {
            "internalType": "uint256",
            "name": "",
            "type": "uint256"
          }
        ],
        "stateMutability": "view",
        "type": "function"
      },
      {
        "inputs": [],
        "name": "startBlock",
        "outputs": [
          {
            "internalType": "uint256",
            "name": "",
            "type": "uint256"
          }
        ],
        "stateMutability": "view",
        "type": "function"
      },
      {
        "inputs": [],
        "name": "endBlock",
        "outputs": [
          {
            "internalType": "uint256",
            "name": "",
            "type": "uint256"
          }
        ],
        "stateMutability": "view",
        "type": "function"
      }
  ]
  ```
Enter "StakeTON" under Contract Name.
Then, click the "Interact with Contract" button
![Interact with Contract](../img/tos-mining-1.png)

Below the button, you will see the "Read/Write Contract" title and function selection box as shown below.

![Read/Write Contract](../img/tos-mining-2.png)

For example, if you want to execute the Withdraw function, select 'withdraw' from the function selection box, enter your address in the account field, and click the Write button to execute the withdraw function.
![Read/Write Contract](../img/tos-mining-3.png)
## Executable functions

### withdraw()
After the mining end block has passed, withdraw the staked TON and operational profits (TOS received as seigniorage from Layer 2).

- Parameters
    - None
- Return Value
    - None

***

### claim() 

After the mining end block has passed, withdraw the interest TOS.

- Parameters
    - None
- Return Value
    - None
***



## Query Functions

### canRewardAmount(address account, uint256 specificBlock) 

Query the claimable interest.

- Parameters
    - address account: Account address to query
    - uint256 specificBlock: Block number of the query point
- Return Value
    - uint256: Claimable interest (wei unit, 18 decimals)

***

### userStaked(address account) 

Check the staking information of an account

- Parameters
    - address account: Account address to query
- Return Value
    - uint256 amount: Amount of TON deposited (wei unit, 18 decimals)
    - uint256 claimedBlock: Block when claimed
    - uint256 claimedAmount: Amount claimed (wei unit, 18 decimals)
    - uint256 releasedBlock: Block when withdrawn
    - uint256 releasedAmount: Amount of TON withdrawn
    - uint256 releasedTOSAmount: Amount of TOS withdrawn (wei unit, 18 decimals)
    - bool released: true if withdrawn, false if not withdrawn

***

### totalStakers()  
Query the total number of staking accounts

- Parameters
    - None
- Return Value
    - uint256: Total number of staking accounts
***

### totalStakedAmount()

Query the total staked amount

- Parameters
    - None
- Return Value
    - uint256: Total staked amount (wei unit, 18 decimals)

***

### startBlock()

Query the mining start block

- Parameters
    - None
- Return Value
    - uint256: Start block number

***

### endBlock()

Query the mining end block

- Parameters
    - None
- Return Value
    - uint256: End block number

***

