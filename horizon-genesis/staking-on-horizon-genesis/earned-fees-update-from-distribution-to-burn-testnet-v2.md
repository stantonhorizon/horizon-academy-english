# Earned Fees Update - From Distribution to Burn (Testnet V2)

Horizon Protocol shares with stakers all the revenue generated through trade fees in the Horizon Protocol Exchange. Currently, the revenue is shared as an "Earned Fee" in the form of zUSD every week. Every staker gets a percentage of the total revenue earned during a week. The "Earned Fee" gets claimed along with the weekly HZN rewards. The percentage is determined by the percentage of debt they have in the global debt market.

The Earned Fees Update changes from distributing the "Earned Fee" as rewards to instead, burning it, which has the same result of lowering the amount of debt owed to all stakers while opening up the possibility for stakers to receive the rewards passively and for fair "Earned Fee" sharing across multiple chains.

\


## How will the Earned Fees Update work?

The Earned Fees Update only does one thing. Instead of distributing zUSD to every wallet every week, it now passively burns the amount of zUSD that you would receive from the global debt pool.

The reason that distributing and burning will create the same results for stakers is due to the global debt pool. In both situations, the percentage of the debt pool the staker owns remains the same. The difference is that instead of distributing all the "Earned Fees" to each staker, the "Earned Fee" gets burned and lowers everyone's debt ratio. The zUSD from the burned "Earned Fee" can be re-introduced into the global debt pool by minting again. The elegance of this solution is that the burning mechanism doesn't require active weekly claims from stakers. This means that even passive stakers who missed the weekly HZN reward will always receive their weekly 'Earned Fee' rewards.

In addition, burning now means that a single smart contract can be called, which burns the total "Earned Fees" from the global debt pool instead of individual contracts from each staker claiming. This also opens up the possibility to cross-chain protocol, since it will become feasible to track the amount of "Earned Fees" burnt across all chains.

\


## Earned Fees Update Benefits

There are two main benefits to this update:

\- All stakers will be able to receive their percentage of the Earned Fees from the Horizon Exchange regardless of whether they are actively claiming every week. Previously, if you did not claim, the missed claims will go back into the pool for next week. With the Earned Fees Update moving from distributing to burning zUSD from the global debt, this means all passive stakers will gain the benefits as well.

\- Makes potential cross-chain rewards fair for all stakers on Horizon Protocol: All stakers will collect their rewards each week, regardless of which chain their staking might be on. This is made possible with the [Debt Share Token](https://academy.horizonprotocol.com/horizon-genesis/staking-on-horizon-genesis/debt-share-testnet-v2) update.

\
