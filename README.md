Part A – Dataset Preparation and Text Preprocessing

In Part A, the IMDB Movie Reviews dataset is loaded using TensorFlow/Keras for sentiment analysis. The dataset contains positive and negative movie reviews. The number of training and testing samples and sentiment class distribution are examined. The reviews are converted into numerical sequences using a tokenizer, and a vocabulary of 10,000 words is used. The sequences are padded to a maximum length of 200 so that all reviews have the same length. The sentiment labels are represented as 0 for negative and 1 for positive. Finally, the prepared training data is divided into training and validation datasets.

Part B – Embedding Generation

In Part B, an Embedding layer is created using Keras to convert the numerical text sequences into dense vector representations. A vocabulary size of 10,000 and an embedding dimension of 64 are used. The embedding layer converts every token into a 64-dimensional vector. The padded sequences are passed through the Embedding layer, producing an embedding representation with the shape of (20000, 200, 64). This representation helps the model learn relationships and similarities between words during training.

Part C – Implementing the LSTM Model

In Part C, an LSTM-based sentiment classification model is created using TensorFlow and Keras. The model consists of an Embedding layer, an LSTM layer with 64 units, and a Dense output layer with a sigmoid activation function. The Embedding layer converts the input tokens into dense vectors, while the LSTM layer learns the sequential dependencies and context of the movie reviews. The Dense layer produces the final sentiment prediction, where 0 represents negative sentiment and 1 represents positive sentiment. The model is compiled using the Adam optimizer, binary cross-entropy loss, and accuracy as the evaluation metric. The model architecture is displayed using the model summary.

Part D – Model Training and Sentiment Prediction

In Part D, the LSTM model is trained using the prepared training dataset and validated using the validation dataset. The model is trained for multiple epochs and the training accuracy, validation accuracy, training loss, and validation loss are recorded. Accuracy versus epoch and loss versus epoch graphs are generated to visualize the model performance. The trained model is then evaluated using the test dataset. Accuracy, precision, recall, F1-score, and confusion matrix are calculated to measure the model's performance. Finally, sample movie reviews are given to the trained model to predict whether the sentiment is positive or negative. The results demonstrate the use of LSTM for sentiment classification of movie reviews.

# 24ADI006_RAMYA-R-_24BAD096_EX_6
