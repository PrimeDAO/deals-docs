# Token Swap Module FAQ

## What is a Token Swap?

The Token Swap is the first product module available in Prime Deals and it allows to safely exchange tokens between two DAOs with customized vesting schedules. It can be initiated as an Open Proposal or as a Partnered Deal:

- an **Open Proposal** allows you to publicly offer a token swap to any DAO wants to propose a partnership deal based off the original offer you initially create.
- a **Partnered Deal** allows you to bring to the negotiation table two DAOs that are already aspiring to close a deal, and it simplifies the process of refine, finalize, and execute their agreement on-chain.

## What is a Primary DAO in a Token Swap?

A Primary DAO is the DAO for which the deal is originally initiated for. A Token Swap can be created by someone in the DAO, or someone outside the DAO.

## What is a Partner DAO in a Token Swap?

A Partner DAO is the DAO that is brought by a Primary DAO in a Partnered Deal, or whose offer to an Open Proposal is accepted by its Proposal Lead.

## What is a DAO Treasury Address in a Token Swap?

A DAO Treasury Address is the address that will receive tokens from the other DAO during the token swap. Whenever a vested amount is claimed (by anyone) these tokens are also being sent to the treasury address.

## In short, what is the process of a making a Token Swap happen on Prime Deals?

Here is an high-level summary of the most relevant steps in a Token Swap. For an in-depth walkthrough and for a more clear differentiation between Open Proposals and Partnered Deals, please refer to the relevant step-by-step tutorials [here](https://deals.prime.xyz/documentation/InitiateandconductaTokenSwap).

1. Decide if you want to start an Open Proposal or a Partnered Deal.
2. Provide a brief description of your proposal.
3. Specify the address of the Proposal Lead and (optionally) contact e-mail. This address will be allowed to edit the deal during the negotiation integrating new points from the conversation.
4. Decide whether you want to keep private or publicly accessible the details of a deal, please see [here](https://deals.prime.xyz/documentation/TokenSwapFAQ#privacy) for a detailed description of how privacy settings work. In the case of a Partnered Deal, this will make public or private the whole deal. In the case of an Open Proposal, this setting will make public or private only the incoming offers.
5. Fill-out the DAO details: the DAO treasury address that will receive the token after the swap, and a list of the address of the DAO representatives who will be able to cast a vote on the deal, either to accept or reject it, fund the deal, as well as claim tokens that will be sent to the treasury address, or withdraw funds they deposited on behalf of their DAO in case the deal is not successful. In case of a Partnered deal, fill-out the same general details for the other DAO.  If you don’t already have a partner DAO choose to start an Open Proposal in step 1., in this way you will be able to find many potential prospects: they will have to provide their own terms and select their own Deal Representatives.
6. Setup the details of the token that your DAO wants to swap. First, define how much of the tokens are instantly transferred to the other DAO versus how much of your token are vested. Then, configure the vesting schedule specifying over which period they’ll be vested and for how long they won’t be claimable by the other DAO. In case of a Partnered Deal define the same details and vesting schedule for the token they want to swap.
7. Define the Funding Period, the period of time after the Proposal Lead has declared voting complete, in which the Deal Representative must fully fund, and the Proposal Lead must execute the swap.
8. Define the terms of the deal by specifying the clauses that you want to seal in the agreement.
9.  Discuss with the two sets of Deal Representatives the clauses. (Note that in an Open Proposal anyone can connect with their address and discuss the clauses. Whereas in a Partnered Deal only Proposal Lead and Deal Representatives can, regardless if the deal is public or private.)
10.  Integrate the feedback of the discussion by editing the deal.
11.  With more than 50% affirmative votes per each DAO, the Proposal Lead may initiate the deal’s funding period. The complete funding of the deal needs to happen before the specified Funding Period ends.
12.  Let the DAOs’ Representatives to claim vested tokens on behalf of their DAO, or withdraw their deposit in the event the deal do not get fully funded by the end of the Funding Period.

![https://ik.imagekit.io/primedao/PrimeDeals/UML-DEALS-TS_k_Xho8YRS.jpg?ik-sdk-version=javascript-1.4.3&updatedAt=1651689966436](https://ik.imagekit.io/primedao/PrimeDeals/UML-DEALS-TS_k_Xho8YRS.jpg?ik-sdk-version=javascript-1.4.3&updatedAt=1651689966436)

## What a Proposal Lead can and cannot do?

A **Proposal Lead** is exclusively responsible for kickstarting:

- the deal by assembling the initial proposal
- edit the deal during the negotiation, integrating new points from the conversation
- initiate the Funding phase once the deal is approved
- unilaterally cancel the deal before a deal is approved
- changing the deal from private to public and vice versa

In addition the Proposal Lead, just like any Deal Representative, can discuss the clauses, and they can manually execute the token swap of a deal that has been fully funded.

Unless also listed as a Deal Representative, a Proposal Lead cannot cast a vote or fund a deal.

The Proposal Lead can be changed at any time until the deal is approved.

You don't need to be part of DAO to be a Proposal Lead (see [here](https://deals.prime.xyz/documentation/GeneralFAQ#daoplomat)).

## What are the pros and cons of keeping the Administrative Rights in an Open Proposal?

When you setup an Open Proposal the Proposal Lead has the chance to decide whether or not you want to keep the Administrative Rights in an Open Proposal.

If you toggle this option off, you will grant the right for the prospective partner DAO to determine the identity of Proposal Lead, to which the administrative rights will be transferred to.

It’s highly recommended that you transfer your administrative rights only if you anticipate too many incoming offers for this proposal and won't have time to manage them all.

Among others, the three most significant rights you are letting go are: 

- the ability to decide when to start the funding period
- the ability to cancel the deal and the ability to edit/amend the deal
- the ability to toggle the deal private/public

It’s also worth remembering that in the near future Prime Deals will feature a commission fee as incentive for DAOplomats that are successfully proposing and facilitating deals and so in that case, if you don’t keep Administrative Rights you will also lose that earning opportunity.

## What Deal Representatives can and cannot do?

Deal Representatives have the exclusive right to cast a vote on the deal, either to accept or reject the deal, they can deposit and withdraw funds, and claim tokens on behalf of their DAO. 

In addition the Deal Representatives, just like the Proposal Lead can discuss the clauses, and they can manually execute the token swap of a deal that has been fully funded.

A Deal Representative does not have all the exclusive rights of the Proposal Lead. In fact, a Deal Representative is cannot edit the deal during the negotiation, initiate the Funding phase or unilaterally cancel the deal.

Note that a Deal Representative can also abstain by non voting as this action is not mandatory. However, keep in mind that unless the Proposal Lead edits the deal, the Deal Representative won’t be able to revert to a neutral un-voted state if they already casted a vote. In this case then voting will be reset and the vote will be in a neutral un-voted state again for all Deal Representatives. 

A Deal Representative can change their vote from accept to reject and vice versa as many times as they want until the Negotiating phase is going on, but beware the deal can only move forward from the Negotiating phase to the Funding phase when at least 50% of the Deal Representatives per each DAO have casted an affirmative vote.

## Who can discuss the clauses of a deal?

In an Open Proposal, anyone with a connected wallet can discuss the clauses (Open Proposals cannot be private). On a Partnered Deal only Deal Representatives and Proposal Lead can discuss irrespective of whether the deal is public or private.

## What is the Total Amount of Tokens to Swap in a Token Swap?

For each token type that is offered as part of a Token Swap deal, the Proposal Lead can define the total amount that will be transferred to the other DAO treasury address during the swap. This amount can only be adjusted before the deal move into the Funding phase. In fact, once the Funding phase has been initiated, the deal and all its parameter are on-chain and the (non-extendable) funding period has started.

Please note that if you need to calculate the amount of tokens based on a Moving Average price within a set period, make sure that before initiating the Funding phase you specify the calculation method in the Deal Clauses, and integrate the results as the Total Amount of Tokens to Swap.

## What is the Instant Transfer Setup in a Token Swap and how is this executed?

The **Instant Transfer Setup** in a Token Swap allow you to define how much of the tokens are instantly transferred to the other DAO versus how much of your token are vested once the deal is executed on-chain. The Instant Transfer amount will be immediately sent to the other DAO's treasury address, whereas the Vested amount is the amount of tokens that will be released progressively throughout the total Vesting period defined in the Vesting setup (see FAQ below).

## What are the Vesting Setup and the Cliff Period?

The Vesting period of a Token Swap always start once the deal is executed on-chain and, if any, the amount of token defined as Vested will be linearly released throughout the Vesting period. 

If you define a Cliff period, tokens will still be linearly released but they won’t be claimable before the Cliff period ends. If you don't define a Cliff period, tokens will be linearly release and progressively available to be claimed after the Vesting period starts.

Since the vesting already starts at the execution of the deal, the Deal Representatives can claim the amount of tokens that has been compounded since the execution of the deal.

![https://ik.imagekit.io/primedao/PrimeDeals/prime-deals-vesting-graph_TsA0D1opU.png?ik-sdk-version=javascript-1.4.3&updatedAt=1651666992668](https://ik.imagekit.io/primedao/PrimeDeals/prime-deals-vesting-graph_TsA0D1opU.png?ik-sdk-version=javascript-1.4.3&updatedAt=1651666992668)

Check the example below to better understand:

- Execution of the deal: Jan 1st
- Vesting Period: 1 year
  - Vesting Period is from Jan 1st until Dec 31st
- Cliff Period: 6 months
  - Cliff Period is from Jan 1st til June 30th 

Therefore, DAO Representatives can claim starting on July 1st, after which they can already claim 50% of the vested tokens, since 50% of the time has passed.

If you define a Cliff period, tokens will not be claimable by the Deal Representatives before the Cliff period ends.

If you don't define a Cliff period, tokens will be progressively available to be claimed on a daily basis after the deal is executed on-chain.

## How does Prime Deals pricing work?

Only in case a deal is successfully approved, funded and executed on-chain, Prime DAO deducts a 0.3% fee. This fee is deducted from each DAO in the native tokens that are swapped, so for instance if D2D and DAI are swapped, then the fee will be collected in D2D and in DAI.

Note that Vesting and Instant schedules are not related to how the fee is withdrawn: the fee is automatically deducted from the amount at the execution of the token swap, so if a DAO receives 100 D2D tokens, it doesn’t matter how much % is vested and how much is instantly transferred, the fee of 0.3 D2D (0.3% of 100) will be transferred to PrimeDAO.

## What is the Funding Period in a Token Swap and what should I take in consideration when setting it up?

The Funding Period is the non-extendable number of days that both parties have to complete to fully fund and execute the swap. If the Deal Representatives and the Proposal Lead have failed to do so within this agreed upon timeframe, the deal is considered failed. The Funding Period is setup by the Proposal Lead who should set a reasonable period that takes in consideration the time needed to pass the deals through the governance processes of both parties. 

## Where do failed deals get archived?

Failed deals don’t get removed from the Prime Deals interface so that anyone can learn from past failed deals and create better ones.

<a name="privacy"></a> 

## Can I set a Deal as Private at any stage?

Yes, the Proposal Lead can set the deal private at any time from the deal dashboard. 

Changing the deal privacy setting is the only edit to a deal that will not reset already casted votes. There are various scenarios in which a DAO would want to toggle the deal from private to public, and vice versa.

For instance, some DAOs want to privately hold the negotiation process, and if an agreement is successfully reached and executed on chain they might want to share it publicly to their communities and to prompt future collaborations with other DAOs. Other DAOs might benefit by having the whole process end-to-end publicly held. Furthermore, a deal can be taken public to receive public comments and be taken back to private for further negotiation in light of the feedback.

## Why I can not see my private deal, edit my deal, or vote on my deal?

Please make sure that you are connected to the wallet address that is registered as a Deal Representative or as a Proposal Lead and sign the necessary authentication. If you’re trying to visit a deal page that is set private while you are not being connected with the proper wallet you will redirected to the homepage.