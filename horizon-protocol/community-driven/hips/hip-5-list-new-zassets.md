---
description: Add new zAssets to Horizon Exchange
---

# HIP-5: List New zAssets

**Type:** Horizon Improvement Proposal\
**Date:** September 16th, 2022\
**Status:** Draft 1

## Summary

Add the following new zAssets that can be longed on Horizon Exchange:&#x20;

* Polygon (MATIC)&#x20;
* Avalanche (AVAX)&#x20;
* Amazon (AMZN)&#x20;
* Microsoft (MSFT)&#x20;
* Nvidia Corporation (NVDA)

## Specification

The zAssets will be added to the protocol using the following Chainlink aggregators:&#x20;

* MATIC - 0x7CA57b0cA6367191c94C8914d7Df09A57655905f&#x20;
* AVAX - 0x5974855ce31EE8E1fff2e76591CbF83D7110F151&#x20;
* AMZN - 0x51d08ca89d3e8c12535BA8AEd33cDf2557ab5b2a&#x20;
* MSFT - 0x5D209cE1fBABeAA8E6f9De4514A74FFB4b34560F&#x20;
* NVDA - 0xea5c2Cbb5cD57daC24E26180b19a929F3E9699B8

Trading for AMZN, MSFT, and NVDA will be halted on Horizon Exchange when markets are closed as the oracles will not be live during this time.

## Motivation

Listing new zAssets will increase the diversity of tradable assets by increasing the diversity of tradable assets and therefore increase the utility of Horizon Protocol. The assets chosen for this release were driven by the wishes of the community and are all top tier assets in their respective industries. MATIC and AVAX are top 20 crypto projects and AMZN, MSFT and NVDA are some of the largest and well known publicly traded companies, therefore price manipulation risks are at a minimum given their market sizes.

## **Potential Risks**

The implementation of this HIP might come with some risks, including the following:

* Listing many zAssets at once could produce unexpected consequences in terms of impact on the global debt pool.&#x20;
* Public companies can have stock splits and reverse-stock splits which could cause risks to the global debt pool if not properly handled.

## Considerations

Additional thoughts we should take into consideration:

* While there is desire to ‘list as many zAssets as possible’, a more methodical approach of releasing zAssets in smaller batches and seeing how the system responds before adding more will be a more secure approach.

## Feedback & Questions

If you have any questions or concerns, please do not hesitate to reach out.
