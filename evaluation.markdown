---
layout: page
title: Evaluation
permalink: /Evaluation/
---

## Metrics

We will evaluate the performance of `cuneiform/transcription/Sumerian-to-English` machine
translation model. The scorers employed for EvaCun 2023 are based on `BLEU`.  

Each participating team will initially have access only to the training data.  
Later, test data
containing only cuneiform and transcribed texts will also be released.  

The `BLEU` metrics measure machine translation quality by word-level n-grams. It is a
modified version of the `sacreBLEU`, which provides hassle-free computation of shareable,
comparable, and reproducible `BLEU` scores.

## Baselines

We will use the results of the NMT from the paper “Translating Akkadian to English with Neural
Machine Translation” (in press PNAS Nexus) as baseline.  Its code and supplementary information is available [here](https://github.com/gaigutherz/Akkademia) and [here](https://github.com/DigitalPasts/AkkadiantoEnglish_NMT_SI).
