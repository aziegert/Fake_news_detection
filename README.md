![zatrzymaj-koncepcje-falszywych-wiadomosci-dzieki-widokowi-z-gory](https://github.com/aziegert/Fake_news_detection/assets/123495041/a240b7f3-e0b2-49c1-8d75-b1d27def92f5)

# Fake news detection

### Project written as part of the course "Data Science after SDA bootcamp"
According to the Collins dictionary, fake news can be defined as 'false, often sensational, information disseminated under the guise of news reporting. Despite the fact that fake news existed for many years, its impact has recently increased.
This project aims to develop a machine learning model that can detect fake news. The Fake News Detection project consists of three projekts.

## Projekt 1
The first part contains the data processing process, including tokenization, data cleaning (which includes: removing stopwords, unnecessary punctuation marks, numbers, special characters, etc.) and embedding.
![image](https://github.com/aziegert/Fake_news_detection/assets/123495041/05b618a4-0445-4e3b-8ae3-46065949533f)
The Most Common Words technique was used to identify the most common words in the dataset.
![image](https://github.com/aziegert/Fake_news_detection/assets/123495041/325173f2-00d1-4664-bcf7-ad2bb5d64f95)
The Word Cloud library was used to create a word cloud based on the dataset. It is a visual representation of words where the frequency of a word is proportional to its size in the cloud.
![image](https://github.com/aziegert/Fake_news_detection/assets/123495041/720f0f9f-0bcb-4532-872f-5b7c8b50d714)

Based on the Logistic Regression model, two models were built: one using the "title" column and the other using the "text" column.
The best prediction was obtained without building a model, only on the basis of the "subject" feature.
The best prediction was obtained in the model analyzing news titles. On the test set, the accuracy was 99.52%.

## Projekt 2
This project is a modified version of Project 1. This version of the project uses SentenceTransformer as the embedding method.

## Projekt 3
Project 3 includes:
Comparing diffrent models
Comparing model performance with and without cutting "stopwords".
Comparing model performance with and without lemmatization nor stemming.
Finding similar news using cosine distance in vector space.
> News title:
> Casualties in explosion at airfield near Kabul: U.S. military
>
> Top 5 most similiar news title in all titles:
> 
> Casualties in explosion at airfield near Kabul: U.S. military 
>  Score: 0.0  ID: 44315
> 
> U.S. military aircraft crashes in Syria, injuring two: officials 
>  Score: 0.1168  ID: 42175
> 
> U.S.-led surveillance aircraft leave area near Islamic State convoy in Syria 
>  Score: 0.1308  ID: 44070
> 
> Turkish military kills three PKK militants in north Iraq near border: sources 
>  Score: 0.1428  ID: 42203
> 
> Violence flares at protest near U.S. Embassy in Lebanon 
>  Score: 0.1511  ID: 36106

## The Data
The data used for this project was sourced from Kaggle.
https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset?select=True.csv
