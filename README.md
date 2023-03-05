# Word2Vec Model
Word2Vec creates an n-dimensional vector representation for every word in our data set. An implementation of the Word2Vec algorithm is provided by Gensim. The model is based on a two-layer neural network that processes text by vectorizing words. The relative distance of one word from another depends on the semantic area. Moreover, words with opposite means in the n-dimensional representation will have different orientation. Fig. shows a t-SNE visualization of the Word2Vec space for our model. Due to the large amount of words we selected a subset of relevant words to plot. Words with similar meanings are near each other in this two-dimensional representation.

<p align="center">
<img src=https://user-images.githubusercontent.com/75221419/222917928-4406a3f1-4db5-4309-b52d-dd8c15d3e51d.jpg  width="500"/>
</p>


We can also see that some of the most similar words from our model are semantically strongly correlated. Gensim model provides most_similar method. Using this method we provide a word as an input and receive as output the most similar word. For example: "sad" → "upset", "stupid" → "lame", "cute" → "adorable".

