---
description: Liquidation Mechanism V2
---

# Liquidation Mechanism (Testnet V2)

{% hint style="danger" %}
This version of Horizon Academy has been deprecated! To find the latest version, please visit: [English V2](https://academy.horizonprotocol.com/)
{% endhint %}

Horizon Protocol is a protocol that requires the maintenance of collateral to make sure that all zAssets are backed by some underlying asset. In the case of Horizon Protocol, that underlying asset is the HZN token. The worst-case scenario is if the underlying asset's value is worth less than zAssets, because that would mean that zAssets are not completely backed anymore.

One of the mechanisms to prevent the worst-case scenario is the liquidation mechanism, which allows wallets that have gone below the safe C-ratio, or collateralization ratio, threshold to be liquidated by a third party to get them back to a safe C-ratio and ensure the protocol’s zAssets are sufficiently collateralized.\


## The current liquidation process is done in 2 steps:

1\. **Wallets that have fallen below the safe C-ratio threshold need to be flagged for liquidation. Flagging requires a transaction on the blockchain.** Currently, all flagging transactions are done by the Horizon Protocol team because there is no incentive for flagging. If flagging is not conducted, liquidations cannot occur.&#x20;

\


2\. Once flagged, and the flagging grace period has passed, a wallet can now be liquidated. To liquidate, zUSD is required to be burned. **The way the liquidation works is that the user performing the liquidation will burn zUSD on behalf of the wallet that needs to be liquidated, and the user will be given the zUSD equivalent value in the form of HZN tokens + a 10% incentive bonus, which is taken from the liquidating wallet.** From a user experience perspective, there are two issues. The first issue is that the user performing the liquidation needs to have zUSD on hand. How much each user can liquidate will be limited by the amount of zUSD they have. The second issue is that once they liquidate the zUSD, they now hold HZN, a much more volatile asset relative to the zUSD stablecoin. If they want to realize their gains from liquidating, they will have to sell their HZN to another stable asset. It is possible for this action to create additional sell pressure on HZN, which could lower the price of HZN and trigger more liquidations that could potentially lead to the theoretical possibility of price instability if the issue is extreme.



The Liquidation Mechanism V2 simplifies the above two actions, provides the appropriate incentives to allow the community to take action more effectively, and eliminates the theoretical possibility of a HZN price instability.



## How Liquidation Mechanism V2 Works

Liquidation Mechanism V2 also can be broken down into two steps:

1\. Wallets that have fallen below the safe C-ratio threshold need to be flagged for liquidation. But now, there is an incentive for flaggers to flag wallets. Flagging wallets will now transfer over a flat fee of HZN from the flagged wallet to the flagger. Flagging a wallet adds them to a Liquidation List.\


2\. Once flagged, a wallet will be able to be liquidated after a certain amount of time (will most likely be set to 12 or 24 hours). To liquidate, a liquidator can just liquidate without the need of any zUSD collateral, and will earn a flat fee of HZN for performing the liquidation, taken from the wallet being liquidated. This process simplifies the entire process as there will be no need to carry zUSD or convert HZN back to zUSD afterward. It will just be a simple blockchain call that requires gas, and a flat fee reward that will cover gas costs plus extra to incentivize the action. The wallet that gets liquidated will pay for the flagging and liquidation fees given to the users who call the functions.\


The liquidation mechanism removes HZN from the wallet being liquidated until the wallet gets back to the correct C-Ratio, with an additional penalty. The initial HZN is used to pay back your debt. The penalty HZN is then deposited into a pooled contract that is re-distributed proportionally to all stakers based on the staker's Debt Share.

Note that liquidated HZN will need to be claimed and escrowed for 1-year upon claiming, but there is no deadline for claiming and any unclaimed HZN from liquidation rewards can still be used as collateral to back zUSD.



The Liquidation Mechanism V2 also allows for two new concepts:

\- Liquidation using Escrowed HZN

\- Self-Liquidation



**Liquidation using Escrowed HZN** means that Escrowed HZN can now be used as part of the liquidation process. Previously, because escrowed HZN could not be touched, there was a possibility of there not being enough wallet HZN (transferable HZN) to cover the debt. When a wallet is liquidated, it will first liquidate the wallet’s HZN, and if that balance is insufficient, it will utilize the HZN locked in the Escrow contract. When accessing the Escrow contract for HZN, the protocol will take the most recent escrow entries and unlock them in descending order until enough HZN has been unlocked to restore the wallet’s C-Ratio. Any leftover HZN unlocked from escrow will be put back in escrow as a new entry with the same vesting deadline as the last entry unlocked. All HZN liquidated from escrow will move to the LiquidatorRewards contract for distribution back to HZN stakers and escrowed for 1-year once claimed.&#x20;

\


**Self-Liquidation** is a new alternative method for a user to restore their C-Ratio. Self-liquidation enables a user to restore their C-Ratio using the HZN in their wallet instead of having to only burn zUSD. A user can self-liquidate at any time when their C-Ratio is below the target, and the protocol will liquidate HZN from their wallet in order to forgive debt, but doing so will come at a penalty (between 20-50%, adjustable via HIP). Note that the user cannot self-liquidate escrowed HZN. This is an additional option for when you have all your zUSD locked up and have no other option but to burn your HZN instead. Similar to ‘Forced Liquidation’, all HZN removed from self-liquidation will be sent to the LiquidatorRewards contract for distribution back to HZN stakers and escrowed for 1-year once claimed. &#x20;

\


## **Liquidation Mechanism V2 and its Benefits**

Liquidation Mechanism V2 plugs a few holes in Horizon Protocol, making it safer for liquidity and stakers by completely stopping liquidating HZN from instantly becoming circulating, opening up escrowed HZN to be liquidated, and providing a significantly more simplified and properly incentivized liquidation experience.

Benefits of using Liquidation Mechanism V2 over the previous version include:

\- Added an incentive for  users to flag wallets that have fallen below a safe C-Ratio, promoting a more decentralized community process.

\- The liquidation action is significantly simplified with a flat fee reward, no collateral requirements, and a redistribution of debt from a less responsible staker to more responsible ones.

\- Prevents the possibility of an HZN price instability due to a spiral of selling liquidated HZN and triggering more liquidations by redistributing all liquidated HZN back to the community of stakers and being escrowed for 1 year..

\- Introduces the ability to use escrowed HZN for liquidation, which fixes a potential bug in liquidating wallets with not enough accessible collateral

\- Introduces the option of Self-Liquidation, which provides an alternative method for wallets to get back to a proper C-Ratio and keep the protocol’s active ratio healthier.

\
