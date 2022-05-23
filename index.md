---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

# Welcome to the WMT 2022 Metrics Shared Task!

<p class="message">
  This shared task will examine automatic evaluation metrics for machine translation. We will provide you with MT system outputs along with source text and the human reference translations. We are looking for automatic metric scores for translations at the system-level, and segment-level. We will calculate the system-level, and segment-level correlations of your scores with human judgements.<br /><br />

  We invite submissions of <strong>reference-free metrics</strong> in addition to <strong>reference-based metrics</strong>.<br /><br />   
  
  Have questions or suggestions? Feel free to <a href="mailto:wmt22-metric@googlegroups.com">Contact Us</a>!
</p>

## Metrics Task Important Dates

|  | Date |
| ----------- | :-----------: |
| System outputs ready to download | 9th August, 2022 |
| Submission deadline for metrics task | 16th August, 2022 |
| Paper submission deadline to WMT | 7th September, 2022 |
| WMT Notification of acceptance | 9th October, 2022 |
| WMT Camera-ready deadline | 16th October, 2022 |
| Conference | 	7th - 8th December, 2022 |

## Goals

The goals of the shared metrics task are:

- To achieve the strongest correlation with human judgement of translation quality over a diverse set of MT systems;
- To illustrate the suitability of an automatic evaluation metric as a surrogate for human evaluation;
- To test robustness of metrics when evaluating domains other than news data;
- To create high quality datasets for developing and evaluating metrics

## Task Description

We will provide you with the source sentences, output of machine translation systems and reference translations.

1. Official results: Correlation with MQM scores at the sentence and system level for the following language pairs:
   - Chinese-English
   - English-Russian
   - English-German
2. Secondary Evaluation: Correlation with official WMT Direct Assessment (DA) scores at the sentence and system level.

### Subtasks:

1. [QE as a Metric](./subtasks/qe/): In this subtask participants have to score machine translation systems without access to reference translations
2. [Challenge Sets](./subtasks/challenge/): While other participants are worried with building stronger and better metrics, participants of this subtask have to build challengesets that identify where metrics fail! 
3. [Minimum Bayes-Risk (MBR) Decoding](./subtasks/mbr/): MBR decoding typically uses metrics as utility function. We invite participants to stress test their metric when used during MBR decoding. 

## Paper Describing Your Metric
You are invited to submit a short paper (4 to 6 pages) to WMT describing your automatic evaluation metric. Information on how to submit is available here. Shared task submission description papers are non-archival, and you are not required to submit a paper if you do not want to. If you don't, we ask that you give an appropriate reference describing your metric that we can cite in the overview paper.

## Training Data

The WMT Metrics shared task takes place yearly since 2008. You may want to use data from previous editions to tune/train your metric. The following table provides links to the descriptions, the _raw_ data and the findings papers of the previous editions:

| year | MQM | DA system level |DA segment level | relative ranking | paper | .bib |
|------|:---:|:---------------:|:---------------:|:--:|:--:|:--:|
| [2021](https://www.statmt.org/wmt21/metrics-task.html) | [🔗](https://github.com/google/wmt-mqm-human-evaluation) | 🔗 | 🔗 |  | [🔗](https://statmt.org/wmt21/pdf/2021.wmt-1.73.pdf)  | [🔗](https://statmt.org/wmt21/bib/2021.wmt-1.73.bib) |
| [2020](https://www.statmt.org/wmt20/metrics-task.html) | [🔗](https://github.com/google/wmt-mqm-human-evaluation) | [🔗](https://www.statmt.org/wmt20/results.html)  | [🔗](https://www.statmt.org/wmt20/results.html)  |  | [🔗](https://statmt.org/wmt20/pdf/2020.wmt-1.77.pdf)  | [🔗](https://statmt.org/wmt20/bib/2020.wmt-1.77.bib) |
| [2019](https://www.statmt.org/wmt19/metrics-task.html) |                                                          | [🔗](https://www.statmt.org/wmt19/results.html)  | [🔗](https://www.statmt.org/wmt19/results.html)  |  | [🔗](https://statmt.org/wmt19/pdf/53/WMT02.pdf)  | [🔗](https://statmt.org/wmt19/bib/53/WMT02.bib) |
| [2018](https://www.statmt.org/wmt18/metrics-task.html) |                                                          | [🔗](https://www.statmt.org/wmt18/results.html)  | [🔗](https://www.statmt.org/wmt18/results.html)  |  | [🔗](https://statmt.org/wmt18/pdf/WMT078.pdf)  | [🔗](https://statmt.org/wmt18/bib/WMT078.bib) |
| [2017](https://www.statmt.org/wmt17/metrics-task.html) |                                                          | [🔗](https://www.statmt.org/wmt17/results.html)  | [🔗](https://www.statmt.org/wmt17/results.html)  |  | [🔗](https://statmt.org/wmt17/pdf/WMT55.pdf)  | [🔗](https://statmt.org/wmt17/bib/WMT55.bib) |
| [2016](https://www.statmt.org/wmt16/metrics-task.html) |                                                          | [🔗](https://www.statmt.org/wmt16/results.html)  | [🔗](https://www.statmt.org/wmt16/results.html)  |  | [🔗](https://statmt.org/wmt16/pdf/W16-2302.pdf)  | [🔗](https://statmt.org/wmt16/bib/W16-2302.bib) |
| [2015](https://www.statmt.org/wmt15/metrics-task.html) |  |  |  | [🔗](https://www.statmt.org/wmt15/results.html)  | [🔗](https://www.statmt.org/wmt15/pdf/WMT31.pdf)  | [🔗](https://www.statmt.org/wmt15/bib/WMT31.bib)  |
| [2014](https://www.statmt.org/wmt14/metrics-task.html) |  |  |  | [🔗](https://www.statmt.org/wmt14/results.html)  | [🔗](https://www.statmt.org/wmt14/pdf/W14-3336.pdf)  | [🔗](https://www.statmt.org/wmt14/bib/W14-3336.bib)  |
| [2013](https://www.statmt.org/wmt13/metrics-task.html) |  |  |  | [🔗](https://www.statmt.org/wmt13/results.html)  | [🔗](https://www.statmt.org/wmt13/pdf/WMT02.pdf)  | [🔗](https://www.statmt.org/wmt13/bib/WMT02.bib)  |
| [2012](https://www.statmt.org/wmt12/metrics-task.html) |  |  |  | [🔗](https://www.statmt.org/wmt12/results.html)  | [🔗](https://www.statmt.org/wmt12/pdf/WMT02.pdf)  | [🔗](https://www.statmt.org/wmt12/bib/WMT02.bib)  |
| [2011](https://www.statmt.org/wmt11/metrics-task.html) |  |  |  | [🔗](https://www.statmt.org/wmt11/results.html)  | [🔗](https://www.statmt.org/wmt11/pdf/WMT03.pdf)  | [🔗](https://www.statmt.org/wmt11/bib/WMT03.bib)  |
| [2010](https://www.statmt.org/wmt10/metrics-task.html) |  |  |  | [🔗](https://www.statmt.org/wmt10/results.html)  | [🔗](https://www.statmt.org/wmt10/pdf/WMT03.pdf)  | [🔗](https://www.statmt.org/wmt10/bib/WMT03.bib)  |
| [2009](https://www.statmt.org/wmt09/metrics-task.html) |  |  |  | [🔗](https://www.statmt.org/wmt09/results.html)  | [🔗](https://www.statmt.org/wmt09/pdf/WMT-0901.pdf)  | [🔗](https://www.statmt.org/wmt09/bib/WMT-0901.bib)  |
| [2008](https://www.statmt.org/wmt08/metrics-task.html) |  |  |  | [🔗](https://www.statmt.org/wmt08/results.html)  | [🔗](https://www.statmt.org/wmt08/pdf/WMT09.pdf)  | [🔗](https://www.statmt.org/wmt08/bib/WMT09.bib)  |


You can use any past year's data to tune your metric's free parameters if it has any for this year's submission. Additionally, you can use any past data as a test set to compare the performance of your metric against published results from past years metric participants.

Last year's data contains all of the system's translations, the source documents and human reference translations and the human judgments of the translation quality.

Also, for running the mearure metrics quality, specially new ones, we encourage you to use [mt-metrics-eval](https://github.com/google-research/mt-metrics-eval) repo developed by George Foster.


## Test Sets (Evaluation Data)
**TBA**

### Submission Format

The output of your software should produce scores for the translations either at the system-level or the segment-level (or preferably both). As of last year, we no longer include document level evaluation.

There are sample metrics (with random scores) available in the validation folder in the shared data folder.

**Output file format for system-level rankings**

The output files for system-level rankings should be called YOURMETRIC.sys.score.gz and formatted as a tab-separated values (TSV) in the following way:

> METRIC-NAME\tLANG-PAIR\tTESTSET\tREFERENCE\tSYSTEM-ID\tSYSTEM-SCORE  
  
The output files for segment-level scores should be called YOURMETRIC.seg.score.gz and formatted as a tab-separated values (TSV) in the following way:

> METRIC-NAME\tLANG-PAIR\tTESTSET\tREFERENCE\tSYSTEM-ID\tSEGMENT-NUMBER\tSEGMENT-SCORE

Each field should be delimited by a single tab character.

Where:

- **METRIC-NAME** is the name of your automatic evaluation metric.
- **LANG-PAIR** is the language pair using two letter abbreviations for the languages (de-en for German-English, for example).
- **TESTSET** is the ID of the test set (newstest2021, florestest2021, tedtalks or challengeset .
- **REFERENCE** is the ID of the reference (ref-A or ref-B or ref-C or ref-D for reference-based metrics, and src for reference-free metrics
- **SYSTEM-ID** is the ID of system being scored (given by the part of the filename for the plain text file, uedin-syntax for example).
- **SEGMENT-NUMBER** is the line number starting from 1 of the plain text input files.
- **SYSTEM-SCORE** is the score your metric predicts for the particular system.
- **SEGMENT-SCORE** is the score your metric predicts for the particular segment.

**How to submit**
Before you submit, please run your scores files through a validation script, which is now available along with the data in the shared folder.


Note that the English to German data was updated at around 27 July 12:15 pm UTC, and additional system outputs were added to newstest2021 en-de, en-ru and zh-en on July 30th at 8:45 am UTC.

Please enter yourself to [this shared spreadsheet](https://docs.google.com/spreadsheets/d/1bj4i5H-fbZJi3H700P56I7kh0_HWeat1GkVq7-M-ij0/edit?usp=sharing) so we can keep track of your submissions. Submissions should be sent to [wmt22-metric@googlegroups.com](mailto:wmt22-metric@googlegroups.com) with the subject "WMT Metrics submission". You are allowed to submit multiple metrics, but we need you to indicate the primary metric in the email. If submitting more than one metric, please share a folder with all your metrics, for example on Google Drive or Dropbox.

**Before August 6th (AOE)**, please send us an email with:

- a short paragraph to describe your metric;
- a list of resources that your metric needs. For example None, or WordNet, or GIZA++, or word2vec, or BERT;
- if your metric is supervised, then the training and validation datasets. For example, Unsupervised, or WMT21 DA, or MetricsMQM, or proprietary HTER
- a reference so we can cite your metric in the metrics task results paper. If this is a submission to WMT22, please email the name of the paper and the list of authors. Otherwise, send a bibtex reference to a previously published paper or a pre-print (like Arxiv).


## Organization:

- Markus Freitag, Google Research
- Ricardo Rei, Unbabel and Instituto Superior Técnico
- Nitika Mathur, University of Melbourne
- Chi-kiu (Jackie) Lo, NRC Canada
- George Foster, Google Research
- Alon Lavie, Unbabel
- Craig Stewart, Unbabel
- Tom Kocmi, Microsoft Research
- André Martins, Unbabel and Instituto Superior Técnico
- Eleftherios Avramidis, German Research Center for Artificial Intelligence (DFKI)

## Sponsors

<style>
	.column {
	  float: left;
	  padding: 20px;
	}
	
</style>
<div style="position: relative; width: 700px; height: 100px; min-height: 200px">    
    <div style="position: relative; bottom: 0px;">
	   <div class="column">
	     <img src="/public/css/google.png" height=70px width=auto>
	   </div>
	   <div class="column">
	     <img src="/public/css/unbabel.png" height=70px width=auto>
	   </div>
	   <div class="column">
	     <img src="/public/css/microsoft.jpeg" height=70px width=auto>
	   </div>
	</div>

<div style="position: relative; width: 700px; height: 100px; min-height: 200px">    
    <div style="position: relative; bottom: 0px;">
	   <div class="column">
	     <img src="/public/css/melbourne.png" height=70px width=auto>
	   </div>
	   <div class="column">
	     <img src="/public/css/NRC-logo.png" height=70px width=auto>
	   </div>
	   <div class="column">
	     <img src="/public/css/IST.png" height=70px width=auto>
	   </div>
	   <div class="column">
	     <img src="/public/css/DFKI.jpeg" height=50px width=auto>
	   </div>
	</div>
