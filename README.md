# Character-Level Language Modeling with LSTM

An educational Jupyter Notebook exploring character-level text generation using Long Short-Term Memory (LSTM) networks implemented in PyTorch.

Developed as part of the **Large Language Models and Applications** graduate course (BİL 822).

## Overview

This notebook demonstrates how an LSTM learns sequential patterns from Turkish text and generates new characters based on previously observed sequences.

The primary goal is to understand LSTM behavior through practical experiments rather than to develop a production-ready language model.

## Experiments

### Experiment 1: Learning from a Small Corpus

- Train a character-level LSTM on a short, repeated Turkish text.
- Observe text generation at different training steps.
- Explore how the model learns character sequences.
- Examine the limitations of training on a small and repetitive dataset.

### Experiment 2: Training on a More Diverse Corpus

- Train a second LSTM using a larger and more varied Turkish text.
- Split the corpus into training and validation sections.
- Compare training and validation losses.
- Evaluate next-character prediction on an independent text.
- Visualize the model's probability distribution for the next character.
- Examine the generalization gap and potential overfitting.

## Model Architecture

The model uses:

- Character embeddings (64 dimensions)
- Two-layer LSTM (256 hidden units)
- Dropout (0.2)
- Linear output layer
- Cross-entropy loss
- Adam optimizer

## Technologies

- Python
- PyTorch
- Jupyter Notebook / Google Colab
- Matplotlib

## Running the Notebook

1. Open the notebook in Google Colab or a local Jupyter environment.
2. Install the dependencies listed in `requirements.txt` if necessary.
3. Run the cells sequentially.
4. Observe the generated text, loss values, and visualizations.

The experiments can run on a CPU, although training time depends on the available hardware.

## Key Observations

- Character-level LSTMs can learn local patterns and sequential dependencies in text.
- Repetitive training data can lead to memorization-like behavior.
- Low training loss does not necessarily imply good generalization.
- Comparing training, validation, and independent test behavior helps reveal model limitations.
- Next-character probabilities provide insight into how text generation works.

## Limitations

This notebook is intended for educational experimentation. It uses relatively small, manually prepared text corpora and does not aim to produce a general-purpose language model.

The validation and test results should be interpreted as exploratory observations rather than comprehensive benchmarks.

## Authors

Öznur Yakut and Büşra Kurun

**Academic coursework — BİL 822: Large Language Models and Applications**
