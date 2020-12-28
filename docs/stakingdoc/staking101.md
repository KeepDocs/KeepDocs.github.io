# Staking on Keep 101

**Staking on Keep is a rewarding yet active job**


<p align="center">
  <img width="619" alt="Image by TopCrypto on Discord" src="https://user-images.githubusercontent.com/73607532/103183516-bd667b80-4891-11eb-9001-af77af1bd589.png">
</p>


## Start
**As outlined at the very beginning you would need 3 things to start :**
- Run a node (by yourself or with a staking provider).
- 70k KEEP token for staking (which will be lower over [time](https://staking.keep.network/about-staking/staking-economics#how-to-get-keep)).
- any amount of ETH for bonding.


**Down the road, soon to be announced, there will be :**
- Eth-only staking, no need for KEEP tokens minimum stack.
- Pooled staking, so you can stake with less tokens than the minimum amount.
- Custodial staking, so you can stake and forget.

## Active job
Staking on Keep is an active job, since there are a few things you just need to watch out permanently:

- Collateralization ratio on every deposit your node is bonding
   - [Allthekeeps.com](https://allthekeeps.com/), [Keepscan.com](https://keepscan.com/), [Keep-Explorer.info](https://keep-explorer.info/) sites and [Peeker Bot](https://t.me/keep_peeker_bot) Telegram Bot are essential tools for this.
- Node health to avoid any slashing
   - have monitoring and backups in place, or have a provider taken care of this.
- Collecting rewards
   - Rewards, fees, stakes, all are handled from the [dashboard.keep.network](https://dashboard.keep.network/overview), detailed explanations [here](https://staking.keep.network/token-dashboard/delegate-stake).

## Rewards
- Rewards for stakers are paid weekly.
- Current rewards mechanism is based on capital added as a stake (KEEP) and as a bond (ETH). **More is better.**
- Rewards will last another 20 months while fees to users stay low.
- The model is explained on the blogpost and detailed thoroughly in the official documentation:
   - Matt's blogpost :[A new rewards mechanism - 
or, How to make 200% APY on your ETH](https://blog.keep.network/a-new-rewards-mechanism-deef3412c3e1)
   - Official Documentation: [Staking Rewards](https://staking.keep.network/about-staking/staking-economics)
- Play with different rewards scenarios on [AllTheKeeps/Stakedrop](https://allthekeeps.com/stakedrop)
 
 <p align="center">
  <img width="500" src="https://user-images.githubusercontent.com/73607532/103181539-c3a02c00-4880-11eb-818c-50db877841ac.png">
</p>

   


## Risks
If you manage your stake and node in a thorough and responsible way nothing should happen, but be aware that :
- You could get liquidated :
   - if any of the deposits gets undercollateralized, the ETH bonded are seized in order to preserve TBTC's value.
   - if this happens you should redeem your deposit inmediately (details below).
- You could get slashed :
   - if you or your node doesn't behave properly, your KEEP staked could be seized partially or totally.
- More overview on our site's [risks section](Node-Operation/risks) 
- Details on the following documentation :
  - **Official :** [Staking Risks](https://staking.keep.network/about-staking/staking-risks)
  - **Ssh's :** [Keep Nodes Risks - Liquidation and Slashing Details](https://hackmd.io/@protocollayer/BkUBl7zIw)
  - **State's :** [Keep stakedrop risks and mitigation strategies](https://hackmd.io/@LayerState/KeepStakedropRisks)
  - **KFerret's :** [ECDSA Node Risks & Mitigation Strategies on his KeepTools.org](https://keeptools.org/staking/ecdsa-risks)


## Run a node
### By yourself: 
The **Node Operation Section** includes links to support documentation in order to :

- [Deploy your Nodes](Node-Operation/deploy.md)
- [Manage your Nodes](Node-Operation/manage.md)
- [Troubleshooting](Node-Operation/troubleshooting.md)
- [Monitoring and Remote Alerting](Node-Operation/monitoring.md)
- [Risk Mitigation](Node-Operation/risks.md)

For further support, join [Discord](https://discord.gg/Dkhc5t8XXD) and see Keep Network's GitHub documentation.

### Staking with a Provider
A staking provider can take over and manage for you the Node operation work. 

Some of the providers are :
- Figment Networks, Yannik Folla (yannick@figment.network) 
- Staked, Tim Ogilvie (togilvie@staked.us)
- Bison Trails, Viktor Bunin (viktor@bisontrails.co)
- Blockdaemon, Konstantin Richter (konstantin@blockdaemon.com)
- Low Fee Validation, Eduardo Agut **(Bonsfi in Discord)**, is the newest alternative, providing high value and fast answers to users.

## How to Redeem TBTC for BTC
- Official Guide for using the [dapp.tbtc.network](https://dapp.tbtc.network/) you can find it [here](https://tbtc.network/developers/how-to-use-the-tbtc-dapp/).
- It's worh mentioning that this process involves several steps, which should be done one by one with only one browser tab open since it can be buggy.
- Please use as reference Agoristen's steps explanation and url detail:

   1. https://dapp.tbtc.network/deposit/YOUR_ADDRESS/redeem    Enter BTC address and submit -> redirects
   2. https://dapp.tbtc.network/deposit/YOUR_ADDRESS/redemption    2 TXN: A) Approval B) Redemption -> redirects
   3. https://dapp.tbtc.network/deposit/YOUR_ADDRESS/redemption/signing    1 TXN -> redirects
   4. https://dapp.tbtc.network/deposit/YOUR_ADDRESS/redemption/confirming    Wait until 6 confirmations -> redirects
   5. https://dapp.tbtc.network/deposit/YOUR_ADDRESS/redemption/prove    Submit withdraw proof

And at step 2 you need to complete it in full with no other dapp related tabs open, otherwise it will fail. After redirect to 3. you can directly access the URL and likely use multiple tabs.

---
<p style="text-align: left; width:49%; display: inline-block;"><a href="/#/comparison/comparesimilar">Previous</a></p>
<p style="text-align: right; width:50%;  display: inline-block;"><a href="/#/Node-Operation/intro-operation">Next</a></p>

---

`Contributors: Ramaruro, EstebanK  -  Image by TopCrypto on Discord`
