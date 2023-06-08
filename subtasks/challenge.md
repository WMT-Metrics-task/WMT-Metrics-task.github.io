---
layout: page
title: 'Challenge Sets Subtask'
---

* [Home](../index.md)

Every year the Metrics shared task has been pushing for better automatic MT metrics and in the last few years we have seen great progress with metrics achieving much higher correlations with human judgements [(Mathur et al., 2020;](https://aclanthology.org/2020.wmt-1.77/) [Freitag et al., 2021;](https://aclanthology.org/2021.wmt-1.73/) [Freitag et al., 2022)](https://aclanthology.org/2022.wmt-1.2/). Yet, while the limitations of metrics such as BLEU are well known in the MT comunity, we still do not know which limitations new metrics (specially neural ones) might have. For this reason we created this subtask.

Inspired by the [Build it, Break it: The Language Edition](https://bibinlp.umiacs.umd.edu/sharedtask.html) we created a subtask where participants (_breakers_) are asked to build challenging examples that target specific phenomena currently not addresses by current. On top of that we also encourage paper submissions on Metrics analysis.

Examples of challenge sets developed to test metrics in 2022:
- [DEMETR: Diagnosing Evaluation Metrics for Translation](https://aclanthology.org/2022.emnlp-main.649.pdf)
- [ACES: Translation Accuracy Challenge Sets for Evaluating Machine Translation Metrics](https://www.statmt.org/wmt22/pdf/2022.wmt-1.44.pdf)

Please check the [proceedings from WMT 2022](https://www.statmt.org/wmt22/papers.html#:~:text=pp.%C2%A0458%E2%80%91468-,Metrics%20Task%20Papers,-Robust%20MT%20Evaluation) to find all submissions to the 2022 edition!

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

For all challenge sets we will report pairwise accuracy meaning, how many times a metric assigns a better score to the `good-translation` compared to the score assigned to the `incorrect-translation`.

## Important Dates:

|  | Date |
| ----------- | :-----------: |
| *Breaking Round* submission deadline | **20th July, 2022 ❗** |
| *Scoring Round* | **17th August, 2022** |
| Scored challenge sets given to participants for analysis | **24th August, 2022** |
| Paper submission deadline to WMT | 5th September, 2022 |
| WMT Notification of acceptance | 6th October, 2022 |
| WMT Camera-ready deadline | 18th October, 2022 |
| Conference | 6th - 7th December, 2022 |