# Exchange FAQ

{% hint style="danger" %}
This version of Horizon Academy has been deprecated! To find the latest version, please visit: [English V2](https://academy.horizonprotocol.com/)
{% endhint %}

<details>

<summary><strong>Where can I submit a bug/suggestion report?</strong></summary>

For now, please go to our [Telegram](https://t.me/HorizonProtocol) to report bugs or suggestions.

In the near future, we will have a form for submitting bugs and feedback with the following template so that we can address the issue as fast as possible:

1. Step by step description on how to reproduce the bug/issue
2. Relevant pictures

</details>

<details>

<summary><strong>How often are the prices updated?</strong></summary>

Each zAsset has two variables that will trigger a price refresh. A variable based on a period of time (e.g. every 1 hour) called a **heartbeat**. Another variable based on price variance (e.g. 0.2%) called **variance**. If either of these conditions are met, the oracle will update the price feed.

These price updates cost money for the oracle and oracles base their heartbeats and variance values based on general usage. This means that more sensitive variables justify a cost increase. This also highlights a tradeoff in decentralized exchanges (DEXs) and centralized exchanges (CEXs). The loss of speed is made up by decentralization, transparency, and ownership of your own assets. This makes a CEX more desirable for high frequency traders but a DEX far more beneficial to a mid to long term trader/investor.

</details>

<details>

<summary><strong>Why is there fee differences between zAssets? For example: zDOGE shows 0.25%, zAPPL shows 0.50%.</strong></summary>

Every zAsset has its own oracle price feed and therefore a corresponding heartbeat and price variance threshold. If a zAsset has a price variance threshold of 0.50%, the exchange fee on Horizon Exchange will also be 0.50% in order to disincentivize users from using the variance threshold to front-run the oracle’s price.

</details>
