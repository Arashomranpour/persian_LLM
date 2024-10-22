# Persian LLM

This repository contains work related to building and experimenting with Persian language models using HuggingFace. The aim is to explore large language models (LLMs) tailored for the Persian language, providing insights into fine-tuning, testing, and evaluation on Persian datasets.

## Files

- **huggingface.ipynb**: Jupyter notebook demonstrating the steps for loading, fine-tuning, and testing a Persian LLM using HuggingFace's transformers library.
- **test.txt**: A sample text file used for testing and evaluation.

## Requirements

- Python 3.x
- HuggingFace Transformers
- PyTorch or TensorFlow (based on backend)
- Jupyter Notebook

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/Arashomranpour/persian_LLM.git
   cd persian_LLM
2. install dependencies
   ```bash
  pip install transformers torch jupyter
3. open jupyter
  ```bash
  jupyter notebook huggingface.ipynb

## Usage
The notebook walks through the process of:

Loading a pretrained model from HuggingFace.
Fine-tuning the model on Persian text.
Evaluating the model using provided datasets.
