# Stake
How it works: Stake Vara and receive gVara — simple, right? \
\
On the Guardian page, you will be able to stake your Vara in the staking section. The team has developed an 
architecture that automates the entire staking process.

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

The following image explains the staking process:

![stake.png](stake.png)

First, the user sends their Vara to a Guardian proxy. This proxy stakes the user's Vara and simultaneously sends a 
transaction to a LiquidContract. This contract manages the transaction and then mints the gVara to the user’s wallet.