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

## Important links

[Test data](https://drive.google.com/file/d/1I0O-NzOLCxrO6noub2pY81BtWxp42A46/view?usp=sharing) for the WMT2022 metric shared task.

[Mt-metrics-eval](https://github.com/google-research/mt-metrics-eval): the tool for calculating correlation numbers aka the sacreBLEU for metric developers. You can also dump the most recent test sets.

## Metrics Task Important Dates

|  | Date |
| ----------- | :-----------: |
| **System outputs ready to download** | **16th August, 2022** |
| **Submission deadline for metrics task** |  **23th August, 2022** |
| **Paper submission deadline to WMT** | **7th September, 2022** |
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

## Paper Describing Your Metric
You are invited to submit a short paper (4 to 6 pages) to WMT describing your automatic evaluation metric. Shared task submission description papers are non-archival, and you are not required to submit a paper if you do not want to. If you don't, we ask that you give an appropriate reference describing your metric that we can cite in the overview paper.

## Training Data

 ``❗`` Since data from previous WMT editions might be difficult to navigate we are adding a table with links to download data from previous years. You have new links in the **New: Download links section**

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

Also, for running the mearure metrics quality, specially new ones, we encourage you to use [mt-metrics-eval](https://github.com/google-research/mt-metrics-eval) repo developed by George Foster.

#### New: Download links

##### DA data:

| year | DA | relative ranks | paper |
|:---: | :--: | :---: | :---: |
| 2017 | [🔗](https://unbabel-experimental-data-sets.s3.eu-west-1.amazonaws.com/wmt/2017-da.csv.tar.gz) | [🔗](https://unbabel-experimental-data-sets.s3.eu-west-1.amazonaws.com/wmt/2017-daRR.csv.tar.gz) | [Results of the WMT17 Metrics Shared Task](https://statmt.org/wmt17/pdf/WMT55.pdf) |
| 2018 | [🔗](https://unbabel-experimental-data-sets.s3.eu-west-1.amazonaws.com/wmt/2018-da.csv.tar.gz) |  [🔗](https://unbabel-experimental-data-sets.s3.eu-west-1.amazonaws.com/wmt/2018-daRR.csv.tar.gz) |[Results of the WMT18 Metrics Shared Task](https://statmt.org/wmt18/pdf/WMT078.pdf) |
| 2019 | [🔗](https://unbabel-experimental-data-sets.s3.eu-west-1.amazonaws.com/wmt/2019-da.csv.tar.gz) |  [🔗](https://unbabel-experimental-data-sets.s3.eu-west-1.amazonaws.com/wmt/2019-daRR.csv.tar.gz) |[Results of the WMT19 Metrics Shared Task](https://statmt.org/wmt19/pdf/53/WMT02.pdf) |
| 2020 | [🔗](https://unbabel-experimental-data-sets.s3.eu-west-1.amazonaws.com/wmt/2020-da.csv.tar.gz) |  [🔗](https://unbabel-experimental-data-sets.s3.eu-west-1.amazonaws.com/wmt/2020-daRR.csv.tar.gz) |[Results of the WMT20 Metrics Shared Task](https://aclanthology.org/2020.wmt-1.77.pdf) |

``❗``: We are not providing links to the Direct Assessments from 2021 because we found bugs in the scores. We advise participants to avoid using that data. For 2021 you can rely on the MQM annotations below 👇.

##### MQM data:

| year | LP | testset | paper |
|:---: | :--: | :---: | :---: |
| 2020 | [en-de 🔗](https://unbabel-experimental-data-sets.s3.eu-west-1.amazonaws.com/wmt/MQM/wmt-ende-newstest2020.csv.tar.gz) | Newstest2020 | [A Large-Scale Study of Human Evaluation for Machine Translation](https://aclanthology.org/2021.tacl-1.87.pdf)|
| 2020 | [zh-en 🔗](https://unbabel-experimental-data-sets.s3.eu-west-1.amazonaws.com/wmt/MQM/wmt-zhen-newstest2020.csv.tar.gz) | Newstest2020 | [A Large-Scale Study of Human Evaluation for Machine Translation](https://aclanthology.org/2021.tacl-1.87.pdf)|
| 2021 | [en-ru 🔗](https://unbabel-experimental-data-sets.s3.eu-west-1.amazonaws.com/wmt/MQM/wmt-enru-newstest2021.csv.tar.gz) | Newstest2021 | [Results of the WMT21 Metrics Shared Task](https://aclanthology.org/2021.wmt-1.73.pdf)|
| 2021 | [en-de 🔗](https://unbabel-experimental-data-sets.s3.eu-west-1.amazonaws.com/wmt/MQM/wmt-ende-newstest2021.csv.tar.gz) | Newstest2021 | [Results of the WMT21 Metrics Shared Task](https://aclanthology.org/2021.wmt-1.73.pdf)|
| 2021 | [zh-en 🔗](https://unbabel-experimental-data-sets.s3.eu-west-1.amazonaws.com/wmt/MQM/wmt-zhen-newstest2021.csv.tar.gz) | Newstest2021 | [Results of the WMT21 Metrics Shared Task](https://aclanthology.org/2021.wmt-1.73.pdf)|
| 2021 | [en-ru 🔗](https://unbabel-experimental-data-sets.s3.eu-west-1.amazonaws.com/wmt/MQM/wmt-enru-tedtalks.csv.tar.gz) | Ted Talks | [Results of the WMT21 Metrics Shared Task](https://aclanthology.org/2021.wmt-1.73.pdf)|
| 2021 | [en-de 🔗](https://unbabel-experimental-data-sets.s3.eu-west-1.amazonaws.com/wmt/MQM/wmt-ende-tedtalks.csv.tar.gz) | Ted Talks | [Results of the WMT21 Metrics Shared Task](https://aclanthology.org/2021.wmt-1.73.pdf)|
| 2021 | [zh-en 🔗](https://unbabel-experimental-data-sets.s3.eu-west-1.amazonaws.com/wmt/MQM/wmt-zhen-tedtalks.csv.tar.gz) | Ted Talks | [Results of the WMT21 Metrics Shared Task](https://aclanthology.org/2021.wmt-1.73.pdf)|

``❗``: MQM data for _en-de_ and _zh-en_ was mostly annotated by Google and it ranges -25 to 0 where 0 is a perfect translation and -25 is the worse possible score. On the other hand, _en-ru_ data was annotated by Unbabel and ranges -inf to 100 where 100 is a perfect translation and something below 0 is a bad translation. You can find the original data [here](https://github.com/google/wmt-mqm-human-evaluation) with more information about raters, etc...


## Test Sets (Evaluation Data)

You can download the System outputs from [here](https://drive.google.com/file/d/1I0O-NzOLCxrO6noub2pY81BtWxp42A46/view?usp=sharing)

### Submission Format

The output of your software should produce scores for the translations either at the system-level or the segment-level (or preferably both). 

We release along with the data two python scripts to help you score the data. The scripts should be easy to modify in order to run your metrics. We advise you to use them.

We also provide 4 examples of scored data using BLEU, chrF, BLEURT, and COMET-QE (for QE-as-a-metric) available [here](https://drive.google.com/file/d/1I0O-NzOLCxrO6noub2pY81BtWxp42A46/view?usp=sharing) 


**Output file format for system-level rankings**

The output files for system-level rankings should be called YOURMETRIC.sys.score.gz and formatted as a tab-separated values (TSV) in the following way:

> METRIC-NAME\tLANG-PAIR\tTESTSET\tDOMAIN\tREFERENCE\tSYSTEM-ID\tSYSTEM-SCORE  
  
The output files for segment-level scores should be called YOURMETRIC.seg.score.gz and formatted as a tab-separated values (TSV) in the following way:

> METRIC-NAME\tLANG-PAIR\tTESTSET\tDOMAIN\tDOCUMENT\tREFERENCE\tSYSTEM-ID\tSEGMENT-NUMBER\tSEGMENT-SCORE

Each field should be delimited by a single tab character.

Where:

- **METRIC-NAME** is the name of your automatic evaluation metric.
- **LANG-PAIR** is the language pair using two letter abbreviations for the languages (de-en for German-English, for example).
- **TESTSET** is the ID of the test set (newstest2021, florestest2021, tedtalks or challengeset.
- **DOMAIN** is the domain of a given segment. It can be _conversation_, _ecommerce_, _news_, _social_ or _all_. The domain will only be used for *en-de*, *en-ru* and *zh-en*. For those languages we will look at results for individual domains + concatenation of all domain (_all_). For all other language pairs the domain should be _all_.
- **DOCUMENT** is the ID of the document. As for the the domain, the document information is only relevant for *en-de*, *en-ru* and *zh-en*. The information about each document and domain can be found in the `metrics_inputs/txt/generaltest2022/metadata`.
- **REFERENCE** is the ID of the reference (ref-A or ref-B or ref-C or ref-D for reference-based metrics, and src for reference-free metrics
- **SYSTEM-ID** is the ID of system being scored (given by the part of the filename for the plain text file, uedin-syntax for example).
- **SEGMENT-NUMBER** is the line number starting from 1 of the plain text input files.
- **SYSTEM-SCORE** is the score your metric predicts for the particular system.
- **SEGMENT-SCORE** is the score your metric predicts for the particular segment.


#### How to submit:

Before you submit, please run your scores files through a validation script, which is now available [here](https://drive.google.com/file/d/12_uzUVUJAppN5PQLo1Uh8TK9UcwV0AfW/view?usp=sharing). You can use it along with either BLEU or COMET-QE sys and seg scores files in the [baselines folder](https://drive.google.com/file/d/1I0O-NzOLCxrO6noub2pY81BtWxp42A46/view?usp=sharing) 

Please enter yourself to [this shared spreadsheet](https://docs.google.com/spreadsheets/d/1bj4i5H-fbZJi3H700P56I7kh0_HWeat1GkVq7-M-ij0/edit?usp=sharing) so we can keep track of your submissions.  

Submissions should be sent to [wmt22-metric@googlegroups.com](mailto:wmt22-metric@googlegroups.com) with the subject "WMT Metrics submission". 

You are allowed to submit multiple metrics, but we need you to indicate the primary metric in the email. If submitting more than one metric, please share a folder with all your metrics, for example on Google Drive or Dropbox.

**Before August 30th (AOE)**, please send us an email with:

- a short paragraph to describe your metric;
- a list of resources that your metric needs. For example None, or WordNet, or GIZA++, or word2vec, or BERT;
- if your metric is supervised, then the training and validation datasets. For example, Unsupervised, or WMT21 DA, or MetricsMQM, or proprietary HTER
- a reference so we can cite your metric in the metrics task results paper. If this is a submission to WMT22, please email the name of the paper and the list of authors. Otherwise, send a bibtex reference to a previously published paper or a pre-print (like Arxiv).


## Organization:

- Markus Freitag, Google Research
- Ricardo Rei, Unbabel and Instituto Superior Técnico
- Nitika Mathur, Oracle
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
	     <img src="/public/css/NRC-logo.png" height=70px width=auto>
	   </div>
	   <div class="column">
	     <img src="/public/css/IST.png" height=70px width=auto>
	   </div>
	   <div class="column">
	     <img src="/public/css/DFKI.jpeg" height=50px width=auto>
	   </div>
	</div>
