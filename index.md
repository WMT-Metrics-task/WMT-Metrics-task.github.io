---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

# Welcome to the WMT 2022 Chat Shared Task!

<p class="message">  
  Translating conversational text, in particular customer support chats, is an important and challenging application task for machine translation technology. This type of content has so far not been extensively explored in prior MT research, largely due to the lack of publicly available data sets. Prior related work has mostly focused on movie subtitles and European Parliament speeches.<br /><br />
  
  The primary goal of this Chat shared task is to encourage participants to train and test models specific for bilingual chat conversations in a corpus composed of original bilingual costumer support conversations. <br /><br />
  
  The language-pairs tested are: en⇔de, en⇔fr, and en⇔pt_br.<br /><br />

  We encourage participants to use the <strong>bilingual context</strong> in the translation models  submissions.<br /><br /> 
  
  Have questions or suggestions? Feel free to <a href="mailto:wmt.metrics@gmail.com">Contact Us</a>!
</p>

## Chat Task Important Dates

|  | Date |
| ----------- | :-----------: |
| Validation set ready to download | TBA |
| Test set ready to download | TBA |
| Submission deadline for Chat task | 23-28th July, 2022 |
| Paper submission deadline to WMT | 7th September, 2022 |
| WMT Notification of acceptance | 9th October, 2022 |
| WMT Camera-ready deadline | 16th October, 2022 |
| Conference | 7th - 8th December, 2022 |

## Goals

The goals of chat translation shared task are to provide the common ground for:

- Studying the applicability of machine translation systems for translating conversational text;
- Investigating the impact of context in a conversation's translation;
- Studying the feasibility of an all-in-one multi-lingual system;

## Task Description

A critical challenge faced by international companies today is delivering customer support in several different languages. One solution to this challenge is centralizing support with English speaking agents and having a translation layer in the middle to translate from the customer's language into the agent's (English) and vice versa.

Although this year's task is not focused on dealing with noisy input nor measuring the model's robustness to such noise, the original English data contains different types of noise including typos, wrong capitalization, among others; and while not required, the participants might want to take this aspect into consideration when developing their models.

1. Official results: Correlation with MQM scores at the sentence and system level, accounting for both directions, for the following language pairs:
   - English⇔German,
   - English⇔French
   - English-Portuguese-br
2. Secondary Evaluation: Correlation with automatic scores at the sentence and system level.

## Data

The data used in this shared task is part of a unique corpus called MAIA corpus that is composed with genuin bilingual costumer support conversations.

### Subtracks:

1. [Zero-shot](./subtasks/zero-shot/): In this subtask participants have to develop machine translation systems without access to any training data.
2. [Low-resource](./subtasks/low-resource/): In this subtask participants have to develop machine translation systems with access to bilingual conversations without reference translations.
   
## Paper Describing Your Metric
You are invited to submit a short paper (4 to 6 pages) to WMT describing your translation model. Information on how to submit is available here. Shared task submission description papers are non-archival, and you are not required to submit a paper if you do not want to. If you don't, we ask that you give an appropriate reference describing your metric that we can cite in the overview paper.

## Data available

TBA


## Test Sets (Evaluation Data)

TBA

### Submission Format

TBA

**How to submit**
Before you submit, please run your scores files through a validation script, which is now available along with the data in the shared folder.

Please enter yourself to [this shared spreadsheet](https://docs.google.com/spreadsheets/d/1bj4i5H-fbZJi3H700P56I7kh0_HWeat1GkVq7-M-ij0/edit?usp=sharing) so we can keep track of your submissions. Submissions should be sent to [wmt.chat@gmail.com](mailto:wmt.chat@gmail.com) with the subject "WMT Chat submission". [REPLACE THIS FOR THE OCELOT PLATFORM!]

**Before August 6th (AOE)**, please send us an email with:

- a short paragraph to describe your translation model;
- a list of resources that your translation model needs. For example None, or WordNet, or GIZA++, or word2vec, or BERT;
- if your translation model is supervised, then the training and validation datasets;
- a reference so we can cite your translation modeel in the Chat task results paper. If this is a submission to WMT22, please email the name of the paper and the list of authors. Otherwise, send a bibtex reference to a previously published paper or a pre-print (like Arxiv).


## Organization:

- Ana C. Farinha, Unbabel
- M. Amin Farajian, Unbabel
- Patrick Fernandes, Google and CMU and Instituto Superior Técnico
- José Souza, Unbabel
- João Alves, Unbabel
- António Lopes, Unbabel
- Helena Moniz, INESC-ID and Unbabel 
- André Martins, Unbabel and Instituto Superior Técnico

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
	     <img src="/public/css/unbabel.png" height=100px width=auto>
	   </div>
	</div>


