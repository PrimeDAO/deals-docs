# Create, conduct and participate in a deal on Gnosis Safe

## Prime Deals as a Gnosis Safe App

Prime Deals is also accessible as an embedded app from the Safe App interface in [Gnosis Safe](https://gnosis-safe.io/). This allows DAOs to use a Gnosis Safe multi-sig wallet as a Deal Representative, ideally using the same address as the DAO Treasury address (recommended).

Using Gnosis Safe couples even deeper governance processes already exising in a DAO with the negotiation flow enabled by Prime Deals, reducing coordination costs and allowing a smoother interaction.

With the Prime Deals Safe App you can initiate and conduct deals in the same way is documented for the normal webapp ~ so you can reference the rest of the documentation as well once you understood the key differences in the workflow with the Safe App.

With the Safe App a DAO can directly deposit their tokens from the multi-sig wallet into the DaoDepositManager module of the Prime Deals smart contract.

By using the Safe App a DAO would need to add the multi-sig as as a sole Representative for that DAO. More Representatives can be added from the webapp during the creation of a deal but that in the vast majority of the cases DAOs will only have one multi-sig Representative to vote, fund, claim or withdraw the tokens.

## How to use Prime Deals Safe App
1. Search for "Prime Deals" in the "Apps" section in the [Gnosis Safe](https://gnosis-safe.io/), and click on it.
2. Accept the disclaimer and authenticate with the multi-sig to Prime Deals
3. A "signMessage" transaction will be created and it needs to be approved
4. Once approved you are authenticated to Prime Deals
5. You can now interact with the app, voting as well as depositing, claiming and withdrawing tokens will work in the same way as described in the other section of Prime Deals documentation. Just remind that Unlocking, depositing, withdrawing etc. will generate corresponding transactions on the Gnosis App ("approve", "deposit", "claimDealVestings"), that follow the same flow as step 3.
7. Happy swapping!


## Known issues
### I have to wait for another approval, can I close the app, and come back later?
Yes you can. Multi-sig approval can take some time. User can close the app or keep it open as regardless, they don't have to wait for the approval to be finished once a transaction has been signed.

### "signMessage" transaction in step 3. was rejected, the app is telling me to wait for an approval, how can I authenticate again?
Clear your localStorage (you can just delete the Prime deals entry) and try to authenticate again.

### A transaction was rejected (e.g. unlock, deposit, withdraw), how can I resubmit it?
Please resubmit the desired action in the Prime Deals UI. A new transaction will be created that can be signed again.

### I triggered an action, and closed the app, or my browser crashed, do I have to re-trigger the action when I revisit the app?
No, wait as the UI will automatically update once the transaction has been successfully approved.

