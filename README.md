# Protein Stability Prediction with DistilProtBERT

This project uses a distilled version of ProtBert (DistilProtBert) to predict protein stability scores. We fine-tune the pre-trained model on a subset of the [proteinglm/stability_prediction](https://huggingface.co/datasets/proteinglm/stability_prediction) dataset using Hugging Face’s Trainer API.

## Overview

- **Dataset:** Protein stability prediction dataset with protein sequences and their stability scores.
- **Data Subset:** Randomly selected 10,000 training examples, 500 validation examples, and 5,000 test examples.
- **Model:** DistilProtBert with a custom regression head.
- **Training:** Fine-tuning with Hugging Face's Trainer API, logging training/validation loss and Mean Squared Error (MSE).

## Setup

1. Install dependencies:
   ```bash
   !pip install transformers torch datasets scikit-learn
