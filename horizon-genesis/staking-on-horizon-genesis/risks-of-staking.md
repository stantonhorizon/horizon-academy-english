# Risks of Staking

{% hint style="danger" %}
This version of Horizon Academy has been deprecated! To find the latest version, please visit: [English V2](https://academy.horizonprotocol.com/)
{% endhint %}

Staking on Horizon Genesis is not risk free. Below are considerations and strategies to reduce the amount of risk you face.

## HZN Price Fluctuations and your C-Ratio <a href="#hzn-price-fluctuations-and-your-c-ratio" id="hzn-price-fluctuations-and-your-c-ratio"></a>

C-Ratio needs to be maintained to collect rewards. There are two states that your HZN can be in:

* **'Staked'** - HZN in your wallet is staked and earning rewards, but cannot be transferred
* **'Transferable'** - HZN in your wallet is not staked and can be transferred whenever

There are two ways in which C-Ratio can change:

* If the market price of HZN increases, the HZN you need to collateralize your position will reduce and your current C-Ratio will increase. Horizon Genesis will automatically release the amount of staked HZN you have to become Transferable HZN (or Escrowed HZN if you have staked your rewards) in order to always maintain a 700% ratio based on your current debt. You have the option to re-stake the extra available HZN.
* If the market price of HZN decreases, your C-Ratio will decrease. If you have Transferable or Escrowed HZN available, Horizon Genesis will automatically migrate those balances to become Staked HZN in order to always maintain the 700% collateralization ratio.

There are two ways to maintain your C-ratio:

* Burn some zUSD. This pays back some or all of your debt and will increase your C-Ratio.
* Stake more HZN. This provides more collateral and will increase your C-Ratio. If your current C-Ratio is under 700%, just adding HZN to your wallet will automatically stake your HZN (up to 700%).

## Price Fluctuations in the Global Debt Portfolio

The Global Debt Portfolio is comprised of the value of all zAssets in Horizon Protocol.

When a user initially mints zUSD by staking HZN, this zUSD is considered debt that you owe Horizon Protocol. To unstake your HZN, you must return this debt.

When minted, the zUSD value is locked in as a percentage of the Global Debt Portfolio. When the Global Debt Portfolio increases in size due to zAssets going up in value, then the amount of debt owed will also go up. Alternatively, if the value of the Global Debt Portfolio goes down, then the amount of debt owed will also go down.

For example, if the Global Debt Portfolio is currently worth $990,000 USD and you come along to mint $1,000 zUSD, the total Global Debt Portfolio is now $1,000,000 USD and your $1,000 zUSD is worth 0.1% of the Global Debt Portfolio. At this point, your debt is $1,000 zUSD.

If some users decide to buy other zAssets with their zUSD, the Global Debt Portfolio will now potentially fluctuate in price. Let's assume that the Global Debt Portfolio balloons to $1,010,000 zUSD, an increase of 1%. This would affect your debt 1% as well, with your debt going from $1,000 to $1,010 USD. This means that you now need to burn or pay back $1,010 zUSD to unstake your HZN.

If the Global Debt Portfolio decreases by 1% to $990,000, then your debt will also go down from $1,000 to $990, which means that you now only need to burn or pay back $990 zUSD to unstake your HZN.

## Missed Claims <a href="#missed-claims" id="missed-claims"></a>

Claims are available until the next reward claim period starts (7 days). Make sure to collect your claims before they expire. Rewards that are not claimed during the week are no longer available to the user and are distributed to the following week's reward pool for everybody to earn.

## Liquidation

If your C-Ratio falls below 200% you will be flagged for liquidation. Once you are flagged for liquidation, you have 3 days to restore your C-Ratio back to 700% and remove the liquidation flag, otherwise, you can be liquidated. Once you are back to a C-Ratio of 700%, you can execute the transaction to clear your liquidation flag. Please note that if you restore your C-ratio back to 700%, but fail to remove the liquidation flag, your account will still be vulnerable to liquidation if you ever go under 700%. If your account does get liquidated, this flag is automatically removed without the user needing to clear it. To learn more about how liquidation works under the hood, please go to the [Liquidation](liquidation.md) page.

Please check the [strategy](c-ratio-strategies.md) section for more details on how to approach staking HZN and the best approach that fits you.

![](../../.gitbook/assets/hzn-docs-liquidation1.png)
