# Multilingual-Abuse-Comment-Detection
This work was done as part of Kaggle InClass competition hosted by Sharechat.  We had to develop AI solutions for predicting abusive comments posted on the Moj app in 10+ languages given natural language data and user context data.  More details about the dataset and competition can be found in this [link](https://www.kaggle.com/c/multilingualabusivecomment/overview).

## Data work - 
- Processed te train data carefully as the data is
- Cleaned the data(remove emojis, punctuations etc)
- Trim the data acc to text lengths

## Approaches - 
- I had applied many technique first starting with the basic TF-IDF approach + Logistic regression/NB/SVM/ensemble of classifiers.
- I had used the BERT model for text classification problem. There is model specificall trained on 17 indian languages i.e [MuRIL] (https://tfhub.dev/google/MuRIL/1). The working code in available in MURIL-BERT notebook.

## Results - 
-  Was able to achieve a score of 0.91631 on test dataset provided by team.
-  Computational intensive problem with huge amount of data, analysed the data and try to find the more important rows.
