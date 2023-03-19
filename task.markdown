---
layout: page
title: Task
permalink: /task/
---
There are several challenges in translating an ancient language like Akkadian. Clay tablets
are rarely completely preserved. As a result, NMT is affected by the lack of context.
Another challenge is the complex logophonetic nature of cuneiform, i.e. signs can have one
of three functions: logograms, determinatives and phonograms/syllabograms. Therefore,
cuneiform signs are polyvalent and have several readings for each function.
Sometimes, even experts cannot figure out the proper sign value.  
Experts do not translate directly to a
modern language from the ancient cuneiform signs. They first gauge the context of each
sign in each sequence – a process which is called "transliteration", resulting in a transcription
of the cuneiform signs in the Latin alphabet. The first step of transliteration is considered in
computational terms to be another sort of translation task. It can include word segmentation,
as cuneiform practically lacks any sort of punctuation marks, therefore, cuneiform
translation (CT) is considered a more complex translation task than transcription translation
(TT). CT requires translation between two different scripts, Unicode cuneiform glyphs to
Latin script, as well as identification of word segmentation. The act of transliteration not
only removes the levels of sign and word ambiguity from the cuneiform signs, it also
simplifies the task of translation between the same script type. Another issue to consider
when translating Akkadian is the different styles of each text genre. The more formulaic the
genre of the source, the more accurate the translation will be. Generally, administrative and
divinatory texts tend to be very formulaic. Furthermore, texts in Akkadian are rarely written
entirely syllabically, as described above, and almost all of them use Sumerian logograms
(transliterated in capital letters). Certain genres, such as divination literature, use logograms
profusely, with many sentences made up only of logograms. Often, the names of people,
places, and temples are themselves complex sentences written using logograms.

# Task Objectives

The goals of the translation task are:
- To investigate the applicability of current MT techniques when translating Akkadian
into English.
- To examine the difference between translating from the cuneiform source and the Latin
transcription.
- To create publicly available corpora for machine translation and evaluation of Akkadian
and Sumerian
- To provide practical experience of the most advanced machine translation methods for
beginners in the field of machine translation
- To prompt the development of machine translation research for Akkadian and Sumerian
and advance the forefront of machine translation technology exploration

# Task Requirements
We will provide parallel corpora of English-Akkadian Cuneiform-Akkadian Transcription,
and Sumerian-English, as well as provide several multilingual models such as RoBERTa
for English. The goal is to improve the model and enhance machine translation performance.
You can choose to participate in any of the tasks, and we will use the same metrics for
evaluation. You can use other models and resources to build the translation system or just
build your own model. However, if additional data is used, participants should clearly
indicate which data is from the provided dataset and which is from external sources. This
will allow us to evaluate the performance of the models on our provided dataset separately
from their performance on external data.
Each participant should include a brief introduction of their translation system when
submitting, including basic information such as the models (if any), techniques, methods
used, etc. Each participant should submit a technical reports emphasizing improvements
made to the model, techniques used, and methods applied.
Although the primary objective of this evaluation is to identify the most exceptional
machine translation system, we encourage participation even if your approach does not
achieve the highest performance. If you have developed an interesting approach, this
evaluation provides an opportunity to further refine and enhance your system.