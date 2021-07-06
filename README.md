# Fake-News-Detective
This repository contains the code required to build the Fake News Headlines Detective dashboard app. 

The internet today, is filled with news from all corners of the world. News comes from several sources. They could be news websites or social media sites like Facebook, Twitter and WhatsApp. Unfortunately, the content also consists of fake news, propaganda which comes packaged as news, satirical news and other kinds of news which are not reliable. So, there is a need to filter out those content. Fact-checking sites do the job of manually, by verifying with the eyewitnesses' accounts. But, there is an increasing need to do the job automatically by means of Natural Language Processing.

This dashboard app classifies news headlines into 6 categories on the increasing probability of unreliability using K-Means clustering and Support Vector classifier. New headlines are collected from Indian and US news sites by manual, web scraping and API key methods and are organized into clusters by K-Means. The Support Vector classifier is then trained on them and is used to predict the category of unseen news headlines. This hybrid method makes the dashboard app more unbiased rather than supervised learning on news headlines manually labelled as being true or fake. The dashboard app is deployed on Heroku, a cloud platform as a service, where developers can deploy their apps for free as well. 

The main challenge faced is the small overlapping of the clusters as evident from the scatterplot. But still we are able to conclude the reliability of news headlines belonging to a particular cluster by comparing the scatterplot with them. Hence this dashboard is reliable.

Do check out my dashboard app at https://fake-news-headlines-detective.herokuapp.com/

<h3> Packages specific to this project that need to be installed </h3>

1. Natural Language ToolKit(NLTK)
2. Seaborn 
3. Scikit Learn
4. Plotly
5. Dash
6. Dash Bootstrap Components

<h3> Files in this repository </h3>

News_classifier_train.ipynb - For training 
News_classifier_test.ipynb - For classifying unseeen headlines
Dashboard.ipynb - For creating dashboard app
NewsArticles.csv - Train dataset of news headlines

<h3> Site from which API key is obtained </h3>

Newsdata.io

You can create an account and choose the suitable subscription plan. Free plans are also available. 


<h3> A word of caution </h3>

The data necessary for training of the model has been collected in adherence to the terms of use and the robots.txt file of the websites. It is highly recommended that the data be collected by using API keys as much as possible. Web scrapping tools must be used only if both the robots.txt and the terms of use do not prohibit from doing so. While using web scrapping tools,it must be ensured that too many HTTP requests to the same website are not made within a short time interval, as doing so will affect the website performance adversely and can make the website crash.
