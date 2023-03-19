---
layout: page
title: How to Participate
permalink: /How_to_Participate/
---
## Registration
If you would like to participate in this shared task, please fill out the [registration form](www.nowhere.com) and ensure that your information is correct and your email is able to receive messages. Once we receive your registration information,
we will send the training data to your email address. Please check your email regularly.
If you do not receive a reply for a long time, please check if your email was sent
successfully.

## Submitting Runs
Once the system has produced the results for the task over the test set, participants have to
follow these instructions for completing your submission:
# File Naming
Name the runs with the following filename format:
`taskID_teamName_systemID.txt`  
"taskID" is the unique ID for each task as follows:  
- For Sumerian to English the taskID is `S2E`  
- For Cuneiform to English the taskID is `C2E`   
- For transcribed Akkadian to English the taskID is `T2E`

# Submission format
The output files for system-level rankings should be formatted as a text file in the
following way:
<center><b>&lt;line_number&gt;&lt;pred&gt;</b></center>  
**\<line_number>** is the line number in the source file.  
**\<pred>** is the machine translation outputs of your system.

# How to submit
Before you submit, please run your scores files through a validation script, which we
will provide later. You should use it along with BLEU.  
You can make up to 2 submissions per language pair, per team.

# Writing the Technical Report

Papers should not be longer than 4 pages of content (for references, unlimited number of
pages is allowed). The papers must follow the [MT Summit 2023 style guides](https://www.overleaf.com/latex/templates/mt-summit-2023-
template/knrrcnxhkqxd) (PDF version,
LaTeX version, MS Word version, and Overleaf
template) and be submitted in **PDF format**.  
To allow for blind reviewing,
please do not include author names and affiliations within the paper and avoid obvious self-
references.  

Papers must be submitted to [this website](https://softconf.com/mtsummit2023/research)  by the conference submission deadline.
