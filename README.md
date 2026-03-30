# NLP Sentiment Analysis with TF-IDF (SST-2)

Machine learning project focused on sentiment analysis of movie reviews using a TF-IDF-based approach and manual feature tuning.

## Overview

This project explores sentiment classification within Natural Language Processing (NLP) using the SST-2 dataset. The goal is to classify movie reviews as **positive** or **negative** and investigate whether manual adjustment of word importance can improve model performance.

## Objectives

* Build a sentiment classifier using TF-IDF features
* Analyze model performance on movie review data
* Experiment with manual word-weight adjustments
* Evaluate the impact of linguistic features like negation

## Dataset

* **Name:** SST-2 (Stanford Sentiment Treebank)
* **Source:** Hugging Face (Stanford NLP)
* **Data Splits** Number of examples = train 67349; validation	872; test	1821.
* **Labels:** Binary (0 = negative, 1 = positive)

## Methodology

* Feature extraction using **TF-IDF (Term Frequency – Inverse Document Frequency)**
* Machine learning-based classification (supervised learning)
* Experiments included:
  * Expanding vocabulary size
  * Using n-grams (word clusters instead of single tokens)
  * Manual adjustment of word weights
  * Analysis of uncertain predictions

## Results

* Initial accuracy: **79.13%**
* After improvements: **79.54%**

### Key Findings

* TF-IDF effectively captures sentiment-heavy words (e.g., *"fantastic", "beautiful"*)
* Model struggles with **negation handling** (e.g., *"not bad"*)
* High-dimensional feature space (62,753 features) limits the impact of small manual adjustments
* Manual tuning can improve specific edge cases but not overall performance significantly

## Insights

* Machine learning approaches outperform rule-based methods in capturing context
* Negation remains a major challenge in sentiment analysis
* Feature engineering (e.g., n-grams) improves contextual understanding

##  Project Structure

```
NLP_Sentiment_Analysis/
│── data/
│── notebooks/
│── src/
│── README.md
```

## Getting Started

```bash
# Clone the repository
git clone https://github.com/luizoquadros-lang/NLP_Sentiment_Analysis.git

# Navigate into the project
cd NLP_Sentiment_Analysis

# Install dependencies
pip install -r requirements.txt
```

## Usage

Run the main script or notebook to train and evaluate the model:

```bash
python main.py
```

## 👥 Authors

* Luiz Otavio de Quadros
* Mengqi Liu
* Nur Rodríguez Boada

## 📚 References

* Socher et al. (2013) – SST-2 Dataset
* Das & Chakraborty (2018) – Sentiment Classification
* Basarslan & Kayaalp (2020) – ML for Sentiment Analysis

---

⭐ If you found this project useful, consider giving it a star!
