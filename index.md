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
| Breaking round for [challenge sets](./subtasks/challenge/) | **25th July, 2023** |
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

The output files for system-level scores should be called YOURMETRIC.sys.score and formatted as tab-separated values (TSV) in the following way:

> METRIC-NAME\tLANG-PAIR\tTESTSET\tDOMAIN\tREFERENCE\tSYSTEM-ID\tSYSTEM-SCORE 
  
**Output file format for segment-level scores**

The output files for segment-level scores should be called YOURMETRIC.seg.score and formatted as tab-separated values (TSV) in the following way:

> METRIC-NAME\tLANG-PAIR\tTESTSET\tDOMAIN\tDOCUMENT\tREFERENCE\tSYSTEM-ID\tSEGMENT-NUMBER\tSEGMENT-SCORE

Each field should be delimited by a single tab character.

Where:
- **METRIC-NAME** is the name of your automatic evaluation metric. Please use short descriptive names that don't contain spaces.
- **LANG-PAIR** is the language pair using two letter abbreviations for the languages (e.g., he-en, zh-en, and en-de for the official language pairs).
- **TESTSET** is the ID of the test set (e.g., generaltest2023, or challenge*).
- **DOMAIN** is the domain of a given segment. For he-en, zh-en, and en-de, domain should be one of conversation, ecommerce, news, social or all. For other language pairs, use all. For system-level scores, this field designates the domain that is being scored (all means the whole test set). For segment-level scores, DOMAIN is used for verification purposes only.
- **DOCUMENT** is the ID of the document. This field is used for verification only.
- **REFERENCE** is the ID of the reference (refA, refB, etc for reference-based metrics, and src for reference-free metrics).
- **SYSTEM-ID** is the ID of the system being scored (given by the part of the filename for the plain text file, for example “uedin-syntax”).
- **SEGMENT-NUMBER** is the line number starting from 1 of the plain text input files.
- **SYSTEM-SCORE** is the score your metric predicts for the particular system.
- **SEGMENT-SCORE** is the score your metric predicts for the particular segment.

#### Codalab:

This year we will be using [Codalab](https://codalab.lisn.upsaclay.fr/) to handle all submissions.

Create a zip archive containing YOURMETRIC.sys.score and/or YOURMETRIC.seg.score, and upload it using the Submit / View Results tab under Participate. Fill in the meta-information for your team and metric, as prompted.

Each submission should contain scores for only one metric. The official metric name is the one that appears in the METRIC-NAME field in the score files.

Reference-free (aka QE) metrics must have `src` in the REFERENCE field; if a metric is reference free, it must be reference-free for both system- and segment-level scores.

If your submission contains only segment-level scores, we will fill in system-level scores by averaging.

You can make multiple submissions. Each new submission must have a different metric name, and one submission must be designated as primary. Only this submission will participate in the official evaluation (final metric ranking). To designate a submission as primary, include PRIMARY in the Description field. You can update this field to change your primary submission at any time before the evaluation ends.

Primary submissions must include, at minimum, segment-level scores for all official language pairs (Hebrew-English, Chinese-English, English-German). 

**Verify submission:**

After uploading your submission, check that its status (under Submit / View Results) shows Finished and a numerical score appears in the Score column. This can take some time. **Use the Results tab to check your correlation scores on the leaderboard. These are correlations with an automatic metric, and will not reflect your final correlations to human MQM scores, nor your true ranking compared to other submissions.However, if they are very low or negative, it could indicate a problem with your scores.** 

If there is a problem uploading your submission, its status will be Failed, and an Error display will show the reasons for the failure. You can get other information from the links under the Error panel. You can also test your submission offline by running the [scoring script](https://github.com/google-research/mt-metrics-eval/blob/main/mt_metrics_eval/codalab/eval.py) yourself.

There is currently no way to remove failed submissions or replace existing valid submissions from codalab. To indicate that you do not wish us to use a submission, include DISCARD in its Description field.

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
