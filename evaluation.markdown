---
layout: page
title: Evaluation
permalink: /Evaluation/
---
___
## Metrics

### Evaluation Metrics for the Shared Task

#### **1. Lemmatization Task**  
The lemmatization task will be evaluated using the following metrics:

- **Accuracy (Exact Match)**: The percentage of words for which the predicted lemma matches the gold standard lemma exactly. This is the primary metric for evaluating the overall performance of the system.
  
$$
\text{Accuracy} = \frac{\text{Number of Correct Lemma Predictions}}{\text{Total Number of Words}}
$$

- **Error Analysis Categories**: Systems will also be evaluated qualitatively by analyzing errors across categories such as:
  - Homographs: Words with the same form but different meanings or lemmas.
  - Rare Lemmas: Lemmas that occur infrequently in the dataset.
  - Morphological Complexity: Cases with challenging inflectional variations.

#### **2. Token Prediction Task**  
The evaluation of the text completion task will include a combination of traditional accuracy metrics and perplexity to provide a comprehensive assessment of system performance.

#### **Primary Metrics**
- **Top-1 Accuracy**: The percentage of placeholders correctly filled with the exact word predicted as the top-ranked choice by the system.
  
$$
\text{Top-1 Accuracy} = \frac{\text{Number of Correct Predictions}}{\text{Total Number of Masked Words}}
$$
  
- **Top-3 Accuracy**: this metric evaluates whether the correct word appears within the top k predictions

$$
\text{Top-}3 \, \text{Accuracy} = \frac{\text{Number of Masked Words where the Correct Word is in the Top-}3 \, \text{Predictions}}{\text{Total Number of Masked Words}}
$$

#### **Secondary Metrics**
- **Perplexity**:  
  Perplexity evaluates how well a probabilistic model predicts masked tokens by measuring the uncertainty in its predictions. Lower perplexity indicates better performance, with the model assigning higher probabilities to the correct completions.
  
$$
\text{Perplexity} = \exp\left(-\frac{1}{N} \sum_{i=1}^{N} \log P(w_i | \text{context})\right)
$$
  
  This metric is critical for assessing probabilistic models' generalization capabilities across different contexts.

We will normalize and combine these metrics to get a single score for this task.
