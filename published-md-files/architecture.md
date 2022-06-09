# Smart Contracts Architecture

## What is the smart contract architecture behind Prime Deals?

The Prime Deals smart contract architecture has been designed with non-custodianship, trustlessness, extensibility and security in mind. Future modules can be added to Deals as they are being built, without having to make structural changes in the underlying architecture. Our first module is the `TokenSwapModule`. To keep the description of the architecture general, the wording `DealModule`  instead of `TokenSwapModule` is used below.

The Prime Deals architecture consists of three main components. These are:

- `DealManager`
- `DaoDepositManager`
- `DealModule`

### Deal Manager

The `DealManager` contract serves as a central registry, managing and storing the addresses of all the contracts involved in Prime Deals. It activates and deactivates new Deals modules and creates `DaoDepositManager`contracts. The `DealManager` is also used in a multitude of authentication processes to make sure that all the contracts involved in Prime Deals are verified contracts part of the Deals Modules. The `DealManager` is governed and managed by PrimeDAO which can add new modules, change fees or intervene in the whole contract to manage extreme events and disasters. **However, this does not grant PrimeDAO with the power to touch any funds or modify deals, as the protocol remains trustless.**

### DaoDepositManager

The `DaoDepositManager` contract serves a similar function to an escrow contract. It can be funded to hold the amount the DAO is contributing to a Deal before it has been executed. After execution, it will hold the agreed-upon vested amount (if applicable) from which the funds can be claimed during and after the vesting period. 

The workings of the vesting mechanism is such that the vesting duration is started automatically right after the deal execution. It locks the tokens for the intended vesting duration in the DAOs `DaoDepositManager`. The function to claim vested tokens can be called through our frontend by all the Deal Representative(s) without restriction. When calling the claim function in the contract, it will transfer the claimable tokens to the DAOs treasury address, which is stored in the `DaoDepositManager` state at creation time. In this way, no tokens can be sent to other addresses than the DAO treasury.

A few other things to highlight are:

- The `DaoDepositManager` is used for all the deals a DAO makes within the Prime Deals ecosystem. This means that a `DaoDepositManager` is specific for a DAO, not a deal. When a DAO participates in Prime Deals for the first time, a `DaoDepositManager` is created which will hold all the future deposits and vestings for that given DAO, across all deals made.
- All the vested DAOs funds are in their own `DaoDepositManager` before and get transferred to the other Dao’s `DaoDepositManager` after the execution
- All the tokens claimable from vested tokens can only be transferred to the DAOs address as set in the `DaoDepositManager` contract

### DealModule

The `DealModule` contract serves as the first point of contact in creating a deal. It stores all the parameters of the deal on-chain. 

When the deal is executed, the `DealModule` will verify if all the conditions for the deal are met, i.e. that all deposits have been made. Next, the module will proceed to pull all the tokens involved in the token swap from each DAOs `DaoDepositContract` into the module. By doing this, all the tokens involved are pooled into the module. The following step in the execution process is to transfer all the unvested tokens to the DAO addresses, after which it sends the to-be-vested token amount into the respective DAOs `DaoDepositContract` to start the vesting period.

## Security

Security was one of our main concerns during the building of Prime Deals.
All of the Prime Deals contracts have therefore undergone an extensive audit by our auditing partner **byterocket GmbH**, involving manual as well as automated reviews, state-of-the-art testing methods like fuzz- testing as well as game theoretic reviews of the protocol itself.

The learn more about the audit, please see <a href="https://byterocket.com/audit/primedeals-token-swaps" target="_blank" rel="noopener noreferrer">here</a>.

## What are the states a Token Swap deal can take on?

A deal can exist in the following states (also known as *phases*):

`Active`
`Cancelled`
`Negotiating`
`Funding` (in Progress)

(Token Swap) `Completed`

(Token Swap) `Failed`

`Active`

- An Open Proposal is running
- Deal is open to receive an offer from a prospective Partner DAO
- Anyone can connect with their wallet and discuss the clauses except when it’s set private

`Cancelled`

- Discussing, Editing and Voting the deal is no longer possible

It can happen when

- An Open Proposal has been withdrawn by the Proposal Lead

OR when 

- The Proposal Lead has deliberately chosen to reject a Partnered deal. This can happen at any time as long as the deal has not been approved (by greater than 50 % of the vote).

`Negotiating`

- Two DAOs (Primary DAO and Partner DAO) are involved
- Deal clauses can be discussed by the Proposal Lead and the Deal representative(s)s
- Deal can be modified by the Proposal Lead
- Edits to the deal automatically resets all votes that have been already casted. The only edit that won’t reset all votes is the change of a deal from private to public.
- Voting the deal is possible by the Deal Representative(s)
- In this phase, voting is in progress (voting rules can be found <a href="/documentation/VoteonaDeal">here</a>). When the majority of the Deal Representative(s) for each DAO have favorably voted for the deals, the deal can go in the Funding phase initiated manually in the UI by the Proposal Lead

`Funding` (in Progress)

- Can happen only after the majority of the Deal Representative(s) for each DAO have voted favorably for the deal
- Can happen only before the end of the specified Funding Period
- It is initiated only by the Proposal Lead in the UI
- Depositing and withdrawing of tokens to be swapped can begin
- Voting and editing the deal is no longer possible
- The Deal Representative(s) can deposit from the UI (Note that anyone can technically deposit tokens directly to the contract if they know the address)
- If the Funding Period is not expired and the all the funds have been successfully collected, the deal become executable by either the Proposal Lead or any of the Deal Representative(s) in the UI

(Token Swap) `Failed`

- The deal never became executable or executed.
- Discussions are no longer possible
- Deal Representative(s) can withdraw their funds if they already allocated some in the escrow

It happens when:

- Voting is completed, the Proposal Lead started the Funding phase, but the Deal Representative(s) failed to fund the deal in the Funding Period specified by the deal

OR

- Voting is completed and the deal is rejected by the majority of the Deal Representative(s) for each DAO.

OR

- Voting is completed, Proposal Lead initiated Funding phase, Deal Representative(s) fully funded the deal but the Proposal Lead failed to execute the deal within the given time.

(Token Swap) `Completed`

- The deal has been manually executed
- Discussions are no longer possible
- The Vesting Period and the ability to claim tokens begins at execution, following the defined vesting rules
- The Funding Period ends automatically when the Deal is executed

## What are the error states that the smart contracts can produce?

This is an updated list of error messages that can be printed on screen while trying to execute on-chain operations. You can refer to this list to understand better what is going on in case of issues, and to communicate with us when you incur in one:

## PrimeDAO General init related

- `001` : Contract already exists, already initialized

## PrimeDAO General input

- `100` :  Invalid input address 
- `101` :  Input value cannot be empty 
- `102` :  Input arrays length mismatch 
- `103` :  Amounts mismatch 

## Prime Deals specific

### Input (200 - 219)

- `200` :  Invalid deposit ID 
- `201` :  Vesting cliff cannot be bigger than the vesting duration 
- `202` :  msg.value does not match the input value 
- `203` :  Invalid metadata, it already exists 
- `204` :  Invalid amount of DAOs, at least 2 are required 
- `205` :  Invalid amount of tokens, at least 1 is required 
- `206` :  Invalid metadata 
- `207` :  Invalid deal ID 

### Permissions (220 - 239)

- `220` :  Can only be called by a Deals module contract 
- `221` :  Can only be called by the DealManager contract 
- `222` :  Withdraw not authorized msg.sender is not the depositor or the deal has not been expired 

### Tokens (240 - 259)

- `240` :  No withdrawable amount available 
- `241` :  ERC20 token transfer failed 
- `242` :  ETH transfer failed 
- `243` :  ERC20 token approve failed 
- `244` :  Claimable amounts mismatch 
- `245` :  Invalid balance 

### General (260 - )

- `260` :  Invalid DealManager address set in the contract 
- `261` :  DaoDepositManager implementation is not set 
- `262` :  Not enough tokens or ETH are sent to the module 
- `263`  :  Function call only available for ERC20 tokens
- `264`  :  Fee cannot be more then 20%
- `265` :  Swap is not executable
- `266` :  Deal status is not ACTIVE 