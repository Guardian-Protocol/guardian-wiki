# Unstake

In order to unstake your vara you can go to the unstake section on the guardian dapp

![unstake_page.png](unstake_page.png)

Here you can come and unstake your vara that has been staked before,

<note>This transaction does not need a gas fee</note>
<warning>You need wait 7 days until you can withdraw your tokens</warning>

> Here are a few things that is important to note: 
> - You can't revert the unstake process
> - you will be able to unstake all of your `gVara`
> - The token value evolve his price in proportion of the staking quantity so the price it will variate

## Architecture

![unstake.png](unstake.png)

In order to unstake your vara, when you make the unstake action that will not have gas cost, the guardian proxy will
send the `unbound vara` transaction and at the same time the proxy will send the `unstake message` to the contract.

Your gVARA will be transferred from your wallet and sent to the smart contract that will retain the tokens until the
unstake process end.