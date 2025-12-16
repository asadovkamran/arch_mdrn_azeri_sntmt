# arch_mdrn_azeri_sntmt
Evaluating multilingual NLP models on archaic Azerbaijani poetry by comparing sentiment classification and embedding similarity between Classical (Füzuli) and modern paraphrases.

This project evaluates how well multilingual transformer models handle historical language variation by comparing Classical Azerbaijani poetry (16th century, Məhəmməd Füzuli) with their modern Azerbaijani paraphrases.

Using a manually curated parallel dataset of 50 real sentences from Leyli və Məcnun, the project analyzes:

Sentiment classification robustness

Precision, recall, and F1-score degradation

Label consistency between archaic and modern forms

Semantic embedding similarity (cosine similarity)

The goal is to measure how linguistic archaism affects semantic understanding in modern multilingual NLP models.

XLM-RoBERTa
(xlm-roberta-base + sentiment fine-tuning)

Multilingual BERT (mBERT)
(bert-base-multilingual-cased + sentiment fine-tuning)
