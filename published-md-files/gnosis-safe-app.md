# Create, conduct and participate in a deal on Gnosis Safe

## Prime Deals as a Gnosis Safe App

Prime Deals is also accessible as an embedded app from the Safe App interface in [Gnosis Safe](https://gnosis-safe.io/). This allows DAOs to use a Gnosis Safe multi-sig wallet as a Deal Representative, ideally using the same address as the DAO Treasury address (recommended).

Using Gnosis Safe couples even deeper governance processes already exising in a DAO with the negotiation flow enabled by Prime Deals, reducing coordination costs and allowing a smoother interaction.

With the Prime Deals Safe App you can initiate and conduct deals in the same way is documented for the normal webapp ~ so you can reference the rest of the documentation as well once you understood the key differences in the workflow with the Safe App.

## Voting, Funding, Claiming and Withdrawing with the Safe App
With the Gnosis Safe App a DAO can directly deposit their tokens from the multi-sig wallet into the `DaoDepositManager` module of the Prime Deals smart contract.

Normally, without the Safe App, the DAO would have to make sure that the DAO Representative(s) have the tokens to fund the deal which would normally require the extra step of moving the funds from the Treasury to the Representatives before ultimately deposit these funds into the deal. Instead, by using the Safe App, a DAO would only need to add the multi-sig as as a sole Representative for that DAO in order to be able to directly fund the deal. It goes without saying that this is a faster and leaner process as the DAO would likely want to appoint as sole Representative the multi-sig which is also the treasury address. Intuitively, the voting process will also rely on the already existing alignment of the respective DAOs' governance systems.

If needed more Representatives can be added from the webapp during the creation of a deal but by using the Safe App this is no longer necessary as a DAO will only need one multi-sig Representative to vote, fund, claim or withdraw the tokens. Also please note that you can sign the multi-sig or another address as the Proposal Lead. It's completely up to you.

## How to use Prime Deals Safe App
1. Search for 'Prime Deals' in the 'Apps' section in the [Gnosis Safe](https://gnosis-safe.io/), and click on it.
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">N.B. If you don't find the App in the Safe marketplace, you can always add it as a custom app by clicking on <kbd>Add custom app</kbd> on the top of the 'All Apps' view in the 'Apps' section. You will be prompted to provide the App URL. You can use `https://deals.prime.xyz`.</div>
2. Accept the disclaimer and authenticate with the multi-sig to Prime Deals
3. A `signMessage` transaction will be created and it needs to be approved
4. Once approved you are authenticated to Prime Deals
5. You can now interact with the app, voting as well as depositing, claiming and withdrawing tokens will work in the same way as described in the other section of Prime Deals documentation. 
Just remind that unlocking, depositing, withdrawing etc. will generate corresponding transactions on the Safe App (`approve`, `deposit`, `claimDealVestings`), that follow the same flow as step 3.
7. Happy swapping!




## Known issues
### I have to wait for another approval, can I close the app, and come back later?
Yes you can. Multi-sig approval can take some time. User can close the app or keep it open as regardless, they don't have to wait for the approval to be finished once a transaction has been signed.

### `signMessage` transaction in step 3. was rejected, the app is telling me to wait for an approval, how can I authenticate again?
Clear your `localStorage` from your browser's DevTools and try to authenticate again. You can just delete the Prime deals key-value pair. 

### A transaction was rejected (e.g. unlock, deposit, withdraw), how can I resubmit it?
Please resubmit the desired action in the Prime Deals UI. A new transaction will be created that can be signed again.

### I triggered an action, and closed the app, or my browser crashed, do I have to re-trigger the action when I revisit the app?
No, wait as the UI will automatically update once the transaction has been successfully approved.

