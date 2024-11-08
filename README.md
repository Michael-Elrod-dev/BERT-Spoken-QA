# BERT-Spoken-QA

This project implements a Question Answering (QA) system using BERT-based models on the Spoken-SQuAD dataset for extractive question answering tasks.

## Dataset
Spoken-SQuAD dataset characteristics:
- Training set: 37,111 question-answer pairs (WER 22.77%)
- Testing set: 5,351 pairs (WER 22.73%)
- Additional test sets with added noise levels (WER 44.22% and 54.82%)

## Implementation

### Base Model
- DistilBERT for Question Answering
- Basic tokenization and preprocessing
- Configuration:
 - Batch size: 16
 - Learning rate: 2e-6
 - Epochs: 10
 - Optimizer: AdamW

### Improvements
- Linear learning rate decay implementation
- Enhanced preprocessing pipeline
- Improved postprocessing with AnswerEvaluator
- Extended training to 30 epochs

## Requirements
- Python 3
- PyTorch
- Transformers
- tqdm
