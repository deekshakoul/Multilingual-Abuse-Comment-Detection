# Multilingual-Abuse-Comment-Detection
This work was done as part of Kaggle InClass competition hosted by Sharechat. We had to develop AI solutions for predicting abusive comments posted on the Moj app in 10+ languages given natural language data and user context data.  More details about the dataset and competition can be found in this [link](https://www.kaggle.com/c/multilingualabusivecomment/overview).

## Data work - 
- Process the train data carefully as the data has emojis, hinglish texts, different languages text, some symbols, links etc. Also, note that the language detected often is not correct so don't rely blindly on it.
- Features like detected language of the text, total likes, total reports and views along with text are also provided. These features were not included by me during the training process.
- Cleaned the data(remove emojis, punctuations etc)
- Trim the data acc to text lengths.

## Approaches - 
- I had applied many technique first starting with the basic TF-IDF approach + Logistic regression/NB/SVM/ensemble of classifiers.
- I had used the BERT model for text classification problem. But the text here compose of Indian languages.
- There is model specifically trained on 17 indian languages i.e [MuRIL](https://tfhub.dev/google/MuRIL/1). The working code on training and further evaluating is available in MURIL-BERT notebook.

## Results - 
-  Was able to achieve a score of 0.91631 on test dataset provided by team.
-  Computational intensive problem with huge amount of data, analysed the data and try to find the more important rows.
