# Home Depot Product Search Relevance
## Practical Deep Learning Workshop 2021- Word Embeddings and Word Level LSTM

### For this assigment we use kaggle dataeset - Home Depot Product Search Relevance

(https://www.kaggle.com/c/home-depot-product-search-relevance)

In this task we received a dataset containing information on query that users search and product description for each product in the website. In this task we Predict the relevance of search results on homedepot.com. For this purpose we will use regression models

Our task in this section is to predict the relevance of a particular search terms according to the product description - but in this section we will perform the word-level prediction.

During this part we will create a dictionary according to the tokens we will receive when we process the data. Our dictionary will contain a number of unique tokens. From these tokens we will create a word2vec model to represent each word in the search term as well as each word in the product description we have.

We will perform embedding process using the word2vec model for the words and create a Siamese model to predict the relevance - we will insert 2 inputs into the model:

The first input layer refers to the query itself - from the column "Search Terms"
The second input layer refers to the description of the product we intended - from the column "Product Description"
