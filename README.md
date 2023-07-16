# Topic Classification using Naïve Bayes Classifier

This repository contains code for implementing topic classification using the Naïve Bayes classifier. The classifier is trained on a set of documents from different domains and then used to predict the topic of test documents.

## Problem Description

The task is to classify documents into different topics based on their content. The Naïve Bayes classifier is used to estimate the probability of each class given the document's features (words).

## Usage

The notebook contains the following components:

1. `Loading Data` function: Downloads training and test documents from Wikipedia API for two different domains.
2. `class_prob` function: Calculates the probability of each class (topic) based on the training documents.
3. `preprocessing` function: Performs preprocessing steps on the training documents.
4. `getTokens` function: Extracts unique words (tokens) from preprocessed training documents.
5. `conditional_prob` function: Calculates the conditional probability of a word given a class.
6. Model training and saving: Trains the Naïve Bayes classifier using the training data and saves the probabilities of all classes and a dictionary of probabilities for each word in each class.
7. `predict` function: Loads the saved probabilities and predicts the topic of test documents.
