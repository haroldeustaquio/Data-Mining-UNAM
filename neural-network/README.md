# Seq2Seq Model for Harry Potter Books

## Overview
This project implements a sequence-to-sequence (seq2seq) model using PyTorch, designed to generate text based on input sequences derived from the Harry Potter series. The model comprises an Encoder-Decoder architecture, where the Encoder processes the input sequences, and the Decoder generates the output sequences. 

Additionally, a word embedding technique is applied to capture semantic relationships between words used in the series.

---

## Project Structure
- **Data Processing**: The project processes text from the Harry Potter books to create input-output pairs suitable for training the seq2seq model. It tokenizes the text and constructs a vocabulary.
- **Model Architecture**:
  - **Encoder**: Encodes the input sequence and generates a hidden state.
  - **Decoder**: Decodes the hidden state to produce the output sequence.
  - **Seq2Seq**: Integrates both the Encoder and Decoder into a single model for end-to-end training.

---

## Implementation Steps
1. **Data Preparation**: Text from multiple Harry Potter books is read and tokenized, generating pairs of input and output sequences.
2. **Vocabulary Construction**: A vocabulary is built based on the frequency of words, ensuring a minimum frequency threshold to filter out less common words.
3. **Model Training**: The model is trained using a loss function optimized for sequence generation tasks.
4. **Word Embeddings**: Word embeddings are extracted for selected words to visualize and analyze their semantic relationships.

---

## Requirements
To run this project, ensure you have the following libraries installed:
- PyTorch
- Torchtext
- Keras
- Matplotlib
- scikit-learn

You can install the required libraries using:
```bash
pip install torch==2.3.1 torchvision==0.18.1 torchaudio==2.3.1 --index-url https://download.pytorch.org/whl/cu121
pip install torchtext==0.18
```