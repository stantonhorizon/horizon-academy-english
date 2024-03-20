# Dynamic Exchange Fees (Testnet V2)

{% hint style="danger" %}
This version of Horizon Academy has been deprecated! To find the latest version, please visit: [English V2](https://academy.horizonprotocol.com/)
{% endhint %}

In the Horizon Protocol Exchange, every time a trade between two different assets is completed, an "oracle delay" is used to prevent front-running and arbitrage due to volatility.

Dynamic Exchange fees allow trading to be instantaneous with no more "oracle delay".

Dynamic exchange fees introduce a dynamic fee on top of the normal exchange base fees for the spot exchange and will be based on the market's volatility. If there is a lot of market volatility, the dynamic exchange fees will increase, while when the market is calm, the dynamic exchange fees will decrease to 0.

## How Dynamic Exchange Fees work

The idea of a dynamic exchange fee is to make it unprofitable for front-runners or parties that are taking advantage of volatility arbitrage.

A dynamic exchange fee contract tracks the price of a zAsset across epochs and as the price swings, the dynamic exchange fee will increase and be applied as an additional fee over the base fee. A decay factor is applied to the dynamic exchange fee the entire time, which means that over time, as the price stabilizes, the dynamic exchange fee will go back down to 0.

To simplify:

* price volatility = dynamic exchange fee going up
* price stability = dynamic exchange fee gradually going down to 0

The dynamic exchange fee will be different for each zAsset and it will be dependent on the market volatility for that zAsset.

## Dynamic Exchange Fees and their benefits

The biggest benefit is that Horizon Protocol's spot exchange can now be integrated with DEX aggregators. DEX aggregators require instant trades, which was not possible before with our "oracle delay".

With Dynamic Exchange Fees, the fees can be immediately calculated for instantaneous trades, making possible the pathway for DEX aggregators to leverage Horizon Protocol for trades with zero slippage, a very attractive option for larger trades.

The upgrade to Dynamic Exchange Fees allows Horizon Protocol and zAssets to provide a lot more utility to the larger DeFi ecosystem, which will open up the doors to additional revenue outside individual trades between zAssets on the Horizon Protocol Exchange.
