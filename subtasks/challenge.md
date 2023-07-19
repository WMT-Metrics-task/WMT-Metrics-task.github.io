---
layout: page
title: 'Challenge Sets Subtask'
---

* [Home](../index.md)

Every year the Metrics shared task has been pushing for better automatic MT metrics and in the last few years we have seen great progress with metrics achieving much higher correlations with human judgements [(Mathur et al., 2020;](https://aclanthology.org/2020.wmt-1.77/) [Freitag et al., 2021;](https://aclanthology.org/2021.wmt-1.73/) [Freitag et al., 2022)](https://aclanthology.org/2022.wmt-1.2/). Yet, while the limitations of metrics such as BLEU are well known in the MT comunity, we still do not know the limitations that new metrics (specially neural ones) might have. For this reason we created the metric challenge sets subtask.

Inspired by the [Build it, Break it: The Language Edition](https://bibinlp.umiacs.umd.edu/sharedtask.html),  participants in the challenge sets subtask (_breakers_) are asked to build challenging examples that target specific phenomena currently not addressed by MT reference-based or reference-less evaluation metrics. On top of that we also encourage paper submissions on metrics analysis.

Examples of challenge sets developed to test metrics in 2022:
- [DEMETR: Diagnosing Evaluation Metrics for Translation](https://aclanthology.org/2022.emnlp-main.649.pdf)
- [ACES: Translation Accuracy Challenge Sets for Evaluating Machine Translation Metrics](https://www.statmt.org/wmt22/pdf/2022.wmt-1.44.pdf)

Please check the [Proceedings of WMT 2022](https://www.statmt.org/wmt22/papers.html#:~:text=pp.%C2%A0458%E2%80%91468-,Metrics%20Task%20Papers,-Robust%20MT%20Evaluation) to find all the submissions to the challenge sets subtask!

This shared task will have the two following rounds:

**1) Breaking Round:**  Challenge set participants (Breakers) create challenging examples for metrics. They must send the resulting "challenge sets" to the organizers.
 
**2) Scoring Round:** The challenge sets created by Breakers will be randomized and sent to all Metrics participants (Builders) to score. Also, the organizers will score all the data with baseline metrics such as BLEU, chrF, BERTScore, COMET, BLEURT, Prism and YiSi-1.

**3) Analysis Round:** Breakers will receive their data with all the metrics scores for analysis.

## Registration

Please register your submission with contacts and a short description [here](https://forms.office.com/e/uhA74RnjMb). 

## Submission format

We expect submissions in a tab-separated values (TSV) with the following format:

| translation-direction | source | good-translation | incorrect-translation | reference | phenomena | 
| :--: | :----: | :--------------: | :-------------------: | :-------: | :--: |
| de-en | Das Shampoo hilft gegen Schuppen. | The shampoo helps against dandruff. |  The shampoo helps against flakes. | The shampoo helps fight dandruff. | lexical-ambiguity |

where the `translation-direction` column contains the translation direction of the entry, the `source` column contains the original segment, `good-translation` column contains a correct translation for the phenomena (in the above case is a lexical ambiguity), `incorrect-translation` an example of a translation that is not correct according to a specific phenomena and a `reference` column with (ideally) human translations, `phenomena` is an identifier that identifies the phenomena being tested.

Further details about formating the segments will be updated later. 

## Submission link

Please submit your challenge set(s) [here](https://cloud.dfki.de/owncloud/index.php/s/sRnY89FbZpSPCjJ), after having completed the registration above. 

For naming every chanllenge set file, please choose a short name for your challenge set and name your file in the form "shortname.tsv".
It is also possible to submit a compressed file/archive. 

## Important Dates:

|  | Date |
| ----------- | :-----------: |
| *Breaking Round* registration & submission deadline | **20th July, 2023 ❗** |
| *Scoring Round* begins | 10th August, 2023 |
| *Scoring Round* submission deadline | 17th August, 2023 |
| *Analysis Round* begins | 24th August, 2023 |
| Paper submission deadline to WMT | **5th September, 2023** |
| WMT Notification of acceptance | 6th October, 2023 |
| WMT Camera-ready deadline | 18th October, 2023 |
| Conference | 6th - 7th December, 2023 |
