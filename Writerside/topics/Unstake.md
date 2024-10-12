# Unstake

To unstake your Vara, you can go to the unstake section on the Guardian dApp. Here, you can unstake your previously 
staked Vara.

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

The unstake action does not require a gas fee. The Guardian proxy will initiate the unstake transaction for the unbound 
Vara and, at the same time, send an unstake message to the contract. Your gVara will be transferred from your wallet to
the smart contract, where it will be held until the unstaking process is complete.