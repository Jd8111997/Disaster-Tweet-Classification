# Disaster-Tweet-Classification
In this project, I had done binary classification on tweets into two following categories:
1) disaster Tweets
2) non-disaster Tweets

You can download the dataset from here : https://www.kaggle.com/c/nlp-getting-started/data  
I have used Distill-bert model to get a word embeddings of the sentence tweets.  
For that, I have used huggingface's transformer module, you can check here : https://huggingface.co/transformers/v2.0.0/model_doc/distilbert.html  
In Distill_bert module, I have got the word embeddings of training and test dataset and stored them in file features_distill.npy and features_test.npy.   
You can directly use apply classification on those word embeddings using Predictions module.  
In predictions module, I have performed classification on word embeddings using different algorithms: Neural network, Logistic regression, GaussianNB, RendomForest, SVC, Gradientboosting, decisiontrees etc. I got the best accurcy on validation data using Logistic Regression, which is 0.82.  
Furthermore, you can also achieve state of the art accuracy using bert-large-uncased model instead of distill-bert, and by using single layer neural network and by retraining last bert output layer, but it take more compute power and training time.  
I have used paperspace free gpu notebooks for this project.  
