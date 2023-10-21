# SentimentAnalysis

## Dataset : []()
##### > Dataset Download Reference Link : http://ai.stanford.edu/~amaas/data/sentiment/ []()
##### > Large Movie Review Dataset []()
##### > This Dataset contains 25,000 highly polar movie reviews for training, and 25,000 for testing. []()

<br> 

## Pre-Processing : []()
##### > Convert to Lower Case []()
##### > Removed Punctuations []()
##### > Removed Extra Spaces []()
##### > Limited the Length of Sentance within 30 - 200 Words []()
##### > Mapped Words to Glove vectors []()
##### > Used PorterStemmer if word not found in Glove file []()

<br> 

## Model : []()
##### > Simple 2 Layer LSTM Model implemented in Tensorflow 1.0 []()
##### > Dynamic RNN with LSTM Cell of Dimenssion 50 & Final Dense layer with 2 Units []()

<br>

## Training : []()
##### > Optimizer used for Training the Model : ADAM []()
##### > Used default learning rate []()
##### > Loss function : softmax_cross_entropy []()

<br>

## Setup : []()

#### 1. Dowload the Dataset & Glove Matrix : []()
```
wget http://ai.stanford.edu/~amaas/data/sentiment/aclImdb_v1.tar.gz -O aclImdb_v1.tar.gz
```

```
tar -xvzf aclImdb_v1.tar.gz
```

```
wget http://nlp.uoregon.edu/download/embeddings/glove.6B.50d.txt -O glove.6B.50d.txt
```
<br>

####  2. Install other Python helper modules : []()

```
python3 -m pip install --upgrade pip
```
```
pip3 install nltk
```
```
pip install pandas
```
<br>

## Run the Training Notebook : [Text_Sentiment_Analysis.ipynb](https://github.com/ajithAI/SentimentAnalysis/blob/master/Text_Sentiment_Analysis.ipynb)
