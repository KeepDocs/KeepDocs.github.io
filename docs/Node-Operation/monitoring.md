# Monitoring and Remote Alerting

This section covers the following topics related to the Nodes Automated Monitoring, Remote Alerting and Early Warning Methods.


## Guides for Setting up Node Monitoring of Keep Nodes
### Random Beacon Monitoring using Grafana, Prometheus, Prometheus Node Exporter, Google cAdvisor and Loki
- MutedTommy's [Keep Random Beacon | Node Monitoring | Part 1](https://medium.com/@hr12rtk/keep-random-beacon-node-monitoring-grafana-prometheus-and-loki-4a4b669b31ea) and [Part 2](https://medium.com/@hr12rtk/keep-random-beacon-node-monitoring-part-2-5cd037464a6e).
This article summarises the steps used to set up the monitoring on Keep Random Beacon node using Grafana, Prometheus, Prometheus Node Exporter, Google cAdvisor and Loki.

<p align="center">
  <img width="600" src="https://user-images.githubusercontent.com/68167410/89043879-c537e900-d30e-11ea-84ad-dfbd47592d2f.png">
</p>


### Random Beacon and ECDSA Nodes Monitoring using Elasticsearch, Logstash, and Kibana
- Guide to [Setting up an Elastic Stack Dashboard](https://www.notion.so/Setting-up-Elastic-Stack-Dashboard-14f9edc94418468bb95af40417a0332a) for Keep Random Beacon and ECDSA Nodes using Elasticsearch, Logstash, and Kibana

>The Elastic Stack — formerly known as the ELK Stack — is a collection of open-source software produced by Elastic which allows you to search, analyze, and visualize logs generated from any source in any format, a practice known as centralized logging. Centralized logging can be very useful when attempting to identify problems with your servers or applications, as it allows you to search through all of your logs in a single place. It’s also useful because it allows you to identify issues that span multiple servers by correlating their logs during a specific time frame.
>
>The [Elastic Stack](https://www.digitalocean.com/community/tutorials/how-to-install-elasticsearch-logstash-and-kibana-elastic-stack-on-ubuntu-18-04#step-4-%E2%80%94-installing-and-configuring-filebeat) has four main components:
>
> Elasticsearch: a distributed RESTful search engine which stores all of the collected data.
>
> Logstash: the data processing component of the Elastic Stack which sends incoming data to Elasticsearch.
>
> Kibana: a web interface for searching and visualizing logs.
>
> Beats: lightweight, single-purpose data shippers that can send data from hundreds or thousands of machines to either Logstash or Elasticsearch.
>
<p align="center">
  <img width="600" src="https://user-images.githubusercontent.com/68167410/89001980-816ac280-d2c1-11ea-98f2-94e0481188fc.png">
</p>


### Kubernetes Monitoring with Prometheus & Grafana
- **Tabert's** video that will help you set up monitoring using the Kubernetes cluster 
- https://www.youtube.com/watch?v=71oa9EKG-Cc

<p align="center">
  <img width="600" src="https://user-images.githubusercontent.com/73607532/102139810-20412700-3e3d-11eb-8080-e62508df2cb5.png">
</p>

---

<p style="text-align: left; width:49%; display: inline-block;"><a href="/#/Node-Operation/troubleshooting">Previous</a></p>
<p style="text-align: right; width:50%;  display: inline-block;"><a href="/#/Node-Operation/risks">Next</a></p>


---
`Written & assembled by Keep Community.`
`Contributors: Ramaruro, EstebanK`
