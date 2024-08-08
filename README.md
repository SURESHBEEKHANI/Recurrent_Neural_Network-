# Recurrent Neural Network (RNN) for Text Generation

## Overview

This project demonstrates how to build and train a Recurrent Neural Network (RNN) using TensorFlow and Keras for generating text. The model is designed to predict the next word in a sequence based on a given input text.

## Components

1. **Data Loading and Preprocessing**

   - Data is loaded from a CSV file into a Pandas DataFrame.
   - The DataFrame is converted into a list of lists and flattened into a single list of sentences.
   - Text data is tokenized using TensorFlow's `Tokenizer` to convert words into integer sequences.
   - Sequences are padded to ensure uniform length.

2. **Model Architecture**

   - **Embedding Layer**: Converts integer sequences into dense vectors of a fixed size.
   - **Simple RNN Layer**: Processes the sequence data and retains temporal information.
   - **Dense Layer**: Outputs a probability distribution over the vocabulary using a softmax activation function.

3. **Model Training**

   - The data is split into features (input sequences) and targets (next words).
   - The model is compiled with the Adam optimizer and sparse categorical crossentropy loss function.
   - Training is conducted over 50 epochs with a validation split to monitor performance.

4. **Prediction**

   - A function is provided to generate predictions of the next word(s) given a seed text.
   - The function tokenizes and pads the seed text, uses the model to predict the next word, and updates the seed text with the predicted word.

## Results

- The model's performance is evaluated using accuracy and loss metrics. The trained model can generate text based on the provided seed text.

## Usage

- Ensure you have the required libraries installed (`TensorFlow`, `NumPy`, `pandas`).
- Prepare your text data in a CSV file named `data.csv`.
- Run the code to train the model and generate text based on a seed input.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contact

For any questions or feedback, please reach out to [SURESH BEEKHANI ](sureshbeekhani26@gmail.com)
