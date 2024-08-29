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
## Airdrop distributed to sTOS holders

- Contract: LockTOSDividendProxy [0x17332F84Cc0bbaD551Cd16675F406A0a2c55E28C](https://etherscan.io/address/0x17332f84cc0bbad551cd16675f406a0a2c55e28c)

### Conducting an airdrop (token distribution)

Before distributing tokens, you must **pre-approve the LockTOSDividendProxy address for the amount of tokens to be distributed.**

- Function: [distribute](https://etherscan.io/address/0x17332f84cc0bbad551cd16675f406a0a2c55e28c#writeProxyContract#F5)
- token: token address
- amount: amount of tokens to distribute

### Checking claimable airdrop amount

- Function: [claimable](https://etherscan.io/address/0x17332f84cc0bbad551cd16675f406a0a2c55e28c#readProxyContract#F6)
- _account: address to receive the airdrop
- _token: token address

### Claiming the airdrop

- Function: [claim](https://etherscan.io/address/0x17332f84cc0bbad551cd16675f406a0a2c55e28c#writeProxyContract#F2)
- _token: token address

## Airdrop for TON stakers

This feature is currently discontinued. The AURA token has conducted two airdrops through this contract. Eligible participants can claim the distributed AURA through the claim function.

- Contract : TokenDividendPoolProxy [0x06245F89576536E9cF844C5804a8ad1CCeDb2642](https://etherscan.io/address/0x06245f89576536e9cf844c5804a8ad1ccedb2642)

### Checking claimable airdrop amount

- Function: [claimable](https://etherscan.io/address/0x06245f89576536e9cf844c5804a8ad1ccedb2642#readProxyContract#F5)
- _token: token address (for AURA, 0xaEC59E5b4f8DbF513e260500eA96EbA173F74149)
- _account: address to receive the airdrop

### Claiming the airdrop

- Function: [claim](https://etherscan.io/address/0x06245f89576536e9cf844c5804a8ad1ccedb2642#writeProxyContract#F2)
- _token: token address (for AURA, 0xaEC59E5b4f8DbF513e260500eA96EbA173F74149)