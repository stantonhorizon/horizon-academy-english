# Exchange Fees

When trading on the Horizon Exchange, each trade is charged an exchange fee. The exchange fee is dependent on the zAsset (so each zAsset will have a slightly different fee, designated by the oracle) because every zAsset has its own oracle price feed, and therefore a corresponding heartbeat and price variance threshold.

Learn more about oracle heart beat and variance by going to the [Oracles](oracles.md#oracle-refresh-rate) page.

## Fees based on Price Variance

Fees are based on the price variance of a zAsset. Each zAsset has a price variance, which dictates the amount of price movement required for the zAsset's oracle to refresh.

To disincentivize users from using the variance threshold to front-run the oracle’s price, the exchange fees are always at least equivalent to the price variance.

For example, if a zAsset has a price variance threshold of 1%, the exchange fee on Horizon Exchange for that zAsset will also be 1%.

## **Trading Delays and its affect on Fees** <a href="#fbee" id="fbee"></a>

Whenever a trade occurs on Horizon Exchange, you will notice a 3 minute waiting period that will prevent you from being able to exchange, transfer, or burn the zAsset you just traded.

This delay is to prevent front-running due to oracle latency, which occurs when a price change occurs in Horizon Exchange and it must be updated on-chain, but there is a delay between the time that the oracle updates and the price seen by the traders on Horizon Exchange. To handle this delay, the Fee Reclamation & Rebates system is set up.

The Fee Reclamation & Rebates system on Horizon Protocol enables a 3 minute oracle check where users cannot exchange, transfer, or burn the zAssets they have just traded into. The time period gives oracles enough time to check for a difference between the initial price and the new price. This verifies whether or not a trade would have been impacted by an oracle lag time and prevent front-running.

If a trade was affected by the oracle latency, that will mean the price is wrong and the trader will either owe zAssets (known as reclamation) or is owed zAssets (known as a rebate).

If there is a reclamation or rebate, it gets remembered on chain and activated the next time the trader exchanges, transfers, or burns that same zAsset. At that time, Horizon Exchange will automatically reclaim the zAssets the trader owes (reclamation) or it will payout the zAssets owed to the user (rebate).&#x20;

The reclamation and rebate of the fee is taken care of by the fee pool, where if a trader owes a reclamation, it is paid into the fee pool and if a trader is owed a rebate, it is paid from the fee pool.

It is possible to manually settle a fee settlement, but it will typically automatically occur the next time you exchange, transfer, or burn that particular zAsset.

To learn more about the Fee Reclamation & Rebates system, click [here](https://blog.synthetix.io/how-fee-reclamation-rebates-work/).
