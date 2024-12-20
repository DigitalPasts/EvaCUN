---
layout: page
title: Task
permalink: /Task/
---
___
### What is Cuneiform?

The cuneiform writing system is a logo-syllabic script, written mostly by impressing wedge-like shapes on clay tablets. Cuneiform was also written on other preserved media, such as stone monuments and metal objects.  

Sumerian is the first recorded written language, spoken from around the fourth millennium BCE (perhaps before) to the early second millennium BCE. However, it remained a scholarly language studied, copied and taught as part of the cuneiform writing tradition that died out around the first two centuries of the common era. Sumerian is an isolate language that cannot be ascribed to any of the known language families.  

Akkadian is the earliest attested Semitic language, belonging specifically to the East Semitic branch. It is attested in writing from c. 2,700 BCE until the end of cuneiform writing. It was a spoken language for most of this period, until it was gradually replaced by Aramaic in the first millennium BCE. During the second millennium BCE, Akkadian was the *lingua franca* of the ancient Near East, in use from Iran to Anatolia, from Syria to Egypt. As such, significant amounts of cuneiform tablets written in Akkadian and Sumerian were discovered outside of Mesopotamia during this time, within the context of cuneiform traditions of other languages.

### Lemmatization and Token Prediction Tasks 

The **lemmatization and token prediction** tasks of Akkadian and Sumerian documents using Large Language Models (LLMs) is crucial to advance computational text analysis, and create linguistic resources like treebanks and word embeddings. However, since cuneiform languages are low-resource languages, the existing corpora of texts consists of a relatively limited amount of data for each historical period of cuneiform, which is moreover divided into different geographical areas and text genres.[^1] Existing lemmatizers have relied mostly on first millennium BCE Assyrian and Babylonian archival and royal texts, and the fragmentary nature of many cuneiform tablets, as well as lexical homonymy in Akkadian and Sumerian, makes the creation of new computational linguistic resources challenging. 

EvaCun 2025 datasets consist of first millennium BCE literary, scientific, and archival texts, mostly from the cuneiform tablets in the British Museum, and early second millennium BCE letters from Mesopotamia. The texts are not split across datasets and/or train-test splits. In Akkadian there are no modern punctuation marks, so the basic unit for context is the physical line on the cuneiform tablet. All the texts are originally written in cuneiform, but for simplicity's sake we bring them here in their transliterated form (i.e. syllabic writing in latin characters).

* **Lemmatization Dataset**: Consists of xyz words and their respective lemma. The words appear in their relative order within a certain text. 
* **Token Prediction Dataset**: Consists of xyz lines of texts and xyz words. In the test split 15% of the words are masked and require prediction. In a later stage, the most successful model could be used to restore actual missing tokens (eroded or physically broken) in cuneiform tablets.

Both datasets contain additional information whenever possible, such as the text genre, tablet find place, word language (Akkadian, Sumerian, etc. Many text contain words from multiple languages). Feel free to use the additional information as you please and find helpful, make sure to include all the information you used in the technical report. The organizers rely on the honesty of all participants who might have some prior knowledge of part of the data that will be used for evaluation. **Unfairly use of such knowledge is not permitted in the shared task.**

### Research Agenda 

We encourage participants to harness LLMs to develop cutting-edge solutions to these tasks that are traditionally done manually or with classic computational methods. We would like to answer three main questions regarding the use of LLMs and cuneiform (LLMs broadly defined, indluding transformer models like BERT, for example):
- Can LLMs show the best performance in lemmatization and token prediction tasks for Akkadian and Sumerian?
- How can we use LLMs to promote the development of resources and language technologies for Cuneiform languages?
- How can we use LLMs to foster collaboration between cuneiform scholars and researchers from different disciplines?

It is important to state that while we encourage participants to use LLMs in their solutions, we do NOT expect to train an LLM from scratch for this task, nor it is feasable with this amount of data. Ideally, we want to use existing instruct-based LLMs that can understand queries in English about cuneiform texts (this is challenging).

### FAQ
**Can we use/add our own data for training?**

No, to avoid data contamiation we request that you'll only work on the data we provide. The data consists of several corpora that we also pre-processed to fit the task so it's important for both training and evaluation not to modify it.

**Can we use instruct-base LLM (such as ChatGPT)?**

Yes, although data contamination holds for these models too, some things are not in our control. However, if you choose to use an instruct-based model make sure to add the conversation entirely (initial prompts, refined prompts, chat-response, etc.) to the technical report as an appendix.

**Can we use Akkadian-based models found online (e.g. on HuggingFace)?**

That depends. Obviously, you can't use someone else's lemmatization model and submit it as your own work. You can use models that were trained on Akkadian for a different task than what you're working on, BUT you'll have to specify in your technical report exactly what they were trained to do, on what data, how successful they were and cite them appropriately. If the model card in HF does not specify this information - you can't use the model.

### About the Organizers 
EvaCun 2025 is co-organized with [ALP 2025](https://www.ancientnlp.com/alp2025/), Albuquerque, New Mexico, US from April 29 to May 4, 2025. As a co-located event with [NAACL 2025](https://2025.naacl.org/), this workshop will provide an opportunity to learn about the challenges and latest developments in the field of ancient languages processing. EvaCun 2025 is organized by the [Digital Pasts lab](https://digitalpasts.github.io/) at Ariel University and the TAD Center for AI and Data Science at Tel-Aviv University, Israel, and is sponsored by the electronic Babylonian Library (LMU Munich) and ARCHIBAB (Collège de France) projects. 

---
[^1]: For a good textual and linguistic overview of Akkadian and its periodization, for example, see Vita, J.-P. (Ed.). (2021). _History of the Akkadian language_. Brill. https://doi.org/10.1163/9789004445215
