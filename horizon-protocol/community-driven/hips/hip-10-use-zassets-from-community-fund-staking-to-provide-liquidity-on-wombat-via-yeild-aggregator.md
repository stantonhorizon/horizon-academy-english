---
description: >-
  Leverage the zAssets minted in HIP-7 and provide liquidity to the zUSD and
  zBNB liquidity pools on Wombat Exchange through Magpie or Wombex Finance.
---

# HIP-10: Use zAssets from Community Fund staking to provide liquidity on Wombat  via Yeild Aggregator

**Type:** Horizon Improvement Proposal \
**Date:** Sep 29th, 2023\
**Status:** Draft 3

<figure><img src="../../../.gitbook/assets/4.png" alt=""><figcaption></figcaption></figure>

## Summary

Should HIP-7 and HIP-9 pass, this HIP proposes to stake the liquidity through Magpie or Wombex Finance,  both are the top yield aggregators built on top of Wombat Finance. The utilization of a yield aggregator will increase the revenue generated for the liquidity staked, which will be directed in full back to the Community Fund. The tokens received will be in the form of WOM and MPG or WMX tokens, which will generate additional revenue and serve the purpose of the community fund, offsetting costs and aiding in the sustainable growth of the protocol.

## Specification

* Distribute zAsset liquidity to the zUSD and zBNB liquidity pools&#x20;
* Earn WOM and MPG or WMX tokens
* WOM and MPG or WMX will be added to the community fund and potentially sold in the open market when needed.

## Motivation

The motivation behind this initiative is to achieve the following objectives:

* Increase liquidity on open markets: By better incentivizing liquidity provision, we aim to enhance the liquidity available on various markets, making them more robust and efficient.
* Generate revenue for the protocol: Through this incentivization process, we intend to generate additional non-HZN revenue for the protocol, ensuring its longer term sustainability and growth.

## Potential Risks

The implementation of this HIP might come with some risks, including the following:

* Magpie and Wombex is another layer of smart contracts on top of Wombat Exchange, introducing additional smart contract risk, more specifically, the MPG or WMX token rewards. Liquidity staked through Magpie or Wombex are still ultimately deposited into Wombat Exchange and are not in the custody of Magpie or Wombex.

## Considerations

Additional thoughts we should take into consideration:

*   Staking the zAssets from the community fund in Wombat via a yield aggregator like Magpie or Wombex might result in reduced WOM token rewards for other liquidity providers, but it is essential to prioritize maximizing liquidity for the overall benefit of the protocol. The primary objective is to ensure ample liquidity, which is crucial for the protocol's success. Additionally, any revenues generated through this process would help with the long-term sustainability of the Community Fund.





## Feedback & Questions

Please ask your questions [here](https://t.me/HorizonProtocol).

**Q: What’s Magpie?**[ ](http://wombex.exchange)

[Magpie](https://www.magpiexyz.io/) is the first protocol within Magpie XYZ, designed to provide yield and veTokenomics boosting services for Wombat Exchange. Incubated by[ Wombat Exchange](https://www.wombat.exchange), Magpie is focused on locking WOM tokens to own governance rights and boosted yield benefits as liquidity provider on Wombat.

The platform offers users the opportunity to deposit their Stablecoins, BNB, Liquid BNB, frxETH, ETH, WOM, mWOM tokens in single-sided boosted pools to earn high APR % while it allows Wombat Exchange voters to cost-effectively acquire voting power and earn passive income at the same time through the MGP token.

Magpie ranked #7 based on TVL locked in the Yeild category across all chains and #3 on the BNB Chain, current TVL 60.15M on 4 chains.\


**Q: What’s Wombex?**\
[Wombex](http://wombex.exchange) combines the power of liquidity providers and WOM token holders, supercharging each other and accelerating long-term Wombat growth. For this purpose, Wombex accumulates veWOM and aggregates LPs deposits simultaneously. For WOM holders, Wombex offers the opportunity to earn more on their WOM by staking WOM into wmxWOM (Wombex-owned veWOM).

Wombex ranked #28 based on TVL locked in the Yeild category across all chains and #6 on the BNB Chain, current TVL 9.59M.



**Q: What are the risks for staking in Wombex?**

Wombex operates its contracts on Wombat Exchange's pools and gauge contracts, which are similar to vaults. For users of Wombex, the main risks to consider are the coverage ratio on pools for LPs (liquidity providers) and the potential for low bribe efficiency (if happens) on Wombat gauges.

Wombex actively participates on Wombat Exchange using its highest veWOM (Wombat governance token) and TVL (Total Value Locked) contribution. This activity allows them to earn WOM tokens as rewards for providing liquidity in LPs. Additionally, they add WMX rewards on top of this and share these rewards with the LPs.

It's important to note that if the values of tokens decrease, there might be a lower risk in terms of rewards based on their USD value, but this risk is not spread out in a proportional emission manner. In simpler terms, the rewards might be impacted by token value changes, but not necessarily in a straightforward, proportional way.

\
**Q: How does Wombex approach security?**

Wombex have three audits which are conducted by Peckshield, Zokyo, and Slowmist.&#x20;

The Devs at Wombex take these audits very seriously. They wait for the results of these checks before introducing new contracts. The Devs are skilled with smart contracts and don't rush when adding new features. They continuously test things, and if they aren't completely sure and haven't seen results, they won't release any new features. This approach has kept them safe from security problems.

On the community side, Wombex values user input. They gather feedback about both the technical aspects (contracts) and the user experience (UX-UI). The community is actively involved and shares their thoughts. The community team then sends this feedback to the Devs using a platform called GitHub. The Devs pay attention and fix mistakes or bugs based on the feedback. They also enhance the protocol according to the suggestions from the community.

\
