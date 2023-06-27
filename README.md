# Inspirational Quote Generator using AI

This is a Colab notebook that demonstrates an Inspirational Quote Generator using AI. The notebook utilizes PyTorch, a popular deep learning library, to build and train a model capable of generating meaningful quotes based on a given input sequence.

## Features

- Imports necessary packages including PyTorch and its submodules (`torch.nn` and `torch.optim`).
- Loads and preprocesses a dataset of quotes from a CSV file (`data.csv`), creating a vocabulary of unique tokens and generating mapping dictionaries.
- Generates training examples by using a sliding window approach to create input sequences and corresponding target sequences.
- Defines a PyTorch module called `QuoteGeneratorModel` which consists of an embedding layer, an LSTM layer, and a fully connected layer.
- Trains the model on the training data using a custom PyTorch dataset and data loaders.
- Performs inference by generating quotes based on a given input sequence using beam search.

## Usage

1. Install the necessary packages by running the first code cell.
2. Load and preprocess the dataset by executing the code in the second code cell.
3. Generate training examples by running the code in the third code cell.
4. Define the `QuoteGeneratorModel` module by executing the fourth code cell.
5. Train the model by running the code in the fifth code cell. Note that training may take a long time if using a CPU, so a GPU runtime is recommended.
6. Perform inference and generate quotes by executing the code in the sixth code cell. Adjust the input parameters `text`, `seed`, and `max_length` as desired.

## Requirements

- Python 3.x
- PyTorch (and the dependencies of it)

## Dataset

The dataset used in this notebook is a CSV file (`data.csv`) containing a list of quotes. The file has been sourced from a Kaggle dataset ([Goodreads Quotes](https://www.kaggle.com/datasets/abhishekvermasg1/goodreads-quotes)) and has been renamed from its original name (`quotes.csv`).

Please make sure to download the dataset and place it in the same directory as the notebook before running the code.

## Acknowledgments

- The model architecture and training code in this notebook are for demonstration purposes and may require further optimization for improved performance and results.
- The dataset used is for illustrative purposes only and may not be suitable for production use.
- This notebook is provided as-is and is not intended for commercial or production use.
