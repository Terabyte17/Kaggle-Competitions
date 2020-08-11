## Kaggle Competitions
This repository holds the notebooks related to all the Kaggle Competitions I have participated in and will be updated continously. 

### List of Notebooks:-
- #### Bengali AI Grapheme Classification. 
  Kaggle competition related to computer vision, in which a bengali grapheme had to be separately classified into its 3 components - grapheme root, vowel diacritic and consonant    diacritic. 2 notebooks were used for this, one for training the [model](https://github.com/Terabyte17/Kaggle-Competitions/blob/master/Grapheme%20Classification%20Model.ipynb) and one for [submitting](https://github.com/Terabyte17/Kaggle-Competitions/blob/master/Bengali%20AI%20Grapheme%20Classification.ipynb) the model. The model consisted of a functional API with 3 different output layers and was trained for 15 mins on Kaggle GPU which gave a final public score of 92.25. You can find the competition [here](https://www.kaggle.com/c/bengaliai-cv19).
  
- #### NLP Disaster Tweets
  Kaggle competition related to natural language processing, in which sentiment analysis had to be carried out on tweets to determine whether the tweets were fake or not. Initially, the tweets were preprocessed to remove all the emojis, html tags and urls, by using RegEx. Then, the words were tokenized, lemmatized, stopwords were removed, and then padded to get a sequence of 50 words. The words in the tweets were converted into embeddings using pretrained GloVE vectors after which the were passed into 2 layers of LSTM network, in which both of them were bidirectional. The second layer only returned the last hidden state of that layer, which was passed through a dense layer. The model was trained for 15 mins to get a final public score of 80.50. You can find the competition [here](https://www.kaggle.com/c/nlp-getting-started).  

- #### KMeans Clustering of NYC WiFi Hotspots
  Notebook based on using the inbuilt sklearn library to cluster the given data points using the KMeans algorithm, and mapping them using the folium library. The dataset consisted of latitudes and longitudes of the various WiFi hotspots around the city along with other features such as provider, borough etc. On clustering all the data points, the result was as follows:-
<p align="center">
<img  width="300" height="300" src="https://github.com/Terabyte17/Kaggle-Competitions/blob/master/media/all.png">
</p>

  However, it is better to cluster data points for each provider individually, to visualize how they have structured their WiFi network. The results of clustering on the data points belonging to the biggest network provider is as follows:-
  
<p align="center">
<img  width="300" height="300" src="https://github.com/Terabyte17/Kaggle-Competitions/blob/master/media/provider.png">
</p>
