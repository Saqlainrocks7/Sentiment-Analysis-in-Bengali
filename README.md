# Sentiment-Analysis-in-Bengali
## Overview
Social media these days is generating a vast amount of sentiment rich data in the   form of tweets, status updates, blog posts etc. Sentiment analysis of this user generated data is very useful in knowing the opinion of the crowd. It deals with identifying and classifying opinions or sentiments expressed in source text. Sentiment analysis of such data helps us to understand the proper meaning of the data. It is an application of natural language processing, also known as emotion extraction or opinion mining.

## Motivation
Usually sentiments can be varied in cultures and languages. On sentiment analysis, an extensive amount of research works can be seen for well-resourced languages like English, Japanese etc. However, such works are relatively less observed for low-resourced language like Bengali. Bengali is the world's seventh most spoken native language.In 2010 ,it was voted as the sweetest language by UNESCO.  Digital contents in Bengali text are increasing with the advancements of World Wide Web (WWW) to express the sentiment of content originators from mixed perspectives. These high voluminous unstructured web contents can be utilized to build smarter tools to assist people through Natural Language Processing (NLP). Though Bengali NLP tools are still inadequate due to its inherent complexities, research on Sentiment Analysis in Bengali is flourishing as a challenging area and is getting researcher's attention at a rapid pace.

## Data Preprocessing
  1. Collecting The Dataset:
We collected a dataset from Kaggle. It was a Bengali dataset of newspaper articles. It had two .txt files. One comprised of negative sentences of around 3500 sentences. The other was a positive news file of around another 3500 sentences. The next step was to pre-process the data 

  2. Data Pre-processing:

         2.1 Removing punctuations

One of the important step towards data cleaning or data pre-processing is removing unwanted punctuations. We have cleaned our dataset of various punctuations such as ‘,’ ‘|’,’!’. Such punctuations do not add any meaning and the removal of these unwanted punctuations would not hamper the result or accuracy of our project. 

       2.2	Removing numbers

Numbers do not contribute to the accuracy and has no meaning
in sentiment analysis. So they are removed during preprocessing.

       2.3	Removing stop words


Stop words are actually the words which do not add any relevant information to our model. In our Bengali dataset there were several stop words as such ‘যা’ , ‘যার’ , ‘এই’ , ‘তাও’ which do not generally carry any important meaning to our dataset and can be removed so that the more emphasis can be made on the important word which in our case are the positive words and the negative words.


## Approach
In resource based sentiment analysis we take the help of a prior resource and with the help of it we predict the sentiment of our dataset. Our resource here is the Bengali SentiWordNet which we have used for classification. From Kaggle we have collected a Hindi SentiWordNet dataset and using googletrans we have converted it to Bengali. The list was POS tagged and each word had its corresponding positive and negative scores assigned to it. The list had around 3000 words.

We had also received a Bengali SentiWordNet from the website created by Amitava Das. But that list did not contain any tagged positive  and negative score assigned to the list of words. So we instead chose the Hindi dataset available from Kaggle. 
