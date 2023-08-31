---
description: >-
  Utilize Wombat Exchange’s incentive system to incentivize liquidity for
  zUSD-USDC and zBNB-BNB pools in the form of WOM tokens
---

# HIP-9: Redirect HZN from EARN Pools to Wombat Exchange as ‘Bribes’

**Type:** Horizon Improvement Proposal \
**Date:** Aug 29th, 2023\
**Status:** Draft 2

<figure><img src="../../../.gitbook/assets/3 (1).png" alt=""><figcaption></figcaption></figure>

## Summary

[Wombat Exchange’s](https://www.wombat.exchange/) incentive system can provide more value than our current earn pools by leveraging Wombat’s incentives and [bribes system](https://medium.com/wombat-exchange/so-what-on-earth-are-bribes-bfb3b6521ae), with the potential of distributing more incentives than relying on just our current [earn pools](https://genesis.horizonprotocol.com/earn).

By redirecting a portion, or all, of the HZN normally going towards Earn to Wombat’s bribes (we currently have 75,000 HZN being offered to EARN per week for both the zUSD-BUSD and zBNB-BNB pools) and sunset both the zUSD-BUSD and zBNB-BNB pools on Earn, users will earn the equivalent, or greater, in [WOM tokens](https://docs.wombat.exchange/docs/tokenomics/about-wom#what-is-wom), with the ability to earn extra HZN by following the Wombat’s incentive system of staking their WOM tokens and [voting with veWOM](https://medium.com/wombat-exchange/wombats-voting-gauge-47c9ee4c8341).

By providing zUSD-BUSD or zBNB-BNB liquidity, liquidity providers will earn the WOM tokens directed from the Wombat governance system.[Wombat Exchange’s](https://www.wombat.exchange/) incentive system can provide more value than our current earn pools by leveraging Wombat’s incentive and [bribe system](https://medium.com/wombat-exchange/so-what-on-earth-are-bribes-bfb3b6521ae), with the potential of distributing more incentives than relying on just our current [earn pools](https://genesis.horizonprotocol.com/earn).

By redirecting a portion, or all, of the HZN normally going towards Earn to Wombat’s bribes (we currently have 75,000 HZN being offered to EARN per week for both the zUSD-BUSD and zBNB-BNB pools) and sunset both the zUSD-BUSD and zBNB-BNB pools on Earn, users will earn the equivalent, or greater, in [WOM tokens](https://docs.wombat.exchange/docs/tokenomics/about-wom#what-is-wom), with the ability to earn extra HZN by following the Wombat’s incentive system of staking their WOM tokens and [voting with veWOM](https://medium.com/wombat-exchange/wombats-voting-gauge-47c9ee4c8341).

By providing zUSD-USDC or zBNB-BNB liquidity, liquidity providers will earn the WOM tokens directed from the Wombat governance system.

Furthermore, liquidity providers who earn WOM will also have the opportunity to earn HZN by participating in the governance "bribe" system. This means their gains can compound further than is currently possible and reinforces the rewards for our liquidity pools.

\


## Specification

* Re-distribute a portion or the same amount of weekly HZN rewards to Wombat Exchange as "Bribes", which will incentivize the Wombat Exchange governance users to allocate WOM rewards to our liquidity pools

## Motivation

The main motivation is to incentivize greater liquidity for our zAsset pairs on Wombat Exchange and increase the incentives for liquidity providers by using Wombat Exchange’s incentive system. For the same HZN that is currently being distributed in Earn, an equivalent or greater value in WOM will be distributed to liquidity providers and the HZN itself can also be earned by voting for our pool using their governance token, veWOM, which you get by staking WOM.

\
Lastly, as proposed in HIP-10, a portion of the HZN distributed as bribes could be mined by the protocol, which can flow back to the community fund, and help alleviate increases to the [circulating supply of HZN](https://dashboard.horizonprotocol.com/#staking).

## Potential Risks

The implementation of this HIP might come with some risks, including the following:

* If the incentive program on Wombat changes to where it no longer provides more rewards than when Horizon Protocol directly incentivizes the liquidity ourselves. In this case, it would make more sense to reactivate our EARN pools again. The community would have to monitor this ratio and the protocol will work with Wombat to ensure it is economical to do so.&#x20;

## Considerations

Additional thoughts we should take into consideration:

* Add instructions on how to maximize our gains in Horizon Academy:\
  \
  With the Wombat Exchange incentive system, users will earn WOM tokens instead of HZN when staking their LP tokens. The WOM tokens are offered by Wombat Exchange, and the HZN that is sent to Wombat Exchange will designate the initial value of the WOM tokens that will be distributed to the zUSD-USDC and zBNB-BNB liquidity pools.\
  \
  The HZN tokens are also used as an incentive in Wombat’s governance system where they act as "bribes" to attract users in the Wombat governance system to allocate and vote with veWOM tokens. The more votes, the larger the WOM rewards. The HZN “bribe” is distributed among the wallets across the users who have allocated and voted with veWOM for this liquidity pool. veWOM tokens are acquired by staking WOM tokens.\
  \
  In other words, users in the Wombat governance system can accept the HZN token “bribes” by allocating and voting for our liquidity pools with veWOM to direct a larger portion of the weekly WOM token rewards to our pools.



* The default token earned via liquidity pools is now WOM instead of HZN.

&#x20;

## Feedback & Questions

Please ask your questions here.
