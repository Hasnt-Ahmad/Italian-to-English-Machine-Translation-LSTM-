# Italian-to-English-Machine-Translation-LSTM

This project implements a machine translation model to convert Italian sentences into English using a sequence-to-sequence (seq2seq) architecture with LSTM layers in Keras. The model is designed to translate text efficiently while handling common challenges such as vocabulary size and sequence padding.

****Key Features:****

  ****1. Data Preprocessing: **** The text data is cleaned by removing punctuation and converting the text to lowercase. Tokenization and padding are applied to prepare the sequences for model input.

  ****2. Tokenization:****  Separate tokenizers are created for the Italian and English texts, converting words to sequences of integers and handling large vocabularies.

  ****3. Model Architecture:****
        i.The model includes an embedding layer for input sequences.
        ii.LSTM layers are used to capture temporal dependencies in the text.
        ii.The model architecture incorporates a RepeatVector layer to repeat the encoded vector across the output sequence.
        
  ****4. Training:**** The model is trained with an RMSprop optimizer and uses checkpoints and early stopping to save the best model during training.
  
  ****4. Prediction: ****  The trained model predicts the English translations for the Italian text, and the results are processed to generate coherent and accurate translations.

****How to Use: ****
  ****1. Dataset: **** Load and preprocess the Italian-English sentence pairs from the provided text file.
  ****2. Model Training: **** Train the model on the dataset, with options for validation and early stopping.
  ****3. Prediction: **** Use the trained model to predict English translations for new Italian sentences.

****Dependencies: ****
    TensorFlow/Keras
    NumPy
    Pandas
    Matplotlib
