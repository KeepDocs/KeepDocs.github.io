# Risk Mitigation for Node Operators

Operating Keep Nodes imply risks, as there are Collateralization and Availability requirements that must be met to avoid being penalized.
This section covers topics related to understanding and mitigating the risks of operating a Keep Poduction System.


## Main Risks for Operating Keep Nodes
From the currrent understanding and Operation of the Keep System, we can see two main risks for the Operator to lose a portion or all of the funds staked to support the tBTC Bridge:
* Undercollateralization and Liquidation
* Node Downtime

The current understanding indicates that the Undercollateralization is a more frequent problem than the Node Downtime. Uptime for Nodes in Testnet is high and other than upgrades to the software or issue with the VPS provider, it doesn't seem a high risk to the operation. It can also be mitigated with a redundant node installation managed with Kubernets (see below). If technical operation is not your thing, you could always talk to [staking providers](https://keepdocs.github.io/#/stakingdoc/stakingoptions?id=staking-with-a-provider) who can take care of this.
However, Undercollateralization seems a bigger problem as it is less controllable and there is no automated way to protect this situation yet other than manual intervention.

?> These risks are well explained on these three reports written by community members Ssh, Kferret and State. You can find them on the [Community Tools-Risks section](https://keepdocs.github.io/#/basics/tools?id=node-running-risks).

This graph from the Ssh's document explains the risks well.
<p align="center">
  <img width="800" src="https://user-images.githubusercontent.com/68167410/88967178-0975ab80-d273-11ea-9696-15f2ce8995c5.png">
</p>




## Undercollateralization Prevention
There is a serious risk that due to relative price fluctuations of the ETH / BTC pair, your collateral (actually, the collateral of the Keep(s) that you have signed) is not sufficient and you run the risk of Liquidation.
The process is detailed in the [tBTC System Design Document](https://docs.keep.network/tbtc/index.pdf), pages 19-20


This article from Bison Trail, [Keep Active Management](https://bisontrails.co/keep-active-participation/), explains this Liquidation Process and lists several measures that can be taken to avoid this issue.


!> Alerts need to be enabled to monitor this relation to then manually take action to close deposits and avoid liquidation. Community developed tools like [All The Keeps site](https://keepdocs.github.io/#/basics/tools?id=all-the-keeps) and [Peeker TG Bot](https://keepdocs.github.io/#/basics/tools?id=peeker-tg-bot) help you monitor open deposits on your nodes.


!> And have always TBTC available to be able to close your deposits when needed.

> Keep Team expressed additional automation features for collateral Eth increase or deposit redemption when needed for v2 of Keep Dashboard. We expect these will help manage better these risks.


## High Availability
### General Considerations from the Keep Team
The Keep Team wrote a detailed document that addresses many aspects of running a [Keep ECDSA Node](https://github.com/keep-network/keep-ecdsa/blob/master/docs/run-keep-ecdsa.adoc#run-ecdsa-keep) with high availability

>The Keep Network expects certain capabilites for each node running on the network. To help attain these capabilities consider the following criteria:
>
>* It is paramount that Keep nodes remain available to the Keep Network. We strongly encourage a stable and redundant internet connection.
>
>* A connection to a production grade self-hosted or third party Ethereum node deployment.
>
>* Persistent and redundant storage that will survive a VM or container rotation, and disk failure.
>
>* Each Keep ECDSA client running on the network requires a unique Ethereum operator account.
>
>* Each Keep ECDSA client running on the network requires a unique IP address or a unique application port running under the same IP.



### Kubernetes Based Deployment
To ensure High Availability of a Keep Production System by introducing Node Redundancy, a [Kubernetes](https://kubernetes.io/) based deployment is recommended. 
Refer to the [Kubernetes Deployment Section](https://github.com/Estebank97/Keep-Node-Operation/wiki/Deploy-your-Node#kubernetes-installation-guide-for-ecdsa-nodeode) for installation instructions. 

This detailed document from the Keep Team provides a lot of information about the ECDSA Node  [Run ECDSA Keep](https://github.com/keep-network/keep-ecdsa/blob/master/docs/run-keep-ecdsa.adoc#5-deployment-consideration)

---

<p style="text-align: left; width:49%; display: inline-block;"><a href="/#/Node-Operation/monitoring">Previous</a></p>
<p style="text-align: right; width:50%;  display: inline-block;"><a href="/#/Node-Operation/links">Next</a></p>


---
`Written & assembled by Keep Community.`
`Contributors: Ramaruro, EstebanK`
