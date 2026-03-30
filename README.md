# Do polarity-based sentiment models flatten engaged-negative user feedback?
### A study of Facebook app reviews

This repository contains the code, notebooks, and final report for Group 18's MSIN0221 Natural Language Processing project.

Our project looks at whether polarity-based sentiment models can distinguish between two types of negative feedback in Facebook app reviews:

- **Engaged-Negative (EN):** reviews that express dissatisfaction while also showing signs of continued use, persistence, re-entry, or dependency
- **Pure-Negative (PN):** reviews that express dissatisfaction without those engagement-related cues

The project combines a rule-based classification approach with benchmarking across several sentiment analysis systems.
---

## Data

The dataset used in this project is from Kaggle: https://www.kaggle.com/datasets/ashishkumarak/play-store-reviews-facebook 

Because the original CSV file is too large for standard GitHub storage, it is not included in this repository.

To reproduce the analysis:

1. Download the dataset from Kaggle
2. Rename the file as `facebook_reviews.csv`
3. Place it in the project root directory

The analysis assumes that the CSV file is stored in the same directory as the notebooks.
---

## Research Question

Our central research question is:

**Do polarity-based sentiment models flatten engaged-negative feedback into a broadly undifferentiated negative category?**

To answer this, we:
1. cleaned and filtered a large corpus of Facebook app reviews,
2. operationalised negative markers and engagement-related cues,
3. constructed EN and PN sub-corpora, and
4. benchmarked multiple sentiment models on these two subsets.
---

## Environment Setup

This project was developed in Python using Jupyter Notebook.

Recommended packages include:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scipy`
- `openai`

You can install the core dependencies with:

```bash
pip install pandas numpy matplotlib seaborn scipy
