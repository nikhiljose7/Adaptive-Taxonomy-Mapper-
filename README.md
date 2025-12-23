# Adaptive Taxonomy Mapper

A semantic similarity-based approach to mapping story snippets to a precise fiction taxonomy. This system prioritizes the semantic content of a story over user-provided tags, ensuring more accurate categorization for platform-scale content.

## Overview

Traditional rule-based or tag-based classification systems often fail when users provide misleading or broad tags. This project implements an Adaptive Taxonomy Mapper that uses:
- **Sentence Embeddings**: Capturing deeper semantic meaning beyond simple keywords.
- **Cosine Similarity**: Calculating the closeness between story content and genre definitions.
- **Dynamic Reasoning**: Explaining the classification by highlighting high-contribution words.

## Key Features

- **Semantic Alignment**: Uses the `all-MiniLM-L6-v2` model to map stories to 12 distinct fiction sub-genres.
- **Explainable AI**: Provides word-level contribution scores for every classification decision.
- **Robust Unmapping**: Handles out-of-domain content (such as non-fiction) using a semantic threshold.
- **Scalable Design**: Extensible to larger taxonomies or multi-label classification tasks.

## Tech Stack

- **Language**: Python
- **Core Libraries**: `sentence-transformers`, `numpy`, `scikit-learn`
- **Interface**: Jupyter Notebook

## Results

The system is evaluated against diverse test cases to demonstrate its performance in:
- **Direct Matches**: Clear alignment with specific genre definitions.
- **Ambiguous Cases**: Identifying correct genres even when user tags are misleading.
- **Out-of-Domain Detection**: Correctly filtering non-fiction or irrelevant content.

## Installation

```bash
pip install -r requirements.txt
```

## Usage

Run the `adaptive_taxonomy_mapper.ipynb` notebook to see the implementation, evaluation, and reasoning logs.

---
**Author**: Nikhil Jose
**GitHub**: [nikhiljose7](https://github.com/nikhiljose7)
