---
description: Frequently Asked Questions for Horizon Genesis
---

# Genesis FAQ

## General

<details>

<summary><strong>What are the contract addresses?</strong></summary>

`HZN: 0xc0eff7749b125444953ef89682201fb8c6a917cd`

`zUSD: 0xf0186490b18cb74619816cfc7feb51cdbe4ae7b9`

</details>

<details>

<summary>Why HZN?</summary>

* Built on the BSC for faster, cheaper, scalable transactions
* More focus on bringing a wider range of synthetic assets that represent the real and crypto worlds
* Building more innovative synthetic assets such as zIndices, zNFTs, leveraged assets and others
* Bringing DeFi to NFTs via Synthetic NFTs
* Cross-chain interoperability: BSC, ETH, Solana, Polygon, Tron, Cosmos, Reef, and more
* Focused on user experience and education
* Community driven

</details>

<details>

<summary><strong>What are the tokenomics of HZN?</strong></summary>

To understand the tokenomics please refer to our [Supply and Inflation Policy article](https://horizonprotocol.medium.com/horizon-supply-and-inflation-policy-f0aaa8cc4a3a).

</details>

<details>

<summary><strong>What was the initial minted distribution for HZN?</strong></summary>

The initial minted supply of HZN tokens is 100,000,000.

Distribution:

* 10% (10,000,000 HZN) will be reserved for the IFO on PancakeSwap.
* 30% (30,000,000 HZN) will be reserved for Liquidity Mining (PHB, HZN, HZN-BNB LP) purposes.
* 60% (60,000,000 HZN) will be reserved for the Ecosystem & Community Fund.

</details>

<details>

<summary><strong>How will the 60M ecosystem funds be used?</strong></summary>

The 60M Ecosystem & Community Fund will be used to support the protocol and community via stabilization of synthetic asset collateralization, market making for synthetic assets, protocol grants and blockchain fees, bounties, partnerships, marketing, and other community incentives. None of these funds are going to the team, advisors, or investors and are not intended to ever be completely circulating in the market. This fund is the treasury of Horizon Protocol itself and is for the benefit and long term sustainability of the protocol. The intention for this fund is to eventually be completely governed by the community via a DAO.

</details>

<details>

<summary><strong>Will there be a deflation mechanism later?</strong></summary>

As our project evolves, we can certainly begin to implement deflationary mechanisms. If you wish to contribute to the discussion around this, please join our Telegram community [here](https://t.me/HorizonProtocol).

</details>

<details>

<summary><strong>Can we see any statistics in real-time?</strong></summary>

To see real-time network data and analytics for Horizon Protocol, check out the [Horizon Dashboard](https://dashboard.horizonprotocol.com).

</details>

## Staking

<details>

<summary>How do I stake my HZN?</summary>

To stake HZN you also need to mint zUSD, which is a stablecoin backed by your staked HZN. This zUSD must be paid back in order to reclaim your HZN and is considered as an interest-free debt. Staking HZN requires managing your Collateralization Ratio (C-Ratio) in order to be eligible for rewards and avoid liquidation.

Learn more about staking [here](staking-on-horizon-genesis/). Get started [here](guides/getting-started.md).

</details>

<details>

<summary>How can I unstake HZN?</summary>

You must burn zUSD in order to unstake HZN. Burning zUSD will reduce your debt which also reduces the amount of HZN required to back that debt.

* Any zUSD burned while under an 700% C-Ratio will only reduce your debt and increase your C-Ratio, but will not unstake any HZN.
* Any zUSD burned while over an 700% C-Ratio will reduce your debt AND unstake HZN at an 700% ratio. Reducing your debt to 0 would unstake all of your HZN. Unstaked HZN would become 'transferable' HZN, which is freely usable HZN.

</details>

<details>

<summary>Why can I still see my HZN in my wallet even though I have staked it?</summary>

When staking HZN in Horizon Genesis, your HZN will never actually leave your wallet. Horizon Genesis will automatically flag your HZN as 'staked' rendering it unusable until you unstake your position. HZN that isn't staked will be considered 'transferable' and freely usable to transfer or sell.

</details>

<details>

<summary>Why is my HZN staked amount constantly changing?</summary>

Horizon Protocol has a dynamic staking mechanism that automatically adjusts the amount of HZN staked based on the current price of HZN in order to always maintain an 700% backing of your current debt. Transferable and escrowed HZN are dynamically used to maintain an 700% C-Ratio as the price of HZN fluctuates.

Let’s take an example:\
(below calculations assumes 1 HZN = $1 and uses a C-Ratio of 800%, which was the original C-Ratio before being lowered to 700%)

1. You mint 100 zUSD with 800 HZN (1 HZN = $1) at 800% C-Ratio, your staked HZN balance would be 800 and your transferable HZN balance would be 0 (assuming you staked all of your HZN).
2. The price of HZN goes up to $1.5, now you would only need 533.33 HZN to back your 100 zUSD. Horizon Genesis would automatically release 266.67 HZN from being staked and it would become transferable HZN. This transferable HZN could then be freely used to mint more zUSD, transferred to another wallet, or sold on an exchange.
3. The price of HZN drops to $0.5, then you will need 1,600 HZN (1600 x $0.5 = $800) to back your 100 zUSD debt position. Horizon Genesis will automatically migrate any transferable or escrowed HZN in your wallet to become staked HZN until the necessary 1600 HZN backing is met. If you don’t have any transferable HZN, then your C-Ratio will fall below the 800% target C-Ratio and you will no longer be able to claim rewards.

</details>

<details>

<summary>What does staking have to do with minting and burning?</summary>

Staking HZN means that you are putting the HZN in there as collateral to Mint/Borrow zUSD. The reason it is called Minting instead of Borrowing is because there is no interest in this process. This is also why zUSD is called “Debt”, because you are technically borrowing this zUSD and you need to return it to be able to take back your HZN. An example of this would be a second mortgage, where you use your house as the collateral and you’re able to borrow some money. To get the house back to be fully under your ownership, then you need to pay back all the money first.

C-Ratio stands for collateralization ratio. This is the amount of collateral needed to borrow/mint a certain amount of zUSD. At 700%, you need $700 worth of HZN to mint $100 of zUSD.

If the price of HZN goes up to double the price, then your HZN is now worth $1400, which means that if you haven’t touched anything else, you are now at a c-ratio of 1400%. At this point, you can Mint again, which would take the extra $700 of HZN and borrow/mint to give you another $100 zUSD for a total of $200 zUSD at 700% c-ratio.

If the price of HZN drops by half back to the previous price so that it is worth $700 again, then you c-ratio has now dropped to 350%. To get back to 700% c-ratio, you need to “Burn”/repay $100 of zUSD so you are back at $100 zUSD of debt.

So the final conclusion is if you hold the zUSD that you mint and don’t do anything with it (trading it away or using it to invest in something else), you will have all the zUSD needed to “burn”/repay your zUSD debt and take out your collateral of HZN.

</details>

<details>

<summary>Why is there a timer blocking me from burning my zUSD?</summary>

There is a 24 hour period between minting and burning zUSD. This is necessary to prevent oracle front-running attacks.

</details>

<details>

<summary><strong>When I stake HZN, and there is the possibility of liquidation, to what degree is my position "leveraged"? I still have my balance of HZN. The threat of liquidation implies that it is leveraged, but this scenario does not seem to entail it?</strong></summary>

Liquidation in Horizon Protocol is not the same as liquidation of a leveraged or margin position. Your position in Horizon Protocol is not leveraged, you are actually over-collateralizing a debt position at an 700% ratio to back the creation of synthetic assets. Liquidation occurs when you lack sufficient backing of those synthetic assets. Please refer to the [liquidation section](staking-on-horizon-genesis/liquidation.md).

</details>

## Managing C-Ratio

<details>

<summary>What is C-Ratio?</summary>

Collateralization Ratio or C-Ratio is the ratio between your collateral and your debt. Horizon Protocol currently has a target C-Ratio of 700% meaning you need $7 worth of HZN staked to mint $1 zUSD to have a $1 debt. The purpose of the C-Ratio is to ensure that the synthetics produced by Horizon Protocol are sufficiently backed during price fluctuations.

</details>

<details>

<summary><strong>What happens if my C-Ratio drops below 700%?</strong></summary>

If your C-Ratio drops below 700% you will not be able to claim rewards. You will continue to gain rewards but will need to restore your C-Ratio to 700% by burning zUSD or adding more HZN in order to claim rewards. If you do not claim your rewards after a week, your rewards will be forfeited and redistributed to the following week's reward pool.

</details>

<details>

<summary><strong>How do I know how much zUSD to burn in order to rebalance my C-Ratio to 700%?</strong></summary>

Horizon Genesis has preset strategies to help you manage your C-Ratio. Simply clicking the “Aggressive - 700%” preset strategy will automatically calculate how much zUSD you need to burn to return to 700%. You may also manually input how much zUSD you want to burn if you want to maintain a different C-Ratio.

</details>

<details>

<summary><strong>When exactly am I in the liquidation zone?</strong></summary>

If your C-Ratio goes under 200% - you will be automatically flagged for liquidation. Horizon Genesis has a 3-day grace period to allow you to restore your C-Ratio and clear your liquidation flag before your account becomes available for liquidation. You will need to restore your C-Ratio back to 700% before you're able to clear your liquidation flag.

**WARNING:**

Please note that clearing your liquidation flag requires a blockchain transaction and is NOT automatic.

Learn more about liquidation [here](staking-on-horizon-genesis/liquidation.md).

</details>

<details>

<summary><strong>When I burn zUSD, do I also burn my HZN?</strong></summary>

No, you never lose HZN when burning zUSD. If your C-Ratio is under 700%, burning zUSD just reduces your debt and increases your C-Ratio. Once your C-Ratio is above 700% you will begin to unstake your HZN when burning zUSD. Reducing your debt to 0 would unstake all of your HZN. Unstaked HZN will become 'transferable' HZN, which is freely usable HZN.

</details>

<details>

<summary><strong>How come no transferable HZN is showing up when I burn zUSD?</strong></summary>

There are 2 reasons this can occur:

1. You are under 700% C-Ratio, therefore no HZN will actually become unstaked until you burn zUSD while over 700% C-Ratio.
2. All escrowed HZN you have used to stake must be first unstaked before un-escrowed HZN begins to unstake and become transferable.

</details>

## Rewards

<details>

<summary><strong>How are my rewards calculated for staking HZN in Horizon Genesis?</strong></summary>

Your rewards are calculated based on the proportion of your personal debt against the global debt pool. Your proportion of global debt is calculated based on a snapshot of the network taken every Friday around 15:00 UTC.

`Your Weekly Rewards = Personal debt/Global debt * Weekly Rewards`

</details>

<details>

<summary><strong>How do I maximize rewards?</strong></summary>

To maximize rewards you want to hold more debt and mint with all of your HZN (aggressive 700% strategy). Any price drop from the point of minting at 700% will result in you not being able to claim rewards. You have 1 week, until the next week’s reward period starts, to make sure your C-Ratio is at least 700% and claim your rewards or they will be forfeited and returned to the following week’s reward pool for others to earn.

**DANGER:**

Maximizing rewards is risky and requires more active management. Do not take on risk that you are not comfortable with.

</details>

<details>

<summary><strong>How long do I have to claim my rewards?</strong></summary>

You have until the next reward period to claim your rewards (7 days from when rewards are claimable). Unclaimed rewards will be redistributed into next week’s reward pool. You can see how long you have left to claim by checking the bottom right of the screen where you will see a timer until the next reward claim period.

</details>

<details>

<summary><strong>Will I still gain rewards if I don’t claim this week’s rewards?</strong></summary>

Yes, you will continue to gain rewards every week based on how much debt you hold. Any rewards you don’t claim each week will be forfeited and returned back to the reward pool for the following week's reward distribution.

</details>

<details>

<summary><strong>When do my rewards stop calculating?</strong></summary>

You will gain rewards as long as you have a debt position at the end of each reward period on Horizon Genesis. If you burn all your zUSD, you will no longer gain rewards.

</details>

<details>

<summary><strong>Why is the reward claim period only 1 week?</strong></summary>

The reward claim period coincides with the Horizon Protocol monetary policy, which distributes new tokens on a weekly basis.

In addition, it is very important to maintain the global C-Ratio, therefore, it is critical that stakers are active stakers, re-adjusting their individual C-Ratios at least once a week. Staking in Horizon Protocol is not a stake-and-forget type of system.

Please remember that rewards for the previous week must be claimed before the start of the next reward period or they will be forfeited and redistributed into the next week’s reward pool.

</details>

<details>

<summary><strong>Why can’t there be a setting to auto burn every 3 days, auto claim and auto stake rewards?</strong></summary>

Burning, claiming, and staking require transactions on the blockchain that need to be paid for by the user.

</details>

<details>

<summary><strong>How long are my rewards in escrow for?</strong></summary>

The vesting period for all claimed rewards is 1 year.

</details>

## Token Information

<details>

<summary>What is transferable HZN?</summary>

Transferable HZN is HZN that is available to be used in your wallet. You can transfer it or sell it, or keep it in your wallet to increase your C-Ratio. Having a good transferable HZN balance will help you maintain your debt position if the HZN price drops and you need more HZN to be staked. Horizon Genesis will automatically migrate your transferable HZN to become staked HZN in this event.

</details>

<details>

<summary><strong>What other forms of collateral will be available to use on Horizon Protocol?</strong></summary>

We’ll be looking into other forms of collateral such as BNB and other assets, but currently you can only use HZN as collateral.

</details>

<details>

<summary><strong>What is zUSD and how is it backed?</strong></summary>

zUSD is a stablecoin that is pegged to the US Dollar and is minted in Horizon Genesis when staking HZN as collateral. More collateral options will be available in the future.

</details>

<details>

<summary><strong>What can I do with zUSD?</strong></summary>

The main purpose of zUSD to is to use it to trade for other zAssets on Horizon Exchange. These zAssets are an array of synthetic assets representing the crypto and real economy (i.e. zBTC, zETH, zAPPL, zTSLA, etc.)

Additionally, for staking purposes, you can trade it on [PancakeSwap](https://pancakeswap.finance/swap?inputCurrency=0xF0186490B18CB74619816CfC7FeB51cdbe4ae7b9\&outputCurrency=0xe9e7cea3dedca5984780bafc599bd69add087d56) or compound your HZN staking rewards by supplying liquidity to the [zUSD/BUSD LP in PancakeSwap](https://pancakeswap.finance/add/0xe9e7CEA3DedcA5984780Bafc599bD69ADd087D56/0xF0186490B18CB74619816CfC7FeB51cdbe4ae7b9) and staking the LP for rewards in the Horizon Genesis [Earn](https://genesis.horizonprotocol.com/earn) tab.

</details>

<details>

<summary><strong>Where do zUSDs come from?</strong></summary>

zUSDs are always minted (and burned) at a value of $1.00 and are backed by the HZN you ‘stake’ into Horizon Genesis.

</details>

<details>

<summary>How can I see zUSD in my wallet?</summary>

Add the zUSD token address: `0xf0186490b18cb74619816cfc7feb51cdbe4ae7b9` to your wallet.

</details>

<details>

<summary><strong>How can I convert my zUSD to BUSD and add liquidity to the zUSD/BUSD pool on PancakeSwap?</strong></summary>

zUSD is tradeable on PancakeSwap [here](https://pancakeswap.finance/swap?inputCurrency=0xF0186490B18CB74619816CfC7FeB51cdbe4ae7b9\&outputCurrency=0xe9e7cea3dedca5984780bafc599bd69add087d56).

You can add liquidity for the zUSD-BUSD pool [here](https://pancakeswap.finance/add/0xe9e7CEA3DedcA5984780Bafc599bD69ADd087D56/0xF0186490B18CB74619816CfC7FeB51cdbe4ae7b9).

The zUSD/BUSD liquidity pool can be checked [here](https://bscscan.com/address/0xc3bf4e0ea6b76c8edd838e14be2116c862c88bdf).

zUSD token address: `0xf0186490b18cb74619816cfc7feb51cdbe4ae7b9`

</details>
