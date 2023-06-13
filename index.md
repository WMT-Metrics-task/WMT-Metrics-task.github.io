---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

# Welcome to the WMT 2023 Metrics Shared Task!

<p class="message">
  This shared task will examine automatic evaluation metrics for machine translation. We will provide you with MT system outputs along with source text and the human reference translations. We are looking for automatic metric scores for translations at the system-level, and segment-level. We will calculate the system-level, and segment-level correlations of your scores with human judgements.<br /><br />

  We invite submissions of <strong>reference-free metrics</strong> in addition to <strong>reference-based metrics</strong>.<br /><br />   
  
  Have questions or suggestions? Feel free to <a href="mailto:wmt-metrics@googlegroups.com">Contact Us</a>!
</p>

## Important links

[mt-metrics-eval](https://github.com/google-research/mt-metrics-eval): the tool for calculating correlation numbers aka the sacreBLEU for metric developers. You can also dump the most recent test sets.

## Important Dates

|  | Date |
| ----------- | :-----------: |
| **System outputs ready to download** | **10th August, 2023** |
| **Submission deadline for metrics task** | **17th August, 2023 ❗** |
| Paper submission deadline to WMT | 5th September, 2023 |
| WMT Notification of acceptance | 6th October, 2023 |
| WMT Camera-ready deadline | 18th October, 2023 |
| Conference | 6th - 7th December, 2023 |

## Goals

The goals of the shared metrics task are:

- To achieve the strongest correlation with human judgement of translation quality over a diverse set of MT systems;
- To illustrate the suitability of an automatic evaluation metric as a surrogate for human evaluation;
- To test robustness of metrics when evaluating domains other than news data;
- To create high quality datasets for developing and evaluating metrics

## Task Description

We will provide you with the source sentences, output of machine translation systems and reference translations.

1. Official results: Correlation with MQM scores at the sentence and system level for the following language pairs:
   - Hebrew-English **(NEW!)**
   - Chinese-English
   - English-German **This will be a paragraph-level task!**
2. Secondary Evaluation: Correlation with official [WMT Human Evaluation](http://www2.statmt.org/wmt23/translation-task.html) at the sentence and system level.

### Subtasks:

1. [QE as a Metric](./subtasks/qe/): In this subtask participants have to score machine translation systems without access to reference translations
2. [Challenge Sets](./subtasks/challenge/): While other participants are worried with building stronger and better metrics, participants of this subtask have to build challengesets that identify where metrics fail! 


## How to participate?

Please fill the following [registration form](https://forms.gle/UTBen7EBRJaMFttK6) so we can keep track of participants. Since we will be using [Codalab](https://codalab.lisn.upsaclay.fr/) to handle all submissions you will also have to create an account on codalab and enroll in the competition.

### Paper Describing Your Metric

You are invited to submit a short paper (4 to 6 pages) to WMT describing your automatic evaluation metric. Shared task submission description papers are non-archival, and you are not required to submit a paper if you do not want to. If you don't, we ask that you give an appropriate reference describing your metric that we can cite in the overview paper.

### Submission Format

The output of your software should produce scores for the translations either at the system-level or the segment-level (or preferably both). 

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
- **DOMAIN** is the domain of a given segment. It can be _conversation_, _ecommerce_, _news_, _social_ or _all_. The domain will only be used for *en-de*, *he-en* and *zh-en*. For those languages we will look at results for individual domains + concatenation of all domain (_all_). For all other language pairs the domain should be _all_.
- **DOCUMENT** is the ID of the document. As for the the domain, the document information is only relevant for *en-de*, *he-en* and *zh-en*.
- **REFERENCE** is the ID of the reference (ref-A or ref-B or ref-C or ref-D for reference-based metrics, and src for reference-free metrics
- **SYSTEM-ID** is the ID of system being scored (given by the part of the filename for the plain text file, uedin-syntax for example).
- **SEGMENT-NUMBER** is the line number starting from 1 of the plain text input files.
- **SYSTEM-SCORE** is the score your metric predicts for the particular system.
- **SEGMENT-SCORE** is the score your metric predicts for the particular segment.

#### How to submit:

This year we will be using [Codalab](https://codalab.lisn.upsaclay.fr/) to handle all submissions. We will be providing more details about [Codalab](https://codalab.lisn.upsaclay.fr/) soon!

You are allowed to submit multiple metrics, but we need you to indicate the primary metric.

## Training Data

Since data from previous WMT editions might be difficult to navigate we uploaded previous years data to Hugging Face Datasets. You can find DA, MQM and SQM annotations from previous years in the following links: [wmt-da-human-evaluation](https://huggingface.co/datasets/RicardoRei/wmt-da-human-evaluation), [wmt-mqm-human-evaluation](https://huggingface.co/datasets/RicardoRei/wmt-mqm-human-evaluation), [wmt-sqm-human-evaluation](https://huggingface.co/datasets/RicardoRei/wmt-sqm-human-evaluation).

If you wish to find the original data please check the [previous editions tab](https://wmt-metrics-task.github.io/subtasks/previous/) and in the results section you can find the original DAs. For MQM you can find the data [here](https://github.com/google/wmt-mqm-human-evaluation)

## Organization:

- Alon Lavie, Unbabel
- Brian Thompson, Amazon Research
- Chi-kiu (Jackie) Lo, NRC Canada
- Chryssa Zerva, Instituto de Telecomunicações and Instituto Superior Técnico
- Craig Stewart, Unbabel
- Dan Deutsch, Google Research
- Eleftherios Avramidis, German Research Center for Artificial Intelligence (DFKI)
- Frédéric Blain, Tilburg University
- George Foster, Google Research
- Markus Freitag, Google Research
- Nitika Mathur, Oracle
- Ricardo Rei, Unbabel, INESC-ID and Instituto Superior Técnico
- Sheila Castilho, ADAPT Centre - Dublin City University
- Tom Kocmi, Microsoft Research

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
	   <div class="column">
	     <img src="/public/css/ADAPT.png" height=50px width=auto>
	   </div>
	</div>
