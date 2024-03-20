---
description: Latest update - January 27th, 2023
---

# Roadmap & Achievements

{% hint style="danger" %}
This version of Horizon Academy has been deprecated! To find the latest version, please visit: [English V2](https://academy.horizonprotocol.com/)
{% endhint %}

<figure><img src="../../.gitbook/assets/May update.png" alt=""><figcaption><p>Roadmap &#x26; Achievements (2021-2023)</p></figcaption></figure>

## Areas of importance we plan to focus on in 2023: <a href="#id-08ea" id="id-08ea"></a>

* Increase open market liquidity/access points for HZN and zAssets
* Increase product usability and usage
* Increase project awareness
* Improve protocol utility
* Improve protocol robustness
* Continue our longstanding focus on security

## **Tech Roadmap** <a href="#b416" id="b416"></a>

On the tech front our objectives can be broken down into 3 sections:

* Smart Contracts
* Front End
* Security Audit

### Smart Contracts <a href="#id-1ecb" id="id-1ecb"></a>

Mentioned in our [previous tech updates](https://horizonprotocol.medium.com/tech-update-4bcb8c9f1a2c), a major focus this year is to launch a decentralized perpetual futures exchange where users can trade using leverage while having competitive fees and no slippage. We are very excited for this feature as it will greatly support the Horizon Protocol business model in generating fees for HZN stakers and greatly improve the utility and volume usage of the protocol.

To address the open market liquidity of zAssets challenge, new ways of collateralizing them is required to increase their circulating supply. With the planned introduction of [collateralized loans](https://academy.horizonprotocol.com/horizon-protocol/introduction/business-model#interests-via-zasset-loans-and-shorts) and [token wrappers](https://academy.horizonprotocol.com/horizon-protocol/introduction/business-model#wrap-unwrap-fees-for-token-wrappers), users will be able to acquire zAssets using other crypto assets more economically than staking HZN. These features will also increase opportunities for arbitrageurs to profit off of open-market price deviations.

* For loans, users will be able to unlock more potential with their assets by leveraging them to borrow zUSD at 150% C-Ratio or higher, allowing them to acquire more zAssets with the same collateral and potentially using the borrowed funds to generate additional returns.
* With token wrappers, users will be able to directly convert their crypto assets into their zAsset equivalents at a 1:1 basis (100% C-Ratio without risk of liquidation), making for the most efficient way possible to collateralize zAssets.

The implementation of dynamic trading fees will revolutionize protocol usage and unprecedented partnership opportunities by allowing the removal of the waiting period after each trade and eliminating oracle front running opportunities during periods of high price volatility.

### Other new features that are being investigated and/or developed (not in any particular order): <a href="#id-31ae" id="id-31ae"></a>

* Introduce market basket/indices tokens (such as an NFT basket)
* Allow the correction of the C-Ratio to be automated when claiming each week to allow for a complete stake-and-forget experience
* Introduce Limit Orders (create orders that are executed at a specific price)
* Introduce Stop Losses (create orders that close your position at a specific price)
* Reduce trading fees by exploring other decentralized oracles
* Improve the protocol liquidation mechanism to allow more users to participate in keeping the network healthy
* Simplifying user debt tracking
* Introduce tools for users to hedge the debt pool and to reduce their C-Ratio volatility

### Front End: <a href="#id-735a" id="id-735a"></a>

To address product usage challenges, a key part is improving the new user onboarding process and user experience. We noticed a limitation to this is occurring due to the fragmentation of all the product and services that users are required to use before they can start trading or staking (i.e. first buying HZN on PancakeSwap, then staking HZN to mint zUSD on Horizon Genesis, then trading zUSD on Horizon Exchange), they must go through 3 different websites with many steps in between to achieve this.

By creating a unified product/frontend that combines Horizon [Genesis](https://genesis.horizonprotocol.com/), [Exchange](https://exchange.horizonprotocol.com/), and [Dashboard](https://dashboard.horizonprotocol.com/) with a built-in Pancake/Ellipsis DEX frontend, we can make it easier than ever for users to access and utilize [HZN](https://academy.horizonprotocol.com/horizon-protocol/synthetic-assets-zassets#how-does-horizon-protocol-create-synthetic-assets), [zUSD](https://academy.horizonprotocol.com/horizon-protocol/synthetic-assets-zassets#zusd), and [zBNB](https://academy.horizonprotocol.com/horizon-protocol/synthetic-assets-zassets#zassets). This streamlined user journey will make it simpler and faster to get the most out of the protocol, and help remove significant user friction. A one-product redesign can not only improve the user experience, but also provide the opportunity to more easily scale new features such as adding in new front ends for Futures, Loans and Wrappers.

Lastly, if there is interest from the community, there are also opportunities to integrate additional onramps into our protocol by adding an interface that allows crypto holders from other chains to bridge into BNB Chain and buy HZN directly as well as possible fiat onramps via bank/credit cards.

### Security Audit

While our current protocol [has already been audited,](https://academy.horizonprotocol.com/horizon-protocol/introduction/security-audit) we are taking extra precautions to ensure the security of our users by contracting a secondary audit to review all the changes we are making. We will not launch on the mainnet until we are confident that all aspects of the protocol have been thoroughly tested and audited.\


## **Where We Are At and Next Steps** <a href="#a246" id="a246"></a>

Our successful and secure deployment of the core products of the protocol (Genesis, Exchange, Dashboard) has enabled us to move forward with expanding the utility and usage of the protocol, creating new use cases and reducing friction.

In 2023, we are thrilled to be building the next evolution of Horizon Protocol’s product ecosystem and are committed to deploying the new contracts and updated front ends to the testnet as early as Q2 (timeline is subject to change). With the Testnet, users will be able to play and test for themselves what’s in store for Horizon Protocol while we battle test the contracts and undergo a thorough security audit to ensure maximum security. Once the audit and the public testnet phase has completed, we look forward to launching everything on the mainnet!
