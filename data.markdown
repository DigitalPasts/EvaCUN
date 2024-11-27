---
layout: page
title: Data
permalink: /Data/
---
___

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
