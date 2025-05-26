# Fake_news_detection#

Fake News Detection using Machine Learning


## Introduction
This repository contains a comprehensive project for detecting fake news using machine learning techniques and various natural language processing techniques.The project includes data analysis, model training, and a web application for real-time fake news detection. The machine learning model is designed to classify news articles as either real or fake based on their content.

## Problem Definition
We aim to develop a machine learning program to identify when a news source may be producing fake news. The model will focus on identifying fake news sources, based on multiple articles originating from a source. Once a source is labeled as a producer of fake news, we can predict with high confidence that any future articles from that source will also be fake news. Focusing on sources widens our article misclassification tolerance, because we will have multiple data points coming from each source.

The intended application of the project is for use in applying visibility weights in social media. Using weights produced by this model, social networks can make stories that are highly likely to be fake news less visible.

## Datasets 
### train.csv
A full training dataset with the following attributes:
- id: unique id for a news article
- title: the title of a news article
- author: author of the news article
- text: the text of the article; could be incomplete
- label: a label that marks the article as potentially unreliable
  - 1: unreliable
  - 0: reliable

### test.csv
A testing training dataset with all the same attributes as train.csv without the label.

## Model Name
The machine learning model used for fake news detection in this project is the *Passive Aggressive Classifier*.

### Model Description
The Passive Aggressive Classifier (PAC) is a type of online learning algorithm for binary classification tasks. It is well-suited for applications like fake news detection. The PAC algorithm updates its model continuously as new data arrives, making it efficient for real-time classification.

### Model Accuracy
The Passive Aggressive Classifier achieved an impressive accuracy of *96%* during evaluation. This high accuracy indicates its effectiveness in classifying news articles as reliable or unreliable.
