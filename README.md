# Inspirational Quote Generator

Welcome to this Inspirational Quote Generator! This repository contains a Colab notebook that demonstrates the generation of meaningful quotes using AI. The project uses PyTorch, a powerful deep-learning library, to train a model capable of generating inspiring quotes based on a given input sequence.

## Key Features

- Importing essential packages, including PyTorch and its submodules (`torch.nn` and `torch.optim`).
- Loading and preprocessing a dataset of quotes from a CSV file (`data.csv`), creating a vocabulary of unique words, and generating mapping dictionaries.
- Generating training examples by using a sliding window approach to create input sequences and corresponding target sequences.
- Defining a PyTorch module called `QuoteGeneratorModel`, which includes an embedding layer, an LSTM layer, and a fully connected layer.
- Training the model on the training data using a custom PyTorch dataset and data loaders.
- Performing inference by generating quotes based on a given input sequence using beam search.

## How to Use

Follow the steps below to use this Inspirational Quote Generator:

1. Install the required packages by running the first code cell.
2. Load and preprocess the dataset by executing the code in the second code cell.
3. Generate training examples by running the code in the third code cell.
4. Define the `QuoteGeneratorModel` module by executing the fourth code cell.
5. Train the model by running the code in the fifth code cell. Note that training may take a while if using a CPU, so it is recommended to use a GPU runtime.
6. Perform inference and generate quotes by executing the code in the sixth code cell. Adjust the input parameters `text`, `seed`, and `max_length` as desired.

## Requirements

To run this project, you need:

- Python 3.x
- PyTorch (and its dependencies)
- At least 8 GB of RAM
- (Optional) A GPU for faster training and inference
- `data.csv` in the same folder as the notebook

## Dataset

The dataset used in this project is a CSV file (`data.csv`) containing a collection of quotes. The file has been sourced from a Kaggle dataset called [Goodreads Quotes](https://www.kaggle.com/datasets/abhishekvermasg1/goodreads-quotes) and has been renamed from its original name (`quotes.csv`).

Before running the code, please download the dataset and place it in the same directory as the notebook.

## License

The code in this notebook is licensed under the Apache License 2.0.

## How to Contribute

I appreciate your interest in contributing to this project! To contribute, please follow these steps:

1. Fork the repository on GitHub.
2. Make the desired changes and improvements.
3. Submit a pull request explaining your changes.

Please ensure that your contributions adhere to the coding style of the project. I value and appreciate any help you provide!

## Acknowledgments

- The model architecture and training code in this notebook are for demonstration purposes and may require further optimization for improved performance and results.
- The dataset used is for illustrative purposes only and may not be suitable for production use.
- This notebook is provided as-is and is not intended for commercial or production use.
