---
description: By staking HZN to mint zUSD, but not claiming the weekly reward
---

# HIP-7: Utilize the Community Fund for Additional Liquidity

**Type:** Horizon Improvement Proposal \
**Date:** Jun 21st, 2023\
**Status:** Draft 1&#x20;

<figure><img src="../../../.gitbook/assets/1 (3).png" alt=""><figcaption></figcaption></figure>

## Summary

Allocate a portion of the community fund for staking to bolster zAsset liquidity on DEXs, while not claiming the weekly rewards.&#x20;

## Specification

* Move 15,000,000 HZN from the [Ecosystem and Community Fund](https://academy.horizonprotocol.com/horizon-protocol/introduction/tokenomics#horizon-protocol-supply-and-inflation-policy) to a new Community Fund Staking Wallet&#x20;
* Stake the HZN at the Target C-Ratio and mint zUSD
* Do NOT claim the weekly reward to allow the unclaimd rewards flow back into the global rewards pool
* Utilize the zAssets for the zUSD and zBNB liquidity pools
* Maintain at least a 300% C-Ratio to avoid [liquidation risk](https://academy.horizonprotocol.com/horizon-genesis/staking-on-horizon-genesis/liquidation)&#x20;

## Motivation

The main motivation for this is to boost the liquidity of our liquidity pools in preparation for:

* The launch of the [Futures Exchange](https://horizonprotocol.medium.com/tech-update-88fd70890b3)
* The launch of Loans
* The launch of Shorting in the Exchange
* Additional partnerships (i.e. DEX aggregators)

Increased zAsset liquidity on the open markets brings substantial benefits to all users of our protocol. It will reduce slippage, ensuring more favorable trading prices for our on-off ramps, stabilizing the [zUSD peg](https://academy.horizonprotocol.com/horizon-protocol/synthetic-assets-zassets#zusd), and facilitating more seamless trading for both existing and new users.

Furthermore, staking the Community Fund’s HZN will also boost our protocol's total value locked (TVL).



## Potential Risks

The implementation of this HIP might come with some risks, including the following:

* In the first week of the implementation, existing stakers will see lower rewards and APY than normal due to the protocol automatically distributing rewards for the new HZN being staked. In the second week, the rewards will be normalized again as the unclaimed rewards from the first week will be distributed back to everyone in the second week.&#x20;

The C-Ratio will have to be watched and mantained to prevent liquidation, but since no rewards will be claimed, [maintaining the Target C-Ratio](https://academy.horizonprotocol.com/horizon-genesis/staking-on-horizon-genesis/collaterialization-and-c-ratio#managing-c-ratio-and-rewards-summary) on target is not necessary. The protocol will take action to restore the C-Ratio if it falls below 300% and return it back to at least 400%.

## Considerations

Additional thoughts we should take into consideration:

* The amount of HZN used is subject to the liquidity needs of the protocol while also not overexposing the community fund. 15 million HZN is proposed as a starting value that can be adjusted to be higher or lower as needed over time.
* A specific wallet will be dedicated to staking the community fund.

In preparation for [HIP-10](hip-10-use-zassets-from-community-fund-staking-to-provide-liquidity-on-wombat-exchange.md) where we provide liquidity on Wombat Exchange, we plan to use the zAssets obtained from staking the Community Fund to provide liquidity in the form of zUSD and zBNB. zUSD and zBNB are dominant assets in [the global debt pool](https://dashboard.horizonprotocol.com/#zasset), but the additional zUSD and zBNB from the Community Fund might affect the token distribution in the global debt pool. If there are any changes in the global debt pool, the approach can be adjusted accordingly to align with the token distribution in the global debt pool.

&#x20;

## Feedback & Questions

Please ask your questions here.
