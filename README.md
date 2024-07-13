# Fine-Tuning BERT for Named Entity Recognition

## Introduction
This project focuses on fine-tuning BERT (Bidirectional Encoder Representations from Transformers) to tackle Named Entity Recognition (NER) tasks using the CoNLL-2003 dataset. NER is a fundamental task in Natural Language Processing (NLP) that involves identifying and categorizing key entities such as names, organizations, locations, and more within text data.

## Authors
- Lam Gia Phu - 21280104
- Tran Ngoc Khanh Nhu - 21280040

## Dataset
We utilize the CoNLL-2003 dataset, which is renowned for its comprehensive annotations of named entities in text. The dataset is split into:
- Training set: 14,041 rows
- Validation set: 3,250 rows
- Test set: 3,453 rows

## Methodology
1. **Tokenization**: Sentences are tokenized into subword units, ensuring that each token is appropriately labeled.
2. **Model Architecture**: 
   - **Embeddings**: Incorporates token, segment, and position embeddings.
   - **Transformer Layers**: Utilizes self-attention mechanisms and feed-forward neural networks.
   - **Output Layer**: Predicts labels for each token based on contextual embeddings.
3. **Training**: The model is trained with optimized hyperparameters, leveraging techniques such as grid search and early stopping to enhance performance.

## Results
Our fine-tuned BERT model achieved remarkable results, surpassing previous benchmarks:
- **Precision**: 94.54
- **Recall**: 95.23
- **F1-score**: 94.88

## Challenges
- **Ambiguity and Polysemy**: Addressing words with multiple meanings.
- **Entity Boundary Detection**: Correctly identifying the start and end of entities.
- **Variability and Synonymy**: Handling synonyms and varying entity representations.
- **Out-of-Vocabulary Words**: Managing words not seen during training.

## Future Work
1. **Nested Entities**: Investigating methods to recognize nested entities.
2. **Multilingual NER**: Expanding the model to support multiple languages.
3. **Context Recognition**: Enhancing the model's ability to understand longer sentences.

## Conclusion
This project demonstrates the efficacy of BERT in improving NER performance, setting new standards on the CoNLL-2003 dataset. Future research will explore domain adaptation and further hyperparameter optimization.

