# Video DAC - Voting Token Distribution

## Introduction and Context

Video DAC is a project to create a mechanism to collect funding to be democratically allocated to projects buiding video applications using Livepeer.

The project receives funding by running a Transcoder Node in Livepeer's network, by:

- Receiving a share of Inflationary Rewards from [Livepeer's Inflation Funding mechanism](https://medium.com/livepeer-blog/inflation-funding-in-practice-in-delegated-stake-based-protocols-15cd9400e458).

   - The share of the rewards depends on the amount of Livepeer Token (LPT) that are bonded to the Transcoder Node by Delegators.
   - The Transcoder Node receives rewards in LPT every round (currently ~22 hours)
   - It first takes a cut for itself (the `Reward Cut`), and then ditributes the remainder to its Delegators.
   - Transcoders compete with each other to attract Delegators.

- Performing Transcoding work in exchange for Ether
   - When the Transcoder does work for customers of the network, it receives Fees in Ether.
   - It shares a proportion of these fees with its Delegators (the `Fee Share`)






All operations of the Transcoder node will be under the control of an Aragon DAO, including:

- Managing funds received via Transcoding activities
- Setting the parameters for the node (`reward cut`, `fee share`, `segmentPrice`)
- Managing the stake owned by the node (`bond`, `unbond`, `withdraw`)
- Granting permissions for actors and entities to perform functions for the DAO

## Types of Token

Membership
Reputation
Equity

## Distribution Proposal

### Objectives

0. Reward participants for Delegating to the DAO node
1. Incentivise continued participation

###

Uncapped supply of voting tokens. New tokens being minted all the time.

Tokens are fully transferable to other addresses / entities - Equity token

Each round that a Delegator is bonded to the node, they receive new tokens based on:

1. How much LPT they have bonded
2. The difference between this T's `Reward Cut` and the lowest T's `Reward Cut`
3. The difference between this T's `Fee Share` and the highest T's `Fee Share`
4. How long they've been bonded for
5. Whether they've been using their existing tokens to participate in voting?

If a Delegator unbonds some or all of their LPT from the node, they don't lose any of their voting tokens, instead they just don't gain any more, hence they become diluted out by other voters.

Delegators receive their tokens through a claiming process. This claiming process allows them to either a) claim for only themselves, or b) claim for themselves + specific individuals, or c) claim for themselves + everyone. For b) and c) they would receive a portion of the voting tokens that should be going to someone else - with the portion dependent on factors such as i) how long since someone else claimed, ii) how long since someone claimed for everyone, iii) how many voting tokens are unclaimed as a proportion of the total claimed...
