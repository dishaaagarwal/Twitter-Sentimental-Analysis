# Twitter-Sentimental-Analysis

## Problem Statement

The objective of this task is to detect hate speech in tweets. For the sake of simplicity, we say a tweet contains hate speech if it has a racist or sexist sentiment associated with it. So, the task is to classify racist or sexist tweets from other tweets.

## Table of Content
- **Objective**
- **Loading the libraries and dataset**
- **Text Cleaning & Preprocessing**
     1. **Cleaning the text using regex**
     2. **Tokenization**
     3. **Stemming & Lemmatization**
- **Data Visualization with WordCloud**
- **Word Vectorization(BOW,TFIDF,WE)**
- **Model Building**
- **Making Submission**

- **Objective**

Hate  speech  is  an  unfortunately  common  occurrence  on  the  Internet.  Often social media sites like Facebook and Twitter face the problem of identifying and censoring  problematic  posts  while weighing the right to freedom of speech. The  importance  of  detecting  and  moderating hate  speech  is  evident  from  the  strong  connection between hate speech and actual hate crimes. Early identification of users promoting  hate  speech  could  enable  outreach  programs that attempt to prevent an escalation from speech to action. Sites such as Twitter and Facebook have been seeking  to  actively  combat  hate  speech. In spite of these reasons, NLP research on hate speech has been very limited, primarily due to the lack of a general definition of hate speech, an analysis of its demographic influences, and an investigation of the most effective features.

- **Text Cleaning & Preprocessing**

In this part I have converted the unstructured data into structured data by removing Special Characters, Puncuations and Stopwords with the help of Regex and finally converted the sentences into cleaned tokens by using the Tokenizer.

**Data Visualization with WordCloud**

Data Visualization plays a key role in improving of understanding on the data. We can do the same using WordCloud which comes handy when dealing with Text data.
With the help of Wordcloud I have tried to understand the distribution of Positive and Negative words and which words appear the most.

![](/images/img_1.png)

Also I have tried to extract useful Information from the **Hashtags** to check if they help in differentiating the labels.


- **Word Vectorization(BOW,TFIDF,WE)**

This is the final step before Model building were we convert our Text data into Sparse matrix. There are various ways of Vectorization but in this repository i have concerntrated on **TFIDF, Bag of Words(BOW)**. 

- **Model Building**

In part I have experimented with Logistic Regression and Naive Bayes techniques using both TFIDF and BOW models.

![](/images/img_5.png)
![](/images/img_6.png)

- **Making Submission**

I wasable to achieve an **f1-score of 0.56** using Logistic Regression with TFIDF mode.
