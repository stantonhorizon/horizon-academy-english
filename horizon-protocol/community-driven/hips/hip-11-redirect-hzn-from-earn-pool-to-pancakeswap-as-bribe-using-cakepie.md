---
description: >-
  Utilize PancakeSwap’s incentive system to incentivize liquidity for HZN-BNB in
  the form of CAKE tokens by using Cakepie bribery market
---

# HIP-11: Redirect HZN from EARN Pool to PancakeSwap as ‘Bribe’ using Cakepie

<figure><img src="../../../.gitbook/assets/HIPs.png" alt=""><figcaption></figcaption></figure>

### Summary

PancakeSwap’s new [Gauges voting incentive system](https://blog.pancakeswap.finance/articles/introducing-gauges-voting-and-ve-cake-your-ownership-of-cake-emissions) can potentially provide more value than our current earn pools by leveraging veCAKE incentives and Cakepie’s bribe system, with the potential to distribute more incentives than relying solely on our current earn pool.

By redirecting a portion or all of the HZN typically directed towards EARN, to Cakepie’s Bribery Market and sunsetting the HZN-BNB pool on Earn, users can earn the equivalent or greater in CAKE tokens. They'll also have the ability to earn extra HZN by following Cakepie’s incentive system.&#x20;

By providing HZN-BNB liquidity, liquidity providers will earn the CAKE tokens directed from the PancakeSwap governance system. PancakeSwap’s incentive system will offer more value than our current earn pools by leveraging their incentive system, potentially distributing more incentives than relying solely on our current earn pool.

### Specification

* Re-distribute a portion or the same amount of weekly HZN rewards to Cakepie Bribery Market as "Bribes," incentivizing Cakepie’s and PancakeSwap’s governance users to allocate voting power and CAKE emissions to our liquidity pool. (We currently offer 144,000 HZN to EARN per week for the HZN-BNB pool)
* Sunset the HZN-BNB LP staker on Horizon Protocol.&#x20;

### Motivation

The main motivation is to incentivize greater liquidity for our core token HZN on PancakeSwap and increase the incentives for liquidity providers by utilizing PancakeSwap’s incentive system and Cakepie Bribery Market. For the same HZN currently distributed in Earn, an equivalent or greater value in CAKE will be distributed to liquidity providers. Additionally, the HZN itself can be earned by voting for our pool on Cakepie Bribery Market.\
A secondary motivation is to further strengthen our network of partners in the DeFi ecosystem, building trust and reaching a wider user base that can get to know and take interest in Horizon Protocol.

### Potential Risks

The implementation of this HIP might come with some risks, including:

* If the incentive program on PancakeSwap changes such that it no longer provides more rewards than when Horizon Protocol directly incentivizes the liquidity ourselves, it might be more logical to reactivate our EARN pool. The community would need to monitor this ratio, and the protocol will collaborate with PancakeSwap to ensure its economic feasibility.
* Interacting with a decentralized application (dApp) involves a number of associated risks, like smart contract risks and front end risks, for example. Users that interact with Cakepie will face these risks, similar to interacting with any other dApp.&#x20;

### Considerations

Additional thoughts we should take into consideration:

* Add instructions on how to maximize gains in Horizon Academy: With the PancakeSwap incentive system, users will earn CAKE tokens instead of HZN when staking their LP tokens. The CAKE tokens are offered by PancakeSwap, and the HZN sent to Cakepie will determine the initial value of the CAKE tokens distributed to the BNB-HZN liquidity pool. HZN tokens are also used as an incentive in Cakepie Bribery Market, acting as "bribes" to attract users to vote in the PancakeSwap governance system. More votes lead to larger CAKE rewards. The HZN “bribe” is distributed through Cakepie among the wallets of users who have allocated and voted for this liquidity pool.\
  \
  \
  **About PancakeSwap**\
  [PancakeSwap](https://pancakeswap.finance/) is a decentralized exchange (DEX) that operates across multiple blockchain networks, allowing users to conduct cryptocurrency trades without the need for middlemen or traditional financial institutions. As the biggest platform on [BNB Chain](https://www.bnbchain.org/en), PancakeSwap is renowned for its three core features: trading, earning, and winning. Users can instantly swap assets, earn tokens by providing liquidity or staking in Syrup Pools, and take part in lotteries and games to win tokens or NFTs.\
  \
  \
  **About Cakepie**\
  Cakepie is a state-of-the-art SubDAO created by Magpie to bolster the long-term sustainability of PancakeSwap. As a yield and veTokenomics service provider, Cakepie’s core mechanism involves locking CAKE tokens as veCAKE. This process allows Cakepie to secure enhanced yields and amplified voting rights within PancakeSwap, serving up as a Meta-Governance layer, providing prime opportunities for DeFi users.
