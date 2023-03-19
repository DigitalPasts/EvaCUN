---
layout: page
title: Data
permalink: /Data/
---
For the Akkadian part we used the following corpora from ORACC, which include
transliterations and their equivalent English translations: RINAP, RIAo, RIBO, SAAo and
Suhu. Chronologically, the great majority of the texts are NeoAssyrian and the best attested
genres are the royal inscriptions (2,997) and administrative letters (2,003). Nevertheless, the
chosen corpus represents a variety of genres. For the transcription to English we used
56,160 sentences, where we treat each sentence as an independent example for training. We
call them in this article “sentences”, even if it is a single word, a group of words, a phrase or
a group of phrases. The shortest sentences in the Cuneiform-to-English task, for example,
are made up of three characters, while the longest is 237 characters long. The median, 118
characters, is considered a medium length sentence. This is relevant because, as stated later
in the human evaluation, the length of a sentence has an effect on the NMT’s performance.

# Data Format
All data is in Unicode (UTF-8) format. The figure below gives an example of the parallel
corpus data format:  

![hello](/images/parallel_corpus_data_format.jpg)


On the left side is the Cuneiform text, on the middle is the English translation and on the
right side is the Akkadian transcription into Latin script.

# Data Splits
We pooled all corpora together and partitioned them in the following manner: 90% for
training (50,544 sentences), 5% for validation (2,808 sentences) and 5% for testing (2,808
sentences). The average length of a sentence is 15.68 characters with 3,723 sentences over
50 characters long and 61 over 200 characters long. There are 2,440 unique transliterations
and 30,101 unique English words.  

Test data will be provided in the same format as the
training data. The details of the test data will be provided to the participants after the
evaluation.
