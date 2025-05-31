# Balanced Adult Dataset – Split Version

This repository provides a **balanced version** of the UCI Adult (Census Income) dataset, split into training, validation, and test sets. The dataset was prepared for experiments in **tabular classification**, and is used to benchmark both classical machine learning models and fine-tuned language models.

## Description

The original UCI Adult dataset is a binary classification dataset that predicts whether an individual's income is greater than \$50,000 per year based on demographic and occupational features.

In this version:
- The dataset was **balanced** to ensure an equal number of examples from each income class (`>50K` and `<=50K`).
- The data was split into:
  - `train_data.csv` — for training
  - `validation_data.csv` — for model tuning
  - `experiment_data.csv` — for final evaluation

Each CSV file contains features such as:
- Age  
- Workclass  
- Education  
- Marital status  
- Occupation  
- Race  
- Gender  
- Hours per week  
- Native country  
- Income (target)

## Use Cases

This dataset was used in two distinct modeling approaches:

1. **Gradient Boosted Trees (GBT)**  
   - Applied directly on the tabular features after preprocessing (e.g., encoding categorical features).
   - Used as a baseline for robustness comparison.

2. **RoBERTa (Transformer-based LLM)**  
   - Each row was converted into a pseudo-sentence of the form:  
     `"age: 39, education: Bachelors, gender: male, ..., income: <mask> than 50,000"`
   - The model was fine-tuned to predict whether the masked token is `greater` or `less`.

## Files

| File                  | Description                      |
|-----------------------|----------------------------------|
| `train_data.csv`      | Training data (balanced)         |
| `validation_data.csv` | Validation set                   |
| `experiment_data.csv` | Test set for evaluation          |

## Related Project

This dataset supports the final project:

**[Adversarial Attack on Tabular Classification](https://github.com/yuvalira/Final-Project-Adversarial-Attack-on-Tabular-Classification/tree/main)**  
Where we evaluate and compare the robustness of RoBERTa vs. GBT under adversarial conditions.

## Authors

- [ETdanR](https://huggingface.co/ETdanR)  
- [yuvalira](https://huggingface.co/yuvalira)
