# Human vs Machine Sentence Detection
This repository contains the implementation of a Natural Language Processing (NLP) task aimed at detecting whether a given sentence pair corresponds to human-written or machine-generated text. The task employs deep learning techniques to explore various approaches for tackling this challenge.

## Task Description
The primary goal of this project is to distinguish between human and machine-generated sentences by analyzing pairs of sentences (one human-written and the other machine-generated). The task leverages modern NLP methods, with a focus on transformer-based architectures, particularly BERT (Bidirectional Encoder Representations from Transformers).

## Baseline Study
Initially, a baseline study was conducted using an imbalanced dataset. This approach yielded poor results due to the imbalance, necessitating the exploration of more sophisticated models and techniques.

## Siamese Network Architecture
To address the challenges identified in the baseline study, a siamese network architecture was employed. This architecture processes pairs of human and machine sentences to determine their characteristics and differences.

## Key Features of the Siamese Network
- Transformer Encoder: The BERT-base-uncased model is used as the core feature extractor.
- Fine-tuning: Different fine-tuning configurations were explored, including:
  - Layer freezing to prevent overfitting and retain pre-trained knowledge.
- Paraphrase Analysis: A new test set was introduced to evaluate the model's performance in handling paraphrased sentences, ensuring robustness and correctness.

## Evaluation
The model's performance was evaluated using standard metrics and visualization techniques:

- **Confusion Matrix**: For analyzing classification performance and error patterns.

<img src="https://github.com/user-attachments/assets/7c04d44f-b9ce-404f-a596-c84749370a66" width="500">

- **Other Metrics**: Precision, recall, F1-score, and accuracy were used to quantify the model's effectiveness.

<img src="https://github.com/user-attachments/assets/398622e6-a889-44e8-ad63-75571bc86f61" width="700">

## Notebook
The implementation is contained in the provided Jupyter Notebook: SiamesaClassifier.ipynb, which includes:

- Data preprocessing and preparation.
- Model architecture and training configuration.
- Evaluation on baseline and paraphrased test sets.
- Results visualization and interpretation.
