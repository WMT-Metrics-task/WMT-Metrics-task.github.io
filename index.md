---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

# Welcome to the WMT 2022 Metrics Shared Task!

<p class="message">
  This shared task will examine automatic evaluation metrics for machine translation. We will provide you with MT system outputs along with source text and the human reference translations. We are looking for automatic metric scores for translations at the system-level, and segment-level. We will calculate the system-level, and segment-level correlations of your scores with human judgements.<br /><br />

  We invite submissions of <strong>reference-free metrics</strong> in addition to <strong>reference-based metrics</strong>.<br /><br />   
  
  Have questions or suggestions? Feel free to <a href="mailto:wmt.metrics@gmail.com">Contact Us</a>!
</p>

## Metrics Task Important Dates

|  | Date |
| ----------- | :-----------: |
| System outputs ready to download | TBA |
| Submission deadline for metrics task | TBA |
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

1. Official results: Correlation with MQM scores at the sentence and system level.
2. Secondary Evaluation: Correlation with official WMT Direct Assessment (DA) scores at the sentence and system level.

### Subtasks:

1. [QE as a Metric](./subtasks/qe/): In this subtask participants have to score machine translation systems without access to reference translations
2. [Challenge Sets](./subtasks/challenge/): While other participants are worried with building stronger and better metrics, participants of this subtask have to build challengesets that identify where metrics fail! 
3. [Minimum Bayes-Risk (MBR) Decoding](./subtasks/mbr/): MBR decoding typically uses metrics as utility function. We invite participants to stress test their metric when used during MBR decoding. 

## Paper Describing Your Metric
You are invited to submit a short paper (4 to 6 pages) to WMT describing your automatic evaluation metric. Information on how to submit is available here. Shared task submission description papers are non-archival, and you are not required to submit a paper if you do not want to. If you don't, we ask that you give an appropriate reference describing your metric that we can cite in the overview paper.

## Training Data
You may want to use some of the following data to tune or train your metric:

**MQM (Multidimensional Quality Metrics) Framework Development/Training Data**

WMT20 and WMT21 en-de, zh-en: [https://github.com/google/wmt-mqm-human-evaluation](https://github.com/google/wmt-mqm-human-evaluation)

**DA (Direct Assessment) Development/Training Data**

For **system-level**, see the results from the previous years:

- WMT21: [http://www.statmt.org/wmt21/results.html](http://www.statmt.org/wmt21/results.html)
- WMT20: [http://www.statmt.org/wmt20/results.html](http://www.statmt.org/wmt20/results.html)
- WMT19: [http://www.statmt.org/wmt19/results.html](http://www.statmt.org/wmt19/results.html)
- WMT18: [http://www.statmt.org/wmt18/results.html](http://www.statmt.org/wmt18/results.html)
- WMT17: [http://www.statmt.org/wmt17/results.html](http://www.statmt.org/wmt17/results.html)
- WMT16: [http://www.statmt.org/wmt16/results.html](http://www.statmt.org/wmt16/results.html)

For **segment-level**, the following datasets are available:

- WMT21: [http://www.statmt.org/wmt21/results.html](http://www.statmt.org/wmt21/results.html)
- WMT20: [http://www.statmt.org/wmt20/results.html](http://www.statmt.org/wmt20/results.html)
- WMT19: [http://www.statmt.org/wmt19/results.html](http://www.statmt.org/wmt19/results.html)
- WMT18: [http://www.statmt.org/wmt18/results.html](http://www.statmt.org/wmt18/results.html)
- WMT17: [http://www.statmt.org/wmt17/results.html](http://www.statmt.org/wmt17/results.html)
- [DAseg-wmt-newstest2016.tar.gz](https://www.dcu.ie/computing~ygraham/DAseg-wmt-newstest2016.tar.gz): 7 language pairs (sampled from newstest2016, tr-en fi-en cs-en ro-en ru-en en-ru de-en; always 560 sentence pairs)
- [DAseg-wmt-newstest2015.tar.gz](https://www.dcu.ie/computing~ygraham/DAseg-wmt-newstest2015.tar.gz): 5 language pairs (sampled from newstest2015, en-ru de-en ru-en fi-en cs-en; always 500 sentence pairs)

Each DA dataset (WMT15/WMT16) contains:

- the source sentence
- MT output (blind, no identification of the actual system that produced it)
- the reference translation
- human score (a real number between -Inf and +Inf)

**RR (Relative Ranking) from Past Years**

Although RR is no longer the manual evaluation employed in the metrics task, human judgments from the previous year's data sets may still prove useful:

- WMT16: [http://www.statmt.org/wmt16/results.html](http://www.statmt.org/wmt16/results.html)
- WMT15: [http://www.statmt.org/wmt15/results.html](http://www.statmt.org/wmt15/results.html)
- WMT14: [http://www.statmt.org/wmt14/results.html](http://www.statmt.org/wmt14/results.html)
- WMT13: [http://www.statmt.org/wmt13/results.html](http://www.statmt.org/wmt13/results.html)
- WMT12: [http://www.statmt.org/wmt12/results.html](http://www.statmt.org/wmt12/results.html)
- WMT11: [http://www.statmt.org/wmt11/results.html](http://www.statmt.org/wmt11/results.html)
- WMT10: [http://www.statmt.org/wmt10/results.html](http://www.statmt.org/wmt10/results.html)
- WMT09: [http://www.statmt.org/wmt09/results.html](http://www.statmt.org/wmt09/results.html)
- WMT08: [http://www.statmt.org/wmt08/results.html](http://www.statmt.org/wmt08/results.html)

You can use any past year's data to tune your metric's free parameters if it has any for this year's submission. Additionally, you can use any past data as a test set to compare the performance of your metric against published results from past years metric participants.

Last year's data contains all of the system's translations, the source documents and human reference translations and the human judgments of the translation quality.

## Test Sets (Evaluation Data)
**TBA**

### Submission Format
The output of your software should produce scores for the translations either at the system-level or the segment-level (or preferably both). As of last year, we no longer include document level evaluation.

There are sample metrics (with random scores) available in the validation folder in the shared data folder.

**Output file format for system-level rankings**

The output files for system-level rankings should be called YOURMETRIC.sys.score.gz and formatted in the following way:

	<METRIC NAME>   <LANG-PAIR>   <TEST SET> <REFERENCE>   <SYSTEM-ID>   <SYSTEM LEVEL SCORE>   
  
The output files for segment-level scores should be called YOURMETRIC.seg.score.gz and formatted in the following way:

	<METRIC NAME>   <LANG-PAIR>   <TESTSET>   <REFERENCE>   <SYSTEM-ID>      <SEGMENT NUMBER>   SEGMENT SCORE>  
  
Each field should be delimited by a single tab character.

Where:

- **METRIC NAME** is the name of your automatic evaluation metric.
- **LANG-PAIR** is the language pair using two letter abbreviations for the languages (de-en for German-English, for example).
- **TEST SET** is the ID of the test set (newstest2021, florestest2021, tedtalks or challengeset .
- **REFERENCE** is the ID of the reference (ref-A or ref-B or ref-C or ref-D for reference-based metrics, and src for reference-free metrics
- **SYSTEM-ID** is the ID of system being scored (given by the part of the filename for the plain text file, uedin-syntax for example).
- **SEGMENT NUMBER** is the line number starting from 1 of the plain text input files.
- **SYSTEM SCORE** is the score your metric predicts for the particular system.
- **SEGMENT SCORE** is the score your metric predicts for the particular segment.

**How to submit**
Before you submit, please run your scores files through a validation script, which is now available along with the data in the shared folder.


Note that the English to German data was updated at around 27 July 12:15 pm UTC, and additional system outputs were added to newstest2021 en-de, en-ru and zh-en on July 30th at 8:45 am UTC.

Please enter yourself to this shared spreadsheet asap so we can keep track of your submissions. Submissions should be sent to wmt.metrics@gmail.com with the subject "WMT Metrics submission". You are allowed to submit multiple metrics, but we need you to indicate the primary metric in the email. If submitting more than one metric, please share a folder with all your metrics, for example on Google Drive or Dropbox.

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
