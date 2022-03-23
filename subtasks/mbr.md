---
layout: page
title: 'Minimum Bayes Risk Subtask'
---

* [Home](../index.md)

Minimum Bayes Risk (MBR) decoding is an alternative decoding strategy for NMT models that has been shown to outperform beam search ([Freitag et al., 2021](https://arxiv.org/pdf/2111.09388.pdf)).
MBR decoding relies on two essential components: a machine translation model and a utility metric. Automatic MT metrics play a crucial role in MBR decoding as they are the typical choice for the utility metric.

In this subtask, we ask the participants to develop utility functions that can be used during MBR decoding. A utility function can be an automatic MT metric used for the general metric task, or a new
metric that has been tailored for the MBR use case. In both cases, MBR decoding is stress testing the utility function as it has to perform well for translations of very different quality.

To evaluate the quality of the utility function only, we provide candidate lists (generated via ancestral sampling) from an English-German WMT NMT model.
Based on the candidate list, we generate a score tsv file that contains all pairs of sentences that are needed to be scored for MBR decoding. Participants are asked to only submit the scored files. BAsed on the scores, we run MBR decoding on our side.

We will then run a MQM human evaluation comparing the different MBR outputs with each other to evaluate the value of each  utility function for MBR decoding.


## Important Dates:

|  | Date |
| ----------- | :-----------: |
| Release of candidate Lists for development | soon |
| Release of candidate Lists for newstest2022 | 1 week after release from WMT |
| Submission deadline | 4 weeks after release of candidate list of newstest2022 |




