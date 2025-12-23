# Adaptive Taxonomy Mapper

A semantic similarity-based approach to mapping story snippets to a precise fiction taxonomy. This system prioritizes the semantic content of a story over user-provided tags, ensuring more accurate categorization for platform-scale content.

## 🚀 Overview

Traditional rule-based or tag-based classification systems often fail when users provide misleading or broad tags. This project implements an **Adaptive Taxonomy Mapper** that uses:
- **Sentence Embeddings**: Capturing deeper semantic meaning beyond simple keywords.
- **Cosine Similarity**: Calculating the closeness between story content and genre definitions.
- **Dynamic Reasoning**: Explaining *why* a category was chosen by highlighting high-contribution words.

## ✨ Key Features

- **Semantic Alignment**: Uses `all-MiniLM-L6-v2` to map stories to 12 distinct fiction sub-genres.
- **Explainable AI**: Provides word-level contribution scores for every classification.
- **Robust Unmapping**: Naturally handles out-of-domain (non-fiction) content using a semantic threshold.
- **Scalable Design**: Easily extensible to larger taxonomies or multi-label classification.

## 🛠️ Tech Stack

- **Language**: Python
- **Libraries**: `sentence-transformers`, `numpy`, `scikit-learn`
- **Environment**: Jupyter Notebook / Python Script

## 📊 Results

The model successfully handles:
- **Direct Matches**: Clear genre alignment (e.g., Slasher, Gothic).
- **Ambiguous Cases**: Correctly identifying the "true" genre when tags are misleading.
- **Irrelevant Content**: Filtering out recipes or technical guides via the similarity threshold.

## ⚙️ Installation

```bash
pip install -r requirements.txt
```

## 📖 Usage

Run the `adaptive_taxonomy_mapper.ipynb` notebook to see the full implementation and evaluation on 10 diverse test cases.

---
**Author**: Nikhil Jose
**GitHub**: [nikhiljose7](https://github.com/nikhiljose7)
