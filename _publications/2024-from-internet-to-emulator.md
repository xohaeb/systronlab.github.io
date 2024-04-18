---
layout: publication
title: "From Internet to Emulator: A Virtual Testbed for Internet Routing Protocols"
date: 2024-04-18 12:00:00 +0000
authors:
- Joshua Levett
- Poonam Yadav
- Vassilios Vassilakis
venue: "UK Systems Workshop 2024"
file: "/files/publications/2024-abstract-from-internet-to-emulator.pdf"
preprint: true
---

The ongoing evolution and expansion of the Internet demands resilient, secure and scalable routing protocols to provide seamless connectivity across global networks. However, the lack of a realistic testbed for the development and analysis of new internetwork routing protocols or extensions at an Internet scale leads to unpredictability in real-world performance prior to implementation. Whilst existing simulation and emulation approaches provide some insight, such as by replicating a routing environment at a smaller scale, or using a lab-generated topology, these do not capture existing architectural challenges or usage and therefore deployment challenges may not be fully addressed, and performance improvement is likely to be artificially optimistic.

We propose an emulation approach based on real-world Internet topology captures and the replay of routing changes, to provide a more comprehensive testbed for new routing protocols. Our underlying hypothesis is that capturing Internet topology and automating Internet emulation by replicating each topological node using an emulated border router, can enable researchers to gleam greater insight into the performance of Internet protocols. This is particularly important for problems of protocol adoption, where our approach may enable real-world understanding of critical adoption thresholds, or in measuring relative resource requirements - such as for energy or relative change in carbon emission - by capturing resource usage metrics from each emulated device.
By taking an emulation approach utilising a combination of Python-based software and Apptainer/Singularity container virtualisation, we hope to provide the flexibility to deploy representative Internet emulation environments in both public cloud and research HPC contexts. The current state of the project is seeking feedback on early conceptual results, but later we hope to undertake routing protocol research at a wider scale, providing evidence-based benefit and adoption statistics.

In conclusion, we endeavour to contribute to the development of Internet scale routing protocols by providing a more realistic and representative emulated testing environment compatible with research HPC. Our proposed approach enables the collection of deployment data representative of real-world routing demands, providing evidence-based statistics and the capture of critical adoption thresholds.