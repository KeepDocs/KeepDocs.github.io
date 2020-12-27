# Staking on Keep 101

Staking on Keep is an rewarding yet active job. 

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
- Collecting rewards
- Collateralization ratio on every deposit your node is bonding
- Node health to avoid any slashing

## Rewards
- Rewards for stakers are paid weekly.
- Current rewards mechanism is based on capital added as a stake (KEEP) and as a bond (ETH). **More is better.**
- Rewards will last another 20 months while fees to users stay low.
- The model is explained on the blogpost and detailed thoroughly in the official documentation:
   - Matt's blogpost :[A new rewards mechanism - 
or, How to make 200% APY on your ETH](https://blog.keep.network/a-new-rewards-mechanism-deef3412c3e1)
   - Official Documentation: [Staking Rewards](https://staking.keep.network/about-staking/staking-economics)
   - Rewards, fees, stakes, all is handled from the [dashboard.keep.network](https://dashboard.keep.network/overview), detailed explanations [here](https://staking.keep.network/token-dashboard/delegate-stake).


## Risks
- If you manage your stake and node in a thorough and responsible way nothing should happen, but be aware that :
- You could get liquidated :
   - if any of the deposits gets undercollateralized, the ETH bonded are seized in order to preserve TBTC's value.
- You could get slashed :
   - if you or your node doesn't behave properly, your KEEP staked could be seized partially or totally.
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

---
<p style="text-align: left; width:49%; display: inline-block;"><a href="/#/comparison/comparesimilar">Previous</a></p>
<p style="text-align: right; width:50%;  display: inline-block;"><a href="/#/Node-Operation/intro-operation">Next</a></p>

---

`Contributors: Ramaruro, EstebanK`
