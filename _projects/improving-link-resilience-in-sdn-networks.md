---
layout: projects
title: "Improving Link Resilience in SDN Networks"
date: 2024-04-29 12:00:00 +0000
authors:
- Rehab Alawadh
- Hamed Ahmadi
- Poonam Yadav
image: '/img/projects/improving-link-resilience-in-sdn-networks.png'
desc: Improving fast failure-recovery models in software-defined networks.
---

Deploying new optimized routing policies on routers in the event of link failure is difficult due to strong coupling between the data and control planes and the absence of topology information about the network. Because of the distributed architecture of traditional Internet protocol networks, policies and routing rules are spread in a decentralized way, resulting in looping and congestion problems. Software-defined networking (SDN) enables centralized network programmability. As a result, data plane devices just focus on packet forwarding, leaving the control plane’s complexities to be managed by the controller. Thus, the controller installs the policies and rules centrally. Considering the controller’s knowledge of the global network architecture, central control enhances the flexibility of link failure identification and restoration. Therefore, this project focuses on the importance of harden networks resilience to link failure by introducing a hybrid intelligent fast failure recovery framework using SDN architecture.

## Objectives

Development of Pre-Failure Detection Mechanisms: Leverage GNN to analyze the simulated network's topology and predict potential failures. This process incorporates Exploratory Data Analysis (EDA) to assess the impact of variables like throughput, latency, and packet loss, enhancing early vulnerability identification through continuous monitoring and dynamic network health analysis. Implementation of Post-Failure Management Protocols: Integrate failure detection and recovery protocols such as Border Gateway Protocol (BGP) routing protocol, Link Layer Discovery Protocol (LLDP) and Bidirectional Forwarding Detection, integrated with GNN within the simulated environment. This will test the system’s ability to manage failures efficiently, minimizing disruption.

## System architecture with pre-failure detection

The System Architecture is designed to provide a resilient and robust network infrastructure capable of anticipating potential failures through advanced detection techniques.

1. Topology discovery is utilized to gather and update diverse networking information from switches and routers in real-time.
2. transmission requests are forwarded to the efficient routing generator for optimal paths calculation and decision-making.
3. Graph Neural Networks (GNN) are used by the system to improve the prediction of potential connection failures at the stage preceding any failure.
4. The decision creator then transmits the new configurations to the network switches and routers using a flow table.

By continuously monitoring and analyzing the network graph, the GNN can predict possible connection failures, enabling proactive actions to reduce risks.

## System architecture with post-failure management

In response to link failures, a new optimal path is selected from a precomputed list of paths to reduce the load on the SDN controller and enhance the speed of calculations to minimize latency. Flows are intelligently classified based on their frequency of use. Backup paths are then stored accordingly, either in the controller's hash table or the switch's flow table, depending on this classification. This approach aims to optimize overall network management, enhancing efficiency and resilience in the network system.

## Publications

- [(Preprint) HIFFR: Hybrid Intelligent Fast Failure Recovery Framework for Enhanced Resilience in Software Defined Networks](https://eprints.whiterose.ac.uk/212995/)