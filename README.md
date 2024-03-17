# News Article Classification using LSTM

This project aims to classify news articles into real and fake categories using a Long Short-Term Memory (LSTM) neural network. The dataset consists of news articles stored in a CSV file with features such as article titles, authors, text content, and labels indicating whether the article is real or fake news.

## Data Preprocessing

The CSV file containing the news articles is loaded using pandas, and any rows with missing values are dropped. The text data is preprocessed by removing special characters, converting text to lowercase, removing stopwords, and stemming the words using NLTK.

## Model Building

The text data is converted into numerical form using one-hot encoding. An LSTM model is constructed using Keras with an Embedding layer, LSTM layer, and a Dense layer with sigmoid activation for binary classification. The model is compiled using binary cross-entropy loss and the Adam optimizer.

## Training the Model

The dataset is split into training and testing sets using sklearn's train_test_split function. The model is trained on the training data and evaluated on the testing data over multiple epochs.

## Results

The LSTM model achieves an accuracy of approximately 91.47% on the testing data. Confusion matrix analysis reveals that the model performs well in correctly classifying both real and fake news articles.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

