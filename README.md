# Transformer-Based Next-Token Prediction Using Self-Attention

## Project Overview

This project implements a Transformer-based next-token prediction model using Python, TensorFlow, and Keras. It uses basic self-attention to learn relationships between words and predict the next word in a sequence.

## Objectives

- Understand next-token prediction in Natural Language Processing (NLP).
- Convert text into numerical tokens using a tokenizer.
- Create input sequences and their next-token targets.
- Build a Transformer-style model using multi-head self-attention.
- Train the model and visualize accuracy and loss.
- Predict the next word for sample text inputs.

## Technologies Used

- Python
- NumPy
- TensorFlow
- Keras
- Matplotlib

## Dataset

The project uses a small, manually created dataset containing 14 sentences related to deep learning, machine learning, neural networks, transformers, and artificial intelligence.

No external dataset download is required.

## Model Architecture

1. **Embedding Layer:** Converts token IDs into 32-dimensional vectors.
2. **Multi-Head Attention:** Uses two attention heads to learn relationships between tokens.
3. **Causal Mask:** Prevents attention to future tokens.
4. **Layer Normalization:** Helps stabilize training.
5. **Dropout:** Uses a dropout rate of 0.1.
6. **Feed-Forward Network:** Contains dense layers with 64 units and ReLU activation, followed by a projection layer.
7. **Output Layer:** Uses softmax to predict the next token from the vocabulary.

## Training Configuration

- Optimizer: Adam
- Loss Function: Sparse Categorical Cross-Entropy
- Evaluation Metric: Accuracy
- Number of Epochs: 100
- Batch Size: 16
- Embedding Dimension: 32
- Number of Attention Heads: 2

## Project Workflow

1. Import the required libraries.
2. Create the sample text dataset.
3. Tokenize the text and build the vocabulary.
4. Generate input and next-token target pairs.
5. Pad sequences to a consistent length.
6. Build the Transformer model with self-attention.
7. Compile and train the model.
8. Plot training accuracy and loss.
9. Predict the next token for sample prompts.
10. Display the prediction results.

## Installation

Install the required dependencies:

```bash
pip install numpy tensorflow matplotlib
```

## How to Run

1. Open `Untitled23 (1).ipynb` in Google Colab or Jupyter Notebook.
2. Run the notebook cells from top to bottom.
3. Review the vocabulary and model summary.
4. Observe the training accuracy and loss graphs.
5. Check the predicted next tokens for the sample inputs.

## Sample Inputs

- `deep learning`
- `machine learning`
- `neural networks`
- `artificial intelligence`

The predicted words may vary depending on training and model initialization.

## Output

The notebook displays:

- Vocabulary size and word-index mapping
- Input and target array shapes
- Model architecture summary
- Training accuracy graph
- Training loss graph
- Predicted next tokens for the sample inputs

## Limitations

- The dataset contains only 14 sentences.
- The notebook does not use a separate validation or test dataset.
- The model has a limited vocabulary and is intended for educational purposes.

## Future Enhancements

- Train using a larger text dataset.
- Add positional embeddings.
- Include validation and test datasets.
- Implement top-k next-token predictions.
- Save the trained model for future use.
