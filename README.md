# Word-Embeddings-Text-representation-_-Word2vec-NLP-
This project uses Word2Vec to analyze semantic relationships in "A Game of Thrones." It preprocesses text, trains a Word2Vec model, and explores word similarities. Visualization via PCA reveals clusters of related words in 3D space, offering insights into character dynamics and themes. 

This project explores word embeddings using the Word2Vec model on the first book of the "A Song of Ice and Fire" series ("A Game of Thrones"). It demonstrates how to:

* Preprocess text data for Word2Vec.
* Train a Word2Vec model.
* Find similar words.
* Visualize word embeddings in 3D.

* 3.  **Data:**

    Place the text file (`001ssb.txt` assumed in the code) of "A Game of Thrones" in the Colab environment.

## Usage

1.  **Preprocessing:**

    The code tokenizes the text into sentences and then into words using `nltk.sent_tokenize` and `gensim.utils.simple_preprocess`.

2.  **Word2Vec Model:**

    A `gensim.models.Word2Vec` model is created and trained on the preprocessed text.

3.  **Exploration:**

    The code demonstrates finding similar words using `model.wv.most_similar` and calculating word similarity using `model.wv.similarity`.

4.  **Visualization:**

    Word embeddings are reduced to 3 dimensions using PCA and visualized using `plotly.express`.

## Insights

*   Word2Vec captures semantic relationships between words in the text.
*   Similar words are clustered together in the 3D visualization.
