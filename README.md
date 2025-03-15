# Tamil-Multi-Class-Text-Classification
This project focuses on classifying Tamil text into different categories using a combination of deep learning and ensemble techniques. It involves preprocessing the text data, training various models, and evaluating their performance to achieve optimal classification accuracy.


## Dataset

The project utilizes a Tamil text dataset sourced from your Google Drive. The dataset consists of text samples with corresponding category labels. These labels are encoded numerically for model training.

## Preprocessing

The following preprocessing steps are performed on the text data:

1. **Cleaning:** Removes special characters, punctuation, and numbers from the text.
2. **Tokenization:** Splits the text into individual words or tokens.
3. **Stop Word Removal:** Filters out common Tamil stop words to reduce noise and improve model efficiency.

## Models

This project employs various deep learning and ensemble models:

1. **Word Embeddings:** Leverages pre-trained FastText word embeddings (`wiki.ta.vec`) to represent Tamil words as numerical vectors, enabling the models to capture semantic meaning.

2. **Deep Learning Models:**
    - **LSTM:** A Long Short-Term Memory network, an RNN architecture adept at processing sequential data like text.
    - **Hybrid Models:** Combines different model architectures to enhance performance.
        - **LSTM + GRU:** Stacks an LSTM layer with a GRU (Gated Recurrent Unit) layer for capturing both long-term and short-term dependencies in the text.
        - **CNN + GRU:** Uses a Convolutional Neural Network (CNN) to extract local features and a GRU to capture sequential information.

3. **Meta Models:** Combines predictions from base models to improve overall accuracy.
    - **Random Forest:** An ensemble method that aggregates predictions from multiple decision trees.
    - **Decision Tree:** A tree-based model that learns decision rules from the data.
    - **Logistic Regression:** A linear model used for classification.


## Evaluation

Model performance is evaluated using metrics such as accuracy, precision, recall, and F1-score. The results are compared to identify the best-performing model for Tamil text classification.

## Usage

1. Open the provided Google Colab notebook.
2. Mount your Google Drive to access the dataset and necessary files.
3. Execute the code cells sequentially to preprocess data, train models, and evaluate their performance.
4. Modify model parameters and experiment with different configurations for potential performance improvements.
