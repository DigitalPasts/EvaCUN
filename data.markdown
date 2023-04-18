---
layout: page
title: Data
permalink: /Data/
---
___

For the **Akkadian part** we used the following corpora from the Open Richley Annotated Cuneiform Corpus [ORACC](http://oracc.museum.upenn.edu/), which include transliterations and their equivalent English translations: RINAP, RIAo, RIBO, SAAo and Suhu (for more information on these projects see [here](http://oracc.museum.upenn.edu/armep/)). Chronologically, the great majority of the texts are Neo-Assyrian (NA) and the best attested genres are the royal inscriptions (2,997) and administrative letters (2,003). Nevertheless, the chosen corpus represents a variety of genres. For the transcription to English we used 56,160 sentences, where we treat each sentence as an independent example for training. We call them in these guidelines “sentences”, even if they are made up of a single word, a group of words, a phrase or a group of phrases. This is mostly because cuneiform does not have punctuation that separates sentences like modern languages do. The shortest sentences in the cuneiform unicode dataset, for example, are made up of three characters, while the longest is 237 characters long. The median, 118 characters, is considered a medium length sentence. This is relevant because the length of a sentence could affect the performance of the Machine Translation model.  
For the **Sumerian** part we used a corpus from the *Cuneiform Digital Library Initiative* (CDLI) and of a neural network-based encode-decoder architecture for English-Sumerian and Sumerian-English. The Sumerian data is only available in transliterated form. The project carries out English<-->Sumerian Translation using a parallel corpus of about 20K sentences for both languages as the parallel corpora.


## Data Format
**Akkadian** - All data is in Unicode (UTF-8) format. The figure below gives an example of the parallel
corpus data format:  

![Akkadian](/images/parallel_corpus_data_format.jpg)

On the left side are the Cuneiform unicode glyphs, on the middle is the English translation and on the right side is the Akkadian transcription into Latin script (also known in the literature as transliteration).

**Sumerian** - The Sumerian data comes only in transliteration, therefore there are only two files for each split, the english version and the transliterated version.  
Below is an example of the two files. This is similar (though not identical) to the format of transliterated Akkadian:

![Sumerian](/images/data_format_sumerian.jpg)


## Data Splits
**Akkadian** - 
We pooled all corpora together and partitioned them in the following manner: 90% for training (50,544 sentences), 5% for validation (2,808 sentences) and 5% for testing (2,808 sentences). The average length of a sentence is 15.68 characters with 3,723 sentences over 50 characters long and 61 over 200 characters long. There are 2,440 unique transliterations and 30,101 unique English words. Test data will be provided in the same format as the training data. The details of the test data will be provided to the participants after the evaluation.  

**Sumerian** - The training data consists of 8,117 pairs of aligned lines, validation consists of 1,015 pairs of aligned lines and the test split consists of another 105 pairs of aligned lines. Overall the splits are divided into 80% training, 10% validation and 10% test datasets.