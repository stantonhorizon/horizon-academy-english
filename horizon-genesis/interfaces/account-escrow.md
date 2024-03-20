---
description: Tracking your escrowed HZN.
---

# Account - Escrow

{% hint style="danger" %}
This version of Horizon Academy has been deprecated! To find the latest version, please visit: [English V2](https://academy.horizonprotocol.com/)
{% endhint %}

In Account > Escrow, you will find the Escrow tab.

The Escrow Tab tracks your escrowed HZN, which is awarded to a user who is Staking.

### **What is Escrowed HZN**

Every time you "Claim" when staking, the HZN rewards from that Claim gets allocated to Escrowed HZN. All Escrowed HZN is vested for 1 year from the claim date to prevent rewards from being immediately sold.

1 year later after the vesting period, Escrowed HZN can then be unlocked

Please note that unlocking requires a transaction on the blockchain. There are no time requirements as to when the unlock happens. A user can unlock it once a week or let it accumulate and unlock it once a year with no penalty either way.

### **What can you do with Escrowed HZN**

Escrowed HZN is considered HZN from your wallet. It can be used to manage your C-Ratio and mint zUSD.

Please note that Escrowed HZN takes priority when unstaking. Therefore, to be able to sell HZN, you need to unstake all of your Escrowed HZN first before your unlocked HZN becomes available.

### **Interface**

The Escrow Tab interface includes the following:

* **Available to Unlock** The accumulated amount of escrowed HZN that is available for unlocking
* **Total Escrowed** The total accumulated amount of escrowed HZN in the history of this wallet.
* **Total Unlocked** The total accumulated amount of escrowed HZN that has already been unlocked in the history of this wallet.
* **Claim Date (UTC)** In the table, the Claim Date is the time at which this amount of HZN was claimed. This is the time that the 1-year escrow begins. All historical Claim Dates will remain in the table even after Unlocking.
* **Unlock Date** In the table, the Unlock Date is the date when the escrowed HZN can be unlocked.
* **Amount** In the table, the Amount is the amount of Escrowed HZN that was claimed and will be unlocked. On the Unlock Date, this Amount will be added to "Available to Unlock".

Note that there is no "Locked Escrowed HZN" number, which can be derived by subtracting "Available to Unlock" and "Total Unlocked" from "Total Escrowed". This number is the equivalent to the Total Amount of all locked Escrowed HZN shown in the table.
