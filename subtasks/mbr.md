---
layout: page
title: 'Minimum Bayes Risk Subtask'
---

* [Home](../index.md)

Minimum Bayes Risk (MBR) decoding is an alternative decoding strategy for NMT models that has been shown to outperform beam search. [Freitag et al., 2021](https://arxiv.org/pdf/2111.09388.pdf)
MBR decoding relies on two essential components: a machine translation model and a utility metric. Automatic MT metrics play a crucial role in MBR decoding as they are the typical choice for the utility metric.

In this subtask, we want the participants to only focus on the utility function. We provide candidates lists (generated via ancestral sampling) from an English-German WMT NMT model. 
Based on the candidate list, we generate a score tsv file that contains all pairs of sentences that need to be scored for MBR decoding. Participants are asked to only submit the scored files so that we can
run MBR decoding on our side. 

We will then run a MQM human evaluation comparing the different MBR outputs with each other to evaluate which metric is most suitable for MBR deoding. 


## Important Dates:

|  | Date |
| ----------- | :-----------: |
| Release of candidate Lists for development | TBA |
| Release of candidate Lists for newstest2022 | TBA |
| Paper submission deadline to WMT | TBA |
| WMT Notification of acceptance | TBA |
| WMT Camera-ready deadline | TBA |
| Conference | TBA |




