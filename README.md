# Sentiment Analysis on Product Reviews

This project performs sentiment analysis on product reviews using natural language processing (NLP) and deep learning. The goal is to classify reviews as positive or negative by training a neural network model on labeled review data.

## Project Workflow

1. **Data Loading**: Load a labeled dataset of product reviews, where each review has a sentiment label (positive or negative).
  
2. **Data Preprocessing**:
   - Tokenize and pad the text data to prepare it for the neural network.
   - Save the `tokenizer` object to replicate tokenization for new reviews.

3. **Model Architecture**:
   - Build an LSTM-based neural network using Keras, with an embedding layer, dropout, and dense layers for classification.
   - Compile the model with `binary_crossentropy` as the loss function, `adam` optimizer, and accuracy as the evaluation metric.

4. **Model Training**:
   - Train the model on the training dataset with a validation split.
   - Save the best model during training to `amazon_model.keras` using `ModelCheckpoint`.

5. **Evaluation**:
   - After training, evaluate the model on test data.
   - Use a classification report and confusion matrix to assess performance.

6. **Comparison of Actual vs. Predicted**:
   - The notebook includes a section to compare actual and predicted values visually using a confusion matrix.
