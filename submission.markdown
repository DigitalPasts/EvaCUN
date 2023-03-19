---
layout: page
title: Submission
permalink: /Submission/
---

## Submitting Runs
Once the system has produced the results for the task over the test set, participants have to follow these instructions for completing your submission:

### File naming
Name the runs with the following filename format:

`taskID_teamName_systemID_modality.tsv`

For example: `testa_unicatt_closed.tsv` would be the first run of a team called "unicatt" using the closed modality for the task using testa.txt(TBD) document (the Akkadian-to-English machine translation).

### Submission format
The output files for system-level rankings should be formatted as a tab-separated values (TSV) in the following way:

**\<id>\\t\<source>\\t\<translation>[\\t\<translation>]**

Each field should be delimited by a single tab character.

Where:

**\<id>**  is the ID of source data (original Akkadian text).

**\<source>** is the original Akkadian text.

**< translation >** is the machine translation result of your system.

(________Table)

### How to submit
Before you submit, please run your scores files through a validation script, which we will provide later. You can use it along with either BLEU, chrF or COMET-QE sys.

Submissions should be sent to (________) with the subject `EvaCun Submission: taskID - teamName`, where the “taskID” is either testa(TBD) or testb(TBD).

You can make up to 2 submissions per language pair, per team.

## Writing the Technical Report
Papers should not be longer than 4 pages for content (for references, unlimited number of pages is allowed). The papers must follow the MT Summit 2023 style guides (PDF version, LaTeX version, MS Word version, and Overleaf template and be submitted in PDF format. To allow for blind reviewing, please do not include author names and affiliations within the paper and avoid obvious self-references.

Papers must be submitted to the website by the conference submission deadline.