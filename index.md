---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

# Welcome to the 2022 Metrics Shared Task!

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
| Paper submission deadline to WMT | TBA |
| WMT Notification of acceptance | TBA |
| WMT Camera-ready deadline | TBA |
| Conference | TBA |

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
**TBA**

## Test Sets (Evaluation Data)
**TBA**

### Submission Format
**TBA**


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
