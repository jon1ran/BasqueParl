# Political Speech Analysis Project

## Overview

This project focuses on analyzing political speeches from the Basque parliament using natural language processing (NLP) techniques. The goal is to uncover latent topics within the speeches and analyze their distribution over time, across political parties, and by speaker gender.

## Dataset

The dataset used for this project is the **Basqueparl** dataset, which includes bilingual transcriptions from the Basque Autonomous Community Parliament spanning from December 3, 2012, to February 7, 2020.

## Methodology

### Data Preprocessing

1. **Lemmatization**: Reducing words to their root forms to minimize dimensionality.
2. **Stopword Removal**: Eliminating common words that do not contribute to topic analysis.
3. **Collocation Identification**: Detecting and replacing common word pairings to capture more complex lexical relationships.

### Topic Modeling

- **Latent Dirichlet Allocation (LDA)**: An unsupervised machine learning algorithm used to discover hidden topics in a set of documents. Three different LDA models were developed to compare the effects of different parameter configurations:
  - **Model 1**: 30 topics, focusing on words appearing in less than 60% of documents and at least 300 times.
  - **Model 2**: 40 topics, with words appearing in less than 60% of documents and at least 150 times.
  - **Model 3**: 40 topics, with words appearing in less than 60% of documents and at least 300 times.

### Evaluation

- The models were evaluated based on the interpretability and intuitive sense of the identified topics, as the dataset lacks labeled data for quantitative evaluation.
- Topics were analyzed for their distribution across different years, political parties, and speaker genders.

## Results

- Visualized the evolution of topics over time and identified key thematic areas for different political parties and speaker genders.
- Highlighted the importance of health in 2020 due to the COVID-19 pandemic.
- Demonstrated variations in topics discussed by different political parties and genders.

## Technologies and Libraries Used

- **Python**
- **Natural Language Toolkit (nltk)**
- **Gensim** for topic modeling
- **pandas** and **numpy** for data manipulation
- **matplotlib** and **seaborn** for data visualization
- **Jupyter Notebook** for interactive data analysis
