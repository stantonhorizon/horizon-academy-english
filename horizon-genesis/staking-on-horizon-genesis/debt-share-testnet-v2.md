# Debt share (Testnet V2)

In Horizon Protocol, to manage how much debt each staker holds as the debt changes due to the fluctuation of each zAsset, a debt registry is kept for each staker. The registry keeps track of every Mint and Burn action by every staker and rolls it up into a single calculation to determine the debt percentage of each staker.

This works for now, but there are limitations to this design as it will not work if Horizon Protocol ever decides to expand beyond one chain, since the debt registry is only recording the actions from one chain and not compatible with a multi-chain debt pool.

Learning from Compound, Aave, and Synthetix, we will be upgrading the debt registry into debt shares, which will simplify the logic and code for tracking debt and also make the protocol capable of tracking debt across multiple chains.



## How Debt Shares Work

Debt shares can be treated similar to the shares of a stock. When minting new zUSD on Horizon Protocol, the protocol is issuing debt. To represent the debt, debt shares are issued at the same time based on the amount of zUSD minted.

The debt shares represent the debt pool in terms of a percentage without worrying about how the global debt pool fluctuates. If you hold 50% of all the debt shares and the global debt pool is $100 zUSD, then your debt shares will show that you owe $50 zUSD. If the global debt pool grows to $200 zUSD, then your debt share of 50% will now represent $100 zUSD. Alternatively, if the global debt pool shrinks from $100 zUSD to $50 zUSD, then your debt share of 50% will now represent $25 zUSD.\


## Debt shares can be simplified into 3 equations:

* How much debt shares are issued or burned when minting or burning by a staker:

`debt_shares = total_shares * zUSD_amount/total_debt_pool`

* Calculate the debt percentage of a staker how much zUSD they owe:

`debt_percentage = balance(user)/total_supply(debtshares)`

* &#x20;The calculate how much zUSD debt a staker holds:

`staker_zUSD_debt = debt_share_percentage * global_debt_pool`\


## Debt Shares and their Benefits

The reason that debt shares are necessary is that there needs to be a way to track your debt without consideration for how your zAssets and the global debt pool fluctuate. Debt shares can accomplish this because it only takes into consideration staking actions.



## Benefits of using debt shares include:

* Provides a way to track staker’s debt using a token.
* Simplifies the system to exactly how many debt shares each staker holds instead of a debt ledger that - needs to be constantly updated with each Mint and Burn from all users.
* Enables staking rewards to be distributed fairly as the debt shares are much easier to keep up to date.
* No more need for snapshotting the debt registry to determine how to distribute the rewards as debt shares will always be available.
* Enables migration of stakers debt across chains in one transaction.



\
