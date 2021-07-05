# Fake-News-Detective
This repository contains the code required to build the Fake News Headlines Detective dashboard app. 

The internet today, is filled with news from all corners of the world. News comes from several sources. They could be news websites or social media sites like Facebook, Twitter and WhatsApp. Unfortunately, the content also consists of fake news, propaganda which comes packaged as news, satirical news and other kinds of news which are not reliable. So, there is a need to filter out those content. Fact-checking sites do the job of manually, by verifying with the eyewitnesses' accounts. But, there is an increasing need to do the job automatically by means of Natural Language Processing.

This dashboard app classifies news headlines into 6 categories on the increasing probability of unreliability using K-Means clustering and Support Vector classifier. New headlines are collected from Indian and US news sites by manual, web scraping and API key methods and are organized into clusters by K-Means. The Support Vector classifier is then trained on them and is used to predict the category of unseen news headlines. This hybrid method makes the dashboard app more unbiased rather than supervised learning on news headlines manually labelled as being true or fake.

Do check out my dashboard app at https://fake-news-headlines-detective.herokuapp.com/

