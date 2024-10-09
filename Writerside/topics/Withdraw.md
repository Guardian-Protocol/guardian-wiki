# Withdraw

The final process of the staking is the withdraw and you can come and withdraw your tokens on the withdraw section in
the guardian dapp

![withdraw.png](withdraw_page.png)

When the unstake process end, you can come and click the claim button, to get your original tokens plus the rewards 
generated on the protocol once the `withdraw` was claimed the card will disappear and your tokens will be reflected on 
your wallet.

<note>This transaction does not need a gas fee</note>
<warning>You need wait 7 days until you can withdraw your tokens</warning>

## Architecture

![withdraw.png](withdraw.png)

When the user click the claim button, the proxy `withdraw the unbounded` value across the proxy pallet and at the same time
sends the `withdrawal messag`e to the smart contract and this last one burn the unstaked gVARA tokens in order to keep the 
relationship 1:1 with the VARA token