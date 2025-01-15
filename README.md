# Stanford Ribonanza RNA Folding
### Kaggle Competition: Top 39%
This repository highlights my approach to RNA folding prediction in the Stanford Ribonanza competition. The goal was to build a machine learning model to predict RNA reactivity values using transformer-based architectures while addressing challenges like longer sequence generalization and effective feature engineering.


## Key Features

- Transformer Model: Custom encoder-only transformer with 12 layers and 192 hidden dimensions.

- Alibi Embedding: Integrated Attention with Linear Biases (ALiBi) to improve generalization for longer sequences.

- BPP Feature Injection: Enhanced model performance by injecting Base Pair Probability (BPP) features directly into the transformer.

- Data Processing: Developed pipelines for sequence length handling, masking, and normalization.

- Generalization Focus: Improved performance on test data with much longer sequences than the training set.

## Challenges


- Generalization to Longer Sequences:

Training sequences maxed at 197, while private leaderboard sequences exceeded 500.

Implemented ALiBi for better generalization but faced high computational costs.


- Feature Engineering:

Injecting BPP features proved more effective and computationally efficient than ALiBi.

## Key Takeaways


Transformers excel at sequence prediction tasks.

Domain-specific features like BPP significantly boost performance.

Simpler, resource-efficient solutions often outperform computationally heavy methods.

## Insights

Improving data representation before attention mechanisms is crucial.

Injecting meaningful features is both efficient and effective for limited-resource scenarios.

Generalization to longer sequences requires architectural enhancements combined with robust preprocessing.


## Conclusion

This project underscores the value of combining cutting-edge ML techniques with domain-specific insights. The lessons learned can guide future RNA folding prediction and BioAI research efforts.



## Data
RNA data is hosted on [Kaggle RNA Folding Dataset](https://www.kaggle.com/c/stanford-ribonanza-rna-folding/data).
