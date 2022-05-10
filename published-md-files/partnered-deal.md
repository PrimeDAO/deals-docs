# Create a Partnered Deal

The wizard will guide you through the process of creating a Partnered Deal. 

Please note that you can always come back to edit your input before you click the <kbd>SUBMIT</kbd> button on the last step of the wizard.

<video style="max-width: 100% !important; height: auto !important;" controls preload="auto"><source src="https://ik.imagekit.io/primedao/PrimeDeals/3-create-a-partnered-deal-deals-comp_oPDFXVnFu.mp4" type="video/mp4">Your browser does not support the video tag.</video>

~~TEST STICKY HEADER SCROLL SETUP~~
You can follow the example of a Partnered Deal linked [here](https://prime-deals-staging.vercel.app/documentation/CreateaPartneredDeal#example-of-a-partnered-deal-input) as a template for your deal. 
~~TEST STICKY HEADER SCROLL SETUP~~
## Token Swap Proposal

1. Provide a clear **Proposal Title** that capture the essence of the deal you want to offer (max 60 ch.).
2. Provide a brief outline of the Token Swap deal in the **Proposal Summary** box (max 350 ch.).
3. In the **Proposal Description** provide the details, background and features of your Token Swap proposal. Explain why it's particularly valuable or unique.

## Lead Details

1. Provide the Ethereum address for the Proposal Lead who will gain administrative rights of the deal. If you are already connected to the app with the wallet of the intended Proposal Lead, just click <kbd>MAKE ME THE PROPOSAL LEAD</kbd>. 
    - To learn more about the role and rights of a Proposal Lead please see [here](https://deals.prime.xyz/documentation/documentation/TokenSwapFAQ#proposal-lead).
3. Provide the **Contact E-mail (optional)**
4. Decide whether you wanna keep this deal and the conversations private, or if you rather keep these publicly accessible.
    * Toggle this option on if you DON’T want the public to see what is being discussed by the DAOs. This will make all conversations of this Partnered Deal only visible by the Proposal Lead and the involved Deal Representatives.
    * You can always turn the deal to public during the Negotiation phase or after the deal is ratified. Note that conversations previously held in private will remain private, even if the deal is turned public. Contrary to an Open Proposal, in a Partnered Deal only Proposal Lead and Deal Representatives can discuss the clauses, regardless if the deal is public or private.
    * A negotiated deal that has been turned public can be turned back into private, and vice versa.

## Primary DAO Details

Fill in the details of the Primary DAO. This is the DAO for which the original proposal is initiated for.

1. Provide the **Primary DAO Name**
2. Provide the **Primary DAO Treasury Address**, which is the address that will receive the tokens from the other DAO after the swap
3. Provide the **Primary DAO Avatar**: a public URL to a small JPG, GIF, PNG or BMP formats image with square aspect ratio with a recommended size of 400x400px and maximum 5MB file size.
4. Provide the addresses of the **Primary DAO Representatives**.  To learn more on the role of the DAO Representatives please see [here](https://prime.deals.xyz/documentation/TokenSwapFAQ#representatives).

### Partner DAO Details

Fill in the same details as above, this time for the Partner DAO

### Token details

In this section you have to fill in the details of the token(s) that both DAOs want to swap. Each DAO can offer up to 2 token types. 

First add the Token details for the Primary DAO, then, move on the Partner DAO step and fill the Token details too. 

Click on <kbd>ADD TOKEN +</kbd>, this will open up a box in which you’ll be able to input the Token details.

For each type of token that a DAO want to swap you’d need to provide these details:

1. The native address of the token to swap.
2. The **Total Amount of Tokens to Swap** which defines the total amount of tokens that will be transferred to the other DAO during the swap. You can adjust this amount at any time before the beginning of the Funding phase of the deal.
3. The **Instant Transfer Setup and the Vesting setup**
    - Toggle the vesting schedule to define how much of the tokens are instantly transferred to the other DAO versus how much of your token are vested once the deal is executed on-chain. The Instant Transfer amount will be immediately sent to the other DAO's treasury address, whereas the Vested amount is the amount of tokens that will be released progressively throughout the total Vesting period defined in the Vesting setup in the next step below.
    - If you have defined a Vested amount, once the deal is executed on-chain, that amount will start to be released linearly throughout the Vesting period. If you define a Cliff period, tokens will not be claimable before the Cliff period ends. If you don't define a Cliff period, tokens will be progressively available to be claimed on a daily basis after the Vesting period starts.
4. The **Funding Period**
    - In this step you can setup the non-extendable number of days that both parties have to complete to fully fund and execute the swap. If the Deal Representatives and the Proposal Lead have failed to do that within this agreed upon timeframe, the deal is considered failed. Make sure that you set a reasonable Funding Period that takes in consideration the time needed to pass the deals through the governance processes of both parties.

## Terms

In this section you have to provide all the important clauses of your proposal (max. 10). Please be specific and clear so that everyone can understand the terms of the agreement between the parties involved. This document can serve as a single source of truth for future reference.

1. Click the button <kbd>ADD CLAUSE +</kbd>
2. Write the text of your clause (max 500 ch.)
3. Click <kbd>SAVE</kbd> to save this clause and move to the next.
4. You can edit a clause with the <kbd>EDIT</kbd> button.
5. Make sure have written and saved all clauses

Click <kbd>PROCEED</kbd> at the bottom of the page to move onto the next section

## Submit

In this section you can visualize a summary of all the information you have input. Please, inspect all parts of the summary byword and make sure they precisely reflect what you want to propose. If you spot an error, you can navigate to previous sections of this wizard to correct them before submitting your proposal. It's your responsibility to verify that all the relevant information is correct (e.g. Treasury address, Deal Representative addresses, Token addresses, Token amount, etc.). PrimeDAO don't offer any validation process to verify your input. For instance, it cannot verifies whether a treasury address is related to a certain DAO. 

When you are ready click <kbd>SUBMIT</kbd>. Please be patient as it might require a moment to register your deal. Once successfully registered you will see a box with a confirmation message. You can now visit the deal page and share the link to have other people join.

# Example of a Partnered Deal input

## Proposal Title

**Example**

<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">Partnership Agreement ADAO <> BDAO</div>

**Example**

<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">Token Swap Agreement ADAO <> BDAO</div>

## Proposal Summary

State the general reasons for what this token swap aims to achieve. Is it to align interests, to collaborate on a strategy, to build together, to participate in a program?
    
**Example**
    
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">The partnership aims to set the foundation for a long-term collaboration between DAO1 and DAO2. The two organizations aim to integrate on a technical and operational level to bring a top-class flexible ProjectA to xChain.</div>

State the value and amount of the tokens to be swapped by each party.
    
**Example**
    
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">DAO1 seeks to partner with DAO2 asking for a swap of $250k in governance tokens from each DAO.</div>

## Proposal Description

Give a background of the communication and relationship between two DAOs. 

- Is there any history context to this partnership? What are the relevant milestones you can provide?
- How long have you been in touch with?
- What is the collaborative background between these DAOs?
- How did the teams meet and how did they find alignment?

Give an overview of the partnership and scope of collaboration. 

- What does this partnership proposal aim to outline?
- What is the value that both groups see in seeding a stronger collaboration through token swap?
- Provide external link if there is a doc version of this proposal.
- Provide external links if there are forum posts related to this proposal.
    
**Example**

<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">Background on the Partnership: The relationship between DAO1 and DAO2 goes back to <Date>. Since the launch of DAO1 in <Date>, the DAO2 has played a crucial role in the DAO1 ecosystem.</div>
    
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">In <Date>, DAO1 set out to revamp its ProductOP experience for users and project teams. Through a grant from DAO2 (link to the grant post), the development of what is known as ProductOP started. ProductOP allows anyone to do this and that. The product provides these advantages to the users, these advantages to the ecosystem, and theese benefits to DAO2.</div>
 
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">With the development of ProductOP, DAO1 became DAO2’s partner, and the collaboration extended to active technical and organizational development. In <Date>, DAO2 and DAO1 made headlines by doing this (add link for reference), which was important for reasons x,y, and z.</div> 
    
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">Since then, the teams have continued to work together, and various DAO1 contributors have supported the development of DAO2 and the DAO2 Protocol.</div> 

<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">After successfully going through the maturity stages of re-branding and raising seed funds, DAO1 has grown to over 30 full-time contributors and is ready to launch its product suite and solidify relationships with DAO2 with a token swap.</div>

## Clauses

Start the clause with a title, and then expand on it. This is a set of suggested dimensions to think about.

### D2D Collaboration

What are the exact collaboration areas and commitments from each DAO?
    
**Example**
    
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">DAO1 will support the development of the DAO2 and, where possible, share learnings and resources with DAO2.</div>

<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">DAO2 will get early access to [](https://www.prime.xyz/deals)DAO1’s upcoming ProductOP, which is described in this definition and has these benefits, to give input, to ensure the product serves the needs of DAO2.</div>

<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">Liquidity Pool Creation: DAO1 aims to create deep liquidity between DAO1 tokens <> DAO2 tokens for these reasons. Here is the grander strategy for this action.</div>

<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">Market buy: DAO1 will commit to market-buying at least 1000 DAO2 tokens within 60 days after the passing of the proposal. DAO1 is allowed to access DAO2 token liquidity on any of the available chains, namely: Ethereum Mainnet, Gnosis Chain, and Celo to acquire the DAO2 tokens.</div>

Does the partnership have an end date?
    
**Example**
    
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">Partnership Term: ****The Partnership is open-ended and does not have an expiry date.</div>

What are the rules for terminating this partnership? Is there an exit clause?
    
**Example**
    
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">Exit Clause: ****Both organizations can at any moment terminate the agreement through their respective governance systems.</div> 

### Technical

What are the technical aspects of this collaboration? Is there a specific development or implementation planned? Is there a product integration?
    
**Example**
    
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">DAO1 will continue to host this protocol and support the development of it on DAO2’s protocol.</div> 
    
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">Friendly fork relation: DAO1 will support the development of the DAO2 on alternative blockchains, currently evaluating these strategies with these potential partners, with the potential for it to develop into a Balancer Friendly Fork.</div>

<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">DAO1’s protocol will support DAO2 with these implementations.</div>

<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">BD Synchronization: Here is how both DAOs will partner to increase these metrics for each other’s protocols.</div>

### Terms of the Token Swap

How are the token swap amounts calculated? Provide the dollar value of the tokens to be swapped from each side, and how it is calculated. If it is Moving Average based on a time period, provide the time period for calculating the MA, and from what date it will be calculated.
    
**Example**
    
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">**Token Swap:** $50.000 worth of $DAO2 tokens will be swapped for $50,000 of $DAO1 tokens taken the 30-day average at the end of the vote on both sides.</div>

<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">**Mutual Grant:** Grant DAO2 $250K USD worth of DAO1’s $DAO1 governance token, and grant DAO1 $250,000 USD worth of $DAO2 governance tokens, calculated through the 30-day average at the end of the vote on both side.</div>

<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">**Token Swap where a DAO’s token value is calculated differently for the deal than the market price:** Conduct a token swap of $250k in $DAO2 tokens from a 30 day TWAP from the date of execution of this proposal - in return for 500k $DAO1 tokens being 0.5% supply at a $50 million fully diluted valuation of DAO1.</div>

### Usage of the Swapped Tokens**

Is there an agreement for how to utilize the swapped tokens?
    
**Example**
    
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">There are no lock-ups or limitations to which the DAOs need to adhere to in regards to the received tokens, however it is expected that both DAOs will communicate any changes to the usage of the tokens to the other party.</div>
    
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">Staking: Each protocol may stake the swapped tokens in order to participate in the other's governance.</div>

### Co-liquidity provision**

**Example**
    
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">To align governance interests, between the two organizations, the creation of a co-liquidity pool is proposed with the following details; 25,000 $DAO2 tokens would be transferred to DAO1 at the end of this date or deliverable  to bootstrap a DAO1 / DAO2 pool with 50/50 weights and 2,5% trading fees.</div>

<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">Right after the conclusion of the DAO1 LBP, DAO1 will seed a pool with the 25,000 $DAO2 tokens and match it with the same $ value in $DAO1 tokens. Once the pool is initiated, DAO1 will transfer 50% of the Liquidity Pool Tokens to DAO2 to complete the transaction.</div>

<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">The pool will again be called the DAO2 <> DAO1 pool and function as a liquidity bridge between the two DAOs. The DAO2xDAO1 pool will be one of the two main liquidity pools for DAO1.</div>

<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">Co-liquidity Provision: ****To enhance alignment, DAO2 will match the received $DAO1 tokens with an equal value in (x) tokens from its treasury and add it to the %50 DAO1/ %50 DAO2 tokens in Balancer. DAO1 will match the received $DAO2 with an amount of (y) - equal to 25% of the amount received - and add it to the %80 DAO2/ %20 (y) pool in Balancer.</div>

Is there any rules for selling other DAO’s swapped tokens?
    
**Example**
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">To ensure long-term alignment, DAO1 will hold no less than 50% of the tokens received through 2023 and act as a meta-delegate in the DAO2 ecosystem. And DAO2 will hold no less than 50% of the tokens received through 2023 and act as a meta-delegate in the DAO1 ecosystem.</div> 

<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">Each protocol undertakes to not reduce its holding or exposure to the swapped tokens for at least a period until 1 January 2023.</div>

### Operational

How will the partnership move forward and kept track of?
    
**Example**
    
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">Both DAOs will actively share DAO operational learnings and workflows, starting with a bi-monthly knowledge-sharing session covering three topics relevant to both DAOs. The first session will be organized in mid-January.</div>
  
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">To ensure operational effectiveness, a monthly call will be set up by at least one Deal Representative of each organization.</div>

### Governance

Does this partnership create a customized governance access to the other DAO? If so, how will this be done?
    
**Example**
    
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">The DAO1xDAO2 liquidity pool token will be added to the Snapshot strategies of both DAOs to allow DAO1xDAO2 token holders to participate in the Governance of both protocols.</div>

<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">A new snapshot will be set-up with the DAO1xDAO2 as the governing token. This snapshot will be used to govern issues related to this DAO agreement.</div>

How will this partnership be overseen? Who are the individuals responsible for running this partnership?
    
**Example**
    
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">Partnership Governance: The partnership is managed by Deal Representatives of the organizations. The respective governance processes of both DAOs can overwrite any decision by Deal Representatives. In the case of this partnership, there are 2 representatives for each organization.</div>

What happens when DAOs want to rule over a clause agreed upon on the deal, or use the tokens in a different way than what is specified in the deal?
    
**Example**
    
<div class="sample"; style="border: 1px solid #EBA7DA; border-radius: 5px; padding: 5px;font-family: monospace; margin: 18px;">There are no lock-ups or limitations to which the DAOs need to adhere to in regards to the received tokens, however it is expected that both DAOs will communicate any changes to the usage of the tokens to the other party.</div> 