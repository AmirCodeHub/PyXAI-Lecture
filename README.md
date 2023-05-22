# Explainable AI - Cognitive Systems Lecture 


## Introduction: Using Jupyter Notebook via Anaconda for the Assignment

Welcome to your next assignment! For this task, we will be using Jupyter Notebook, an open-source web application that allows you to create and share documents that contain live code, equations, visualizations, and narrative text. We will access the Jupyter Notebook through Anaconda, a powerful and easy-to-use open-source distribution of Python.

Anaconda greatly simplifies the process of installing and managing the different software dependencies for data science and machine learning. Here's a simple guide to get you started:

## 1. Installation
- Download Anaconda: Go to the [Anaconda Installations](https://www.anaconda.com/download) page, and download the version that suits your system and Python version preference. We recommend using Python 3.x.

- Install Anaconda: Run the installer file and follow the instructions. If you are unsure about any settings, accept the defaults. They can be changed later.

## 2. Launching Jupyter Notebook
- Open Anaconda Navigator: After installation, you can open Anaconda Navigator from your programs/applications menu. It provides a user-friendly interface for managing packages and environments and launching applications.

- Launch Jupyter Notebook: From the Anaconda Navigator, click on the Jupyter Notebook icon. A new browser window will open with the Jupyter file browser.

- Navigate and Launch: From the file browser, you can navigate to the directory containing your assignment notebook file (.ipynb extension), and click on it to open.





## Assignment Description: Explainable AI with LIME and Random Forest Classifier

#### In this assignment, you will be introduced to the concept of explainable AI using Python. You will get hands-on experience with the LIME (Local Interpretable Model-Agnostic Explanations) algorithm and Random Forest Classifier.

Your task is to:

1. Load the 20 Newsgroups dataset: This dataset is a collection of approximately 20,000 newsgroup documents, partitioned across 20 different newsgroups. You will be working with a subset of this data, specifically focusing on the 'alt.atheism' and 'soc.religion.christian' categories.

     **Tip** - **Loading the 20 Newsgroups dataset**: This is a well-known dataset available in sklearn. You can find more information and the necessary functions to load this dataset in the sklearn.datasets documentation ([Click here](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_20newsgroups.html)), specifically the fetch_20newsgroups function and its parameters (e.g. "subset" and "categories" parameter).


2. Preprocess the data: You will use sklearn.feature_extraction.text.TfidfVectorizer to convert the raw documents into TF-IDF features. You need to transform both the training and the test datasets.

     **Tip** - **Preprocessing the data**: The TfidfVectorizer function from sklearn.feature_extraction.text is used in this step. This function is well-documented in sklearn's feature extraction documentation ([Click here](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html)). It is essential to understand the parameters and the output of this function.


3. Train a Random Forest Classifier: You will use sklearn.ensemble.RandomForestClassifier to train a model on the preprocessed training data. Random Forest is a powerful ensemble learning method that operates by constructing multiple decision trees during training and outputting the class that is the mode of the classes or the mean prediction of the individual trees.

      **Tip** - **Training a Random Forest Classifier**: The RandomForestClassifier is a part of the ensemble module of sklearn. The official sklearn documentation provides a comprehensive explanation and examples for this classifier (click here: [sklearn.ensemble.RandomForestClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)).


4. Use the LIME algorithm to explain the predictions: LIME is a novel algorithm that can explain the predictions of any classifier or regressor in a faithful way, by approximating it locally with an interpretable model. You need to use the LimeTextExplainer to explain the prediction of a test document of your choice (here we are using document with index 83). Finally, you are required to display the explanation using show_in_notebook() function.

    **Tip** - **Using the LIME algorithm to explain the predictions**: LIME is a separate package for Python, and it has its own dedicated documentation which explains how to use the LimeTextExplainer among other things ([Checkout the documentation here](https://lime-ml.readthedocs.io/en/latest/lime.html#module-lime.lime_text)). Make sure to understand the parameters and the output of the explain_instance function. 