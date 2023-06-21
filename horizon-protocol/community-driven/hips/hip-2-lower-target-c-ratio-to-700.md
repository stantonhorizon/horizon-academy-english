---
description: Lower Target C-Ratio to 700% from 800%
---

# HIP-2: Lower Target C-Ratio to 700%

**Type:** Horizon Improvement Proposal\
**Date:** May 12th, 2022\
**Status:** Draft 2 | Completed

<figure><img src="../../../.gitbook/assets/2 (1).png" alt=""><figcaption></figcaption></figure>

## Summary

Lower Target C-Ratio to 700% to increase zAsset liquidity.

## Specification

* Set target C-Ratio to 700%
* In Horizon Genesis, adjust Preset Strategies to:
  * Conservative: 1200% → 1100%
  * Neutral: 1000% → 900%
  * Aggressive: 800% → 700%

## Motivation

Lowering the Target C-Ratio to 700% will increase the total zAsset liquidity by about 14%. Lowering the C-Ratio more incrementally will make changes less volatile and allow the community to see its impact on the system and on any open market liquidity pools (i.e. zUSD/BUSD LP on PancakeSwap). Despite the current state of the altcoin market over the last 6 months or so, no user has been liquidated in the history of Horizon Protocol with a 800% Target C-Ratio (Update note 220610: this statement was true as of May 12, but not true as of June 10th, 2022).

Currently there is about $420,000 in TVL in the zUSD/BUSD LP. By increasing the supply of zAssets, more zUSD liquidity can be potentially supplied to the LP, making new users who want to just trade on Horizon Exchange, and not have to stake HZN, able to have access to a more liquid pool. A more liquid stablecoin pool will make it easier for traders to enter the ecosystem as we continue to increase awareness for the project.

The zUSD/BUSD staking pool on Horizon Genesis still offers very high APY for stablecoin yield farming even with the current state of the altcoin market. By increasing zAsset liquidity, more users can participate in these lower IL staking rewards to boost liquidity in the pool.

## **Potential Risks**

The implementation of this HIP might come with some risks, including the following:

* Increased liquidity of zUSD could potentially mean additional sell pressure for zUSD on the open market which would further throw it off the $1.00 peg if the demand is lacking.
* Easier to reach the 200% liquidation C-Ratio, so users have to be 12.5% more vigilant in managing their debt.

## Considerations

Additional thoughts we should take into consideration:

* For stakers who are not participating in trading, lowering the c-ratio generally presents no upside (except that it produces more zAsset liquidity, which might help grow the project and increase HZN price).

## Feedback & Questions

**“If the C-ratio changes from 800% to 700% and everybody decides to now stake at 700% instead of 800%, how does the APY change? Is everybody more leveraged and incurring more risk, but for the same APY?"**\
In a sense, yes. By lowering from 800% to 700%, everyone is slightly closer to the 200% liquidation rate, hence, there is slightly more risk. But this is only if you choose to lower your C-Ratio to 700%. You can also maintain a higher C-Ratio, just like the other strategies available, but you would not be getting the maximum possible return from staking. It is important to note that the goal of all this is to increase liquidity in Horizon Exchange. The more liquidity, the more potential for users to try out the Horizon Exchange.
