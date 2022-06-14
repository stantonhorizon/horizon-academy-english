# Oracles

Oracles are data sources or data feeds that are designed to be fed into a smart contract. Oracles are typically third-party services that allows a blockchain to connect with and receive external data from outside of their ecosystem.

Most common use case for oracles involves the access of real-time data, most often in the form of real-time price feeds of different assets.

Oracles give the crypto and defi ecosystem a method to connect blockchain ecosystems between each other and to the real world as well, while providing security features to ensure data confidentiality.

## Why Horizon Protocol Use Oracles

![](../../.gitbook/assets/Oracles)

Oracles are a critical part to Horizon Protocol and are necessary because oracles are responsible for providing the price feeds that determine the prices of assets listed in the Horizon Exchange.

![](../../.gitbook/assets/Oracle\_Horizon\_x\_Chainlink)

Different oracle providers such as [@chainlink](https://twitter.com/chainlink) and [@Phoenix\_Chain](https://twitter.com/Phoenix\_Chain) represent unlimited access to any type of asset and enforce the security and safety of the price feeds to:&#x20;

* crypto&#x20;
* stocks&#x20;
* indices
* commodities
* NFTs
* and more!

## Oracle Refresh Rate

Horizon Protocol Synthetic Assets (zAssets) need regular on-chain price feeds to update their price shown on the Horizon Exchange.

It is important to note that each refresh of a price requires a payment to the oracle providing the price, making constant price checks financially unfeasible. To solve this, oracles used by Horizon Protocol refresh prices based on two variables:

* _Heartbeat_ — a predetermined time period (e.g. every 4 hours)
* _Variance_ — a predetermined price threshold (e.g. 0.2% change in price)

Should either of these variables return true, the oracle will refresh the price.

The Heartbeat and Variance is potentially different for each zAsset. Learn more about this in [Exchange Fees](exchange-fees.md#fbee). And check out [Chainlink Docs](https://docs.chain.link/docs/bnb-chain-addresses/) for Heartbeat and Variance for each oracle data feed that we use (click into a particular data feed to see the specifics).
