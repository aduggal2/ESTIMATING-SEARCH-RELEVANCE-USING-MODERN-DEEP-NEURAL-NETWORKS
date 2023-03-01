# ESTIMATING-SEARCH-RELEVANCE-USING-MODERN-DEEP-NEURAL-NETWORKS

Many websites have search functionality to allow users to search for various documents, such as products, user posts, and text articles. It is important to suggest **semantically relevant** documents to users. 

Dataset Link: https://www.kaggle.com/competitions/home-depot-product-search-relevance/data

The data is spread across three main datasets: train, product descriptions, and attributes.

The goal of this project is to predict the relevance score given product information and search term. The relevance score describes how relevant a product is to the given search term. 

The task involves training various neural network models, including** Bidirectional LSTM, One-dimensional Convolution, Attention Mechanism, and Transformer-based models such as BERT**, to solve the problem. 

Then evaluating each of the models using **RMSE** as a metric. It is also important to consider the time taken to predict the relevance as a constraint while evaluating models.

The dataset was preprocessed to eliminate words that did not provide much useful information and tokenize the words. 

Stop words were also removed, and lemmatization was performed on the words using nltk’s WordNetLemmatizer class. 

Features were extracted from the dataset, including the length of titles, search terms, and descriptions, and the vocabulary length of the product titles, product description, product attributes, and the search query. 

Text encoding was used to convert meaningful text into number/vector representation using Keras tokenization method fit to texts().

The **result** of the project is a model that can predict the relevance score given product information and search term. The models were evaluated using RMSE as a metric, and the time taken to predict the relevance will also be considered as a constraint. The model will suggest semantically relevant documents to users, which will improve the user experience on websites.

Until now some good RMSE score of 0.488 from Bidirectional LSTM which has taken the least time of 0.177 was achieved
