# Archaic vs Modern Azerbaijani NLP Evaluation

This project evaluates how well **multilingual transformer models** handle **historical language variation** by comparing **Classical Azerbaijani poetry** (16th century, *Məhəmməd Füzuli*) with their **modern Azerbaijani paraphrases**.

Using a manually curated parallel dataset of **50 real sentences** from *Leyli və Məcnun*, the project analyzes sentiment robustness and semantic understanding across time.

---

## Objectives

- Evaluate **sentiment classification robustness** on archaic language
- Measure **performance degradation** from modern to classical text
- Compare **XLM-RoBERTa** and **Multilingual BERT (mBERT)**
- Analyze **semantic embedding similarity** between archaic and modern forms

---

## Models Used

- **XLM-RoBERTa**
  - Encoder: `xlm-roberta-base`
  - Sentiment head: `cardiffnlp/twitter-xlm-roberta-base-sentiment`

- **Multilingual BERT (mBERT)**
  - Encoder: `bert-base-multilingual-cased`
  - Sentiment head: `cardiffnlp/bert-base-multilingual-cased-sentiment-multilingual`

---

## Evaluation Metrics

- Accuracy
- Precision / Recall / F1-score (macro, weighted)
- Sentiment label consistency (archaic ↔ modern)
- Cosine similarity of sentence embeddings

---

## Dataset

- **Source text:** *Leyli və Məcnun* (c. 1536), Məhəmməd Füzuli  
- **Language:** Classical Azerbaijani (Ottoman-Azeri literary language)
- **Status:** Public domain
- **Size:** 50 sentence pairs
- **Annotations:** Human-labeled sentiment (gold labels)

---

## Methodology

1. Run sentiment analysis on archaic and modern sentences
2. Compare predictions against gold labels
3. Measure sentiment consistency across forms
4. Compute embedding similarity using mean-pooled transformer embeddings

---
