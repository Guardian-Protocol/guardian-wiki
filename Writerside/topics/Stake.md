# Stake
How it works: Stake vara and receive 1:1 gVARA, easy right? \
On the Guardian page, you will be able to stake your vara on the stake section.

![stake_page.png](stake_page.png)

<note>This transaction have a gas cost</note>

> Here are a few things that is important to note: 
> - You can't have less than 1 token on the VARA network 
>   -  so, the `MAX` button take the max amount -1 VARA
> - You can't send a 0 stake transaction 
> - You need wait on the page until the transaction ends

## Architecture

In order to stake vara on the guardianDeFi the guardian team develop an architecture
that will automate all the staking process.

The following image explain the staking process

![stake.png](stake.png)

First the user sends their vara to a GuardianProxy a proxy, this proxy stakes the user vara and at the same time
sends a transaction to a LiquidContract this contract handle the transaction and then mint the 1:1 gVARA
to the user wallet.