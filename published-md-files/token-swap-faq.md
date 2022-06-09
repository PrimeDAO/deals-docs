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

Here is an high-level summary of the most relevant steps in a Token Swap. For an in-depth walkthrough and for a more clear differentiation between Open Proposals and Partnered Deals, please refer to the relevant step-by-step tutorials <a href="/documentation/INITIATEADEAL">here</a>.

1. Decide if you want to start an Open Proposal or a Partnered Deal.
2. Provide a brief description of your proposal.
3. Specify the address of the Proposal Lead and (optionally) contact e-mail. This address will be allowed to edit the deal during the negotiation integrating new points from the conversation.
4. Decide whether you want to keep private or publicly accessible the details of a deal, please see <a href="/documentation/TokenSwapFAQ/#can-i-set-a-deal-as-private-at-any-stage">here</a> for a detailed description of how privacy settings work. In the case of a Partnered Deal, this will make public or private the whole deal. In the case of an Open Proposal, this setting will make public or private only the incoming offers.
5. Fill-out the DAO details: the DAO treasury address that will receive the token after the swap, and a list of the address of the DAO representatives who will be able to cast a vote on the deal, either to accept or reject it, fund the deal, as well as claim tokens that will be sent to the treasury address, or withdraw funds they deposited on behalf of their DAO in case the deal is not successful. In case of a Partnered deal, fill-out the same general details for the other DAO.  If you don’t already have a partner DAO choose to start an Open Proposal in step 1., in this way you will be able to find many potential prospects: they will have to provide their own terms and select their own Deal Representatives.
<a aria-current="page" class="Link__SLink-sc-2d0ctv-0 kICpDJ" href="/"><svg class="Header__SLogo-sc-14sqt5o-9 cJdvUX" id="Layer_1" data-name="Layer 1" viewBox="0 0 1360 280"><title>horizontal_left_small_black</title><path d="M137,9.84A128.75,128.75,0,1,0,265.7,138.59,128.76,128.76,0,0,0,137,9.84Zm94.23,135.78H171.44a36.38,36.38,0,1,1,.28-12.66h59.46a6.33,6.33,0,0,1,0,12.66Z"></path><path d="M 1302.59 139.464 C 1312.27 139.464 1318.86 145.644 1320.92 155.524 L 1283.21 155.524 C 1285.27 145.434 1292.69 139.464 1302.59 139.464 M 1352.23 165.004 C 1352.23 135.134 1331.43 113.904 1302.99 113.904 C 1272.51 113.904 1251.08 135.544 1251.08 166.034 C 1251.08 197.354 1273.32 218.364 1303.82 218.364 C 1326.69 218.364 1340.69 210.744 1349.14 200.234 L 1330.6 181.234 C 1324.678 188.048 1316.136 192.019 1307.11 192.154 C 1294.75 192.154 1285.11 186.154 1283.01 174.654 L 1351.61 174.654 C 1351.82 172.584 1352.23 167.844 1352.23 164.964 M 1197.1 216.514 L 1229.45 216.514 L 1229.45 141.734 L 1248.61 141.734 L 1248.61 115.734 L 1229.45 115.734 L 1229.45 101.144 C 1229.45 93.144 1233.15 90.224 1238.92 90.224 C 1241.81 90.224 1247.17 91.664 1251.49 93.934 L 1257.49 70.644 C 1253.99 68.174 1243.69 62.824 1230.3 62.824 C 1210.11 62.824 1197.13 74.974 1197.13 99.904 L 1197.13 115.764 L 1187.45 115.764 L 1187.45 141.764 L 1197.13 141.764 Z M 1124 189.934 C 1111.23 189.934 1102.37 180.464 1102.37 166.244 C 1102.37 151.824 1111.64 142.344 1124 142.344 C 1136 142.344 1145.22 152.434 1145.22 166.244 C 1145.22 180.664 1135.54 189.934 1124 189.934 M 1117.21 218.364 C 1129.36 218.364 1138.42 214.244 1145.02 205.804 L 1145.43 206.004 L 1145.43 216.514 L 1176.13 216.514 L 1176.13 115.764 L 1143.78 115.764 L 1143.78 126.274 L 1143.37 126.484 C 1136.422 118.372 1126.23 113.763 1115.55 113.904 C 1089.55 113.904 1069.61 135.334 1069.61 166.244 C 1069.61 197.354 1089.61 218.364 1117.21 218.364 M 1008.21 218.364 C 1032.53 218.364 1061.98 206.004 1061.98 171.594 C 1061.98 143.374 1042.21 136.774 1016.45 126.894 C 1000.59 120.714 995.24 117.004 995.45 109.994 C 995.45 102.994 1000.6 98.674 1009.05 98.674 C 1017.29 98.674 1026.35 102.584 1038.92 112.464 L 1058.29 87.334 C 1044.29 75.334 1026.77 67.964 1007.61 68.334 C 980.41 68.744 959.61 87.074 959.61 111.384 C 959.61 140.234 981.87 150.744 1004.11 158.384 C 1020.6 163.944 1025.74 167.444 1025.74 175.484 C 1025.74 182.074 1020.8 187.844 1009.26 187.844 C 999.17 187.844 985.78 182.694 974.66 170.534 L 954.46 195.054 C 970.12 211.124 989.46 218.334 1008.23 218.334 M 864.64 218.334 C 892.25 218.334 905.64 204.734 905.64 185.984 C 905.64 166.214 893.49 160.444 871.23 152.824 C 861.14 149.324 857.43 147.054 857.43 143.954 C 857.43 140.044 861.75 138.404 865.43 138.404 C 872.23 138.404 880.88 141.904 887.89 148.904 L 903.14 126.454 C 891.39 117.804 880.27 113.874 865.02 113.874 C 844.02 113.874 827.32 125.624 827.32 146.024 C 827.32 165.384 842.15 173.624 859.05 178.774 C 871.62 182.694 874.71 184.774 874.71 188.054 C 874.71 191.754 871.41 194.054 865.02 194.054 C 855.75 194.054 847.1 190.344 838.65 182.724 L 823.6 203.584 C 834.72 213.474 848.73 218.414 864.6 218.414 M 780.14 216.564 L 812.28 216.564 L 812.28 115.764 L 780.13 115.764 Z M 796.2 103.254 C 807.33 103.254 815.57 95.254 815.57 84.704 C 815.57 74.614 807.33 66.574 796.2 66.574 C 785.07 66.574 777 74.774 777 84.654 C 777 95.164 785 103.204 796.16 103.204 M 725.74 218.364 C 753.35 218.364 766.74 204.764 766.74 186.014 C 766.74 166.244 754.58 160.474 732.34 152.854 C 722.24 149.354 718.53 147.084 718.53 143.984 C 718.53 140.074 722.86 138.434 726.53 138.434 C 733.32 138.434 741.98 141.934 748.98 148.934 L 764.22 126.484 C 752.48 117.834 741.36 113.904 726.11 113.904 C 705.11 113.904 688.41 125.654 688.41 146.054 C 688.41 165.414 703.24 173.654 720.13 178.804 C 732.71 182.724 735.79 184.804 735.79 188.084 C 735.79 191.784 732.5 194.084 726.11 194.084 C 716.84 194.084 708.19 190.374 699.74 182.754 L 684.74 203.564 C 695.86 213.454 709.88 218.394 725.74 218.394 M 625 189.934 C 612.22 189.934 603 179.634 603 166.244 C 603 152.434 612.07 142.544 625 142.544 C 637.56 142.544 646.84 152.234 646.84 166.244 C 646.84 180.044 637.16 189.934 625 189.934 M 625 218.364 C 656.73 218.364 679.39 197.144 679.39 166.244 C 679.39 135.134 656.73 113.904 625 113.904 C 592.45 113.904 570.4 135.544 570.4 166.244 C 570.4 196.734 592.45 218.364 625 218.364 M 459.57 216.514 L 491.7 216.514 L 491.7 165.834 C 491.7 150.174 499.12 142.544 510.25 142.544 C 520.75 142.544 526.32 147.284 526.32 163.974 L 526.32 216.514 L 558.46 216.514 L 558.46 156.144 C 558.46 124.214 543.21 113.904 522.4 113.904 C 510.785 113.711 499.686 118.7 492.12 127.514 L 491.7 127.514 L 491.7 115.764 L 459.57 115.764 Z M 384.16 218.154 C 406.83 218.154 429.07 210.534 442.46 200.234 L 442.46 134.514 L 381.07 134.514 L 381.07 162.944 L 409.5 162.944 L 409.5 180.254 C 401.753 184.553 393.019 186.756 384.16 186.644 C 359.23 186.644 344.61 167.274 344.61 143.574 C 344.61 116.384 361.92 100.514 382.72 100.514 C 395.843 100.473 408.44 105.666 417.72 114.944 L 442.02 94.344 C 427.02 77.034 403.91 68.174 382.69 68.174 C 335.93 68.174 308.52 101.174 308.52 143.574 C 308.52 191.174 341.9 218.154 384.13 218.154"></path></svg></a> 
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">Please note that even if Deal Representatives are normally the ones that are exclusively allowed to fund a deal and claim tokens on behalf of the DAO, this is not true if the DAO is using a multi-sig wallet from the Gnosis Safe App to execute these steps. You can refer here (TODO add link) on how funding and claiming works in case a DAO wants to use the Gnosis Safe App.</div>
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

You don't need to be part of DAO to be a Proposal Lead (see <a href="/documentation/GeneralFAQ/#what-is-a-daoplomat">here</a>).

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

## Can I set a Deal as Private at any stage?

Yes, the Proposal Lead can set the deal private at any time from the deal dashboard.

Changing the deal privacy setting is the only edit to a deal that will not reset already casted votes. There are various scenarios in which a DAO would want to toggle the deal from private to public, and vice versa.

For instance, some DAOs want to privately hold the negotiation process, and if an agreement is successfully reached and executed on chain they might want to share it publicly to their communities and to prompt future collaborations with other DAOs. Other DAOs might benefit by having the whole process end-to-end publicly held. Furthermore, a deal can be taken public to receive public comments and be taken back to private for further negotiation in light of the feedback.

## Why I can not see my private deal, edit my deal, or vote on my deal?

Please make sure that you are connected to the wallet address that is registered as a Deal Representative or as a Proposal Lead and sign the necessary authentication. If you’re trying to visit a deal page that is set private while you are not being connected with the proper wallet you will redirected to the homepage.