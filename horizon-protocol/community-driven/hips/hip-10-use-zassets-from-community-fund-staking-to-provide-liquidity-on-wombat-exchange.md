---
description: >-
  Leverage the zAssets minted in HIP-7 and provide liquidity to the zUSD and
  zBNB liquidity pools on Wombat Exchange through Wombex Finance
---

# HIP-10: Use zAssets from Community Fund staking to provide liquidity on Wombat via Wombex Finance

**Type:** Horizon Improvement Proposal \
**Date:** Aug 29th, 2023\
**Status:** Draft 2

<figure><img src="../../../.gitbook/assets/4.png" alt=""><figcaption></figcaption></figure>

## Summary

Should HIP-7 and HIP-9 pass, this HIP proposes to stake the liquidity through Wombex Finance, the top yield aggregator built on top of Wombat Finance. The utilization of a yield aggregator will increase the revenue generated for the liquidity staked, which will be directed in full back to the Community Fund. The tokens received will be in the form of WOM and WMX tokens, which will be sold on the open market to generate additional revenue and serve the purpose of the community fund, offsetting costs and aiding in the sustainable growth of the protocol.

## Specification

* Distribute zAsset liquidity to the zUSD and zBNB liquidity pools&#x20;
* Earn WOM and WMX tokens
* WOM and WMX will be added to the community fund and potentially sold in the open market when needed.

## Motivation

The motivation behind this initiative is to achieve the following objectives:

* Increase liquidity on open markets: By better incentivizing liquidity provision, we aim to enhance the liquidity available on various markets, making them more robust and efficient.
* Generate revenue for the protocol: Through this incentivization process, we intend to generate additional non-HZN revenue for the protocol, ensuring its longer term sustainability and growth.

## Potential Risks

The implementation of this HIP might come with some risks, including the following:

* Wombex is another layer of smart contracts on top of Wombat Exchange, introducing additional smart contract risk, more specifically, the WMX token rewards. Liquidity staked through Wombex are still ultimately deposited into Wombat Exchange and are not in the custody of Wombex.

## Considerations

Additional thoughts we should take into consideration:

* Staking the zAssets from the community fund in Wombat via Wombex might result in reduced WOM token rewards for other liquidity providers, but it is essential to prioritize maximizing liquidity for the overall benefit of the protocol. The primary objective is to ensure ample liquidity, which is crucial for the protocol's success. Additionally, any revenues generated through this process would significantly extend the protocol's runway, enabling it to achieve long-term objectives.

## Feedback & Questions

Please ask your questions here.

**Q: What’s Wombex?**\
[Wombex](http://wombex.exchange) combines the power of liquidity providers and WOM token holders, supercharging each other and accelerating long-term Wombat growth. For this purpose, Wombex accumulates veWOM and aggregates LPs deposits simultaneously. For WOM holders, Wombex offers the opportunity to earn more on their WOM by staking WOM into wmxWOM (Wombex-owned veWOM).

the top yield aggregator built on top of Wombat Finance.,&#x20;

Wombex ranked #28 based on TVL locked in the Yeild category across all chains and #6 on the BNB Chain, current TVL 9.59M.



**Q: What are the risks for staking in Wombex?**

Wombex has been built with safety and security in mind. However, there are inherent risks when interacting with any DeFi smart contracts. Our contributors have vigorously reviewed its smart contracts, and also pursued external auditors to identify potential vulnerabilities in the platform prior to launch.

However, there are certain risks of using Wombex that provide non-zero potential exposure to the risk of losing funds. These risks included:

* Risks of BNB/Arbitrum Chain vulnerabilities/operational issues as the underlying L1 or blockchain risks
* Risks of Wombat.exchange as underlying platform for Wombex operation since Wombex is tightly integrated with Wombat
* Wallet Risks (Metamask, etc) and node infrastructure risks
