
# BERT - Based Text Classification

This repository contains a Python implementation of a BERT-based text classification model using TensorFlow and TensorFlow Hub.

## Features

- Uses **BERT** (Bidirectional Encoder Representations from Transformers) for text encoding.
- Leverages **TensorFlow Hub** for pre-trained BERT models.
- Implements a simple classifier on top of BERT's pooled output.
- Supports training, evaluation, and prediction on text data.

## Dependencies

Ensure that you have the following dependencies installed:
```bash
pip install tensorflow tensorflow-hub tensorflow-text
pip install matplotlib
```

## Model Architecture

The model consists of the following components:

1. **Preprocessing Layer**: Uses a TensorFlow Hub module for tokenization and input encoding.
2. **BERT Encoder**: A pre-trained BERT model from TensorFlow Hub.
3. **Classification Head**: A fully connected dense layer with a dropout for binary classification.


## Troubleshooting

- If encountering `ValueError: A KerasTensor is symbolic`, ensure that the correct TensorFlow functions are applied within the model.
- If encountering input shape mismatches, check that the input to the model is correctly formatted and preprocessed.


## Acknowledgments

- [TensorFlow Hub](https://www.tensorflow.org/hub) for pre-trained BERT models
- [BERT](https://arxiv.org/abs/1810.04805) for its foundational NLP advancements

