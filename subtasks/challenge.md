---
layout: page
title: 'Challenge Sets Subtask'
---

* [Home](../index.md)

Every year the Metrics shared task has been pushing for better automatic MT metrics and in the last few years we have seen great progress with metrics achieving much higher correlations with human judgements [(Mathur et al., 2020;](https://aclanthology.org/2020.wmt-1.77/) [Freitag et al., 2021)](https://aclanthology.org/2021.wmt-1.73/). Yet, while the limitations of metrics such as BLEU are well known in the MT comunity, we still do not know which limitations new metrics (specially neural ones) might have. For this reason we created this subtask!

Inspired by the [Build it, Break it: The Language Edition](https://bibinlp.umiacs.umd.edu/sharedtask.html) we created a subtask where participants (_breakers_) are asked to build challenging examples that target specific phenomena currently not addresses by current. On top of that we also encourage paper submissions on Metrics analysis.

Analysis papers for inspiration: 
- [A Fine-Grained Analysis of BERTScore](https://aclanthology.org/2021.wmt-1.59/)
- [Identifying Weaknesses in Machine Translation Metrics Through Minimum Bayes Risk Decoding: A Case Study for COMET](https://arxiv.org/abs/2202.05148)

This shared task will have the two following rounds:

**1) Breaking Round:**  Participants (Breakers) create challenging examples for metrics. They must send the resulting "challenge sets" to the organizers.
 
**2) Scoring Round:** The challenge sets created by Breakers will be sent to all Metrics participants/Builders to score. Also, the organizers will score all the data with baseline metrics such as BLEU, chrF, BERTScore, COMET, BLEURT, Prism and YiSi-1.

**3) Analysis Round:** Breakers will receive their data with all the metrics scores for analysis.


## Challenge Set Structure:

We expect submissions in a tab-separated values (TSV) with the following format:

### Format:

| source | good-translation | incorrect-translation | reference | phenomena | 
| :----: | :--------------: | :-------------------: | :-------: | :--: |
| Das Shampoo hilft gegen Schuppen. | The shampoo helps against dandruff. |  The shampoo helps against flakes. | The shampoo helps fight dandruff. | lexical-ambiguity |

where the `source` column contains the original segment, `good-translation` column contains a correct translation for the phenomena (in the above case is a lexical ambiguity), `incorrect-translation` an example of a translation that is not correct according to a specific phenomena and a `reference` column with (ideally) human translations, `phenomena` is an identifier that identifies the phenomena being tested.

For all challenge sets we will report kendall tau-like similar to what we have done in [WMT 2021](https://aclanthology.org/2021.wmt-1.73/). This formula measures how many times a given metric scores the `good-translation` above the `incorrect-translation` and it is defined as follows:

<p align="center">
    <img src="/public/css/kendall-tau.png" alt="Kendall Tau-like Formula" style="height: 75px;"/>
</p>

### Data/Resources:

In this shared task we accept any data as long as it respects the format described above! 

With that said, if you are planing to follow an automated approach similar to our approach last year, you will need access to corpora with 2 reference translations. Here are some resource ideas:

- [WMT16 QE data](https://lindat.mff.cuni.cz/repository/xmlui/handle/11372/LRT-1646) 
- [APE-QUEST](https://ape-quest.eu/downloads/)

Both corpora have Source, PE and MT. You can apply different pertubations to the PE and compare the perturbed PE version against the original PE using the reference translation. 

Another possibility is to use recent testsets from WMT where you have 2 or more references (e.g: [WMT21 En-De had 4 references](https://github.com/WMT-Metrics-task/wmt21-metrics/tree/main/newstest2021_submissions/ende)). But note that, some metrics participating this year, might include that data into training and validation.

## Important Dates:

|  | Date |
| ----------- | :-----------: |
| *Breaking Round* task announcement | 21th March, 2022 |
| *Breaking Round* submission deadline | **26th July, 2022** |
| *Scoring Round* | **25th August, 2022❗** |
| *Analysis Round* | 7th September, 2022 |
| Paper submission deadline to WMT | 7th September, 2022 |
| WMT Notification of acceptance | 9th October, 2022 |
| WMT Camera-ready deadline | 16th October, 2022 |
| Conference | 7th - 8th December, 2022 |
