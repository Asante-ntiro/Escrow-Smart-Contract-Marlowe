# Escrow-Smart-Contract-Marlowe

This file contains code for a smart contract written in [DAML](https://daml.com/), a programming language for writing distributed applications. The contract is for a simple escrow between a seller and a buyer, with the option for a mediator to resolve disputes. The contract specifies the following steps:

1. The seller deposits a token and specifies a price.
2. The buyer has the option to either confirm the purchase or report a problem.
3. If the buyer confirms the purchase, the contract closes and the transaction is complete.
4. If the buyer reports a problem, the seller has the option to either confirm or dispute the problem.
5. If the seller confirms the problem, the contract closes and the buyer is refunded.
6. If the seller disputes the problem, the mediator has the option to either dismiss the claim or confirm it.
7. If the mediator dismisses the claim, the buyer is refunded and the contract closes.
8. If the mediator confirms the claim, the contract closes.

The contract also includes time parameters for dispute response and mediation deadlines.

To use this contract, you will need to have a DAML interpreter and ledger set up. Please refer to the [DAML documentation](https://docs.daml.com/) for more information.
