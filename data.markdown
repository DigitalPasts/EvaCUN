---
layout: page
title: Data
permalink: /Data/
---
___

This shared task focuses on advancing computational approaches to understanding Akkadian, a Semitic language of the ancient Near East. Participants are invited to tackle two challenging tasks designed to test their systems' ability to process and interpret Akkadian texts, which often exhibit unique linguistic complexities.

## Lemma Prediction in Context
The first task is to predict the correct lemma for each word in a given sentence. Unlike straightforward lemmatization, this task requires systems to account for contextual nuances that influence lemma assignment. Akkadian, with its extensive use of homographs and context-dependent morphology, makes this problem particularly intricate. For instance, the same surface form may correspond to multiple lemmas depending on its syntactic or semantic environment.

## Text Restoration
The second task involves completing sentences with missing words. Participants will receive texts where certain words are replaced by placeholders, and their goal is to predict the correct form to fill these gaps. This task evaluates systems' ability to understand broader sentence structure, context, and linguistic conventions of Akkadian. Success in this task demonstrates a system's proficiency in both lexical and syntactic reconstruction.


## Data Format

**Lemmatization** - CSV file where each row represents a single word. The file includes the columns 'value' and 'uniqueLemma' for the training part (you may also use other available columns if they help your prediction).
**Text Restoration Task** - CSV file with lines of texts. Notice that since Akkadian does not contain sentences as in modern languages, the context for the restoration is based on the actual lines of the original text in their respective order.


## Data Splits
**Lemmatization** -
We pooled all corpora together and partitioned them in the following manner: 80% for training (NUMBER lines) and 20% for testing (NUMBER lines). The average length of a line is  characters.

**Text Restoration Task** - The training data consists of NUMBER lines. In both train and test data ~15% of the words are [MASK] and need to be restored.

## Train Data
**Lemmatization Task**  
<!--[Training_data_Sumerian.zip](/data/Training_data_Sumerian.zip)  -->

**Text Restoration Task**  
<!--[Training_data_Akkadian.zip](/data/Training_data_Akkadian.zip)  -->

## Test Data

**To be published according to schedule**
