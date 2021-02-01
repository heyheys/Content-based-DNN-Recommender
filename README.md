# Content-based-DNN-Recommender

The goal of this project is to recommend an article for a visitor to the site. The information of current content -- content ID, category (news, lifestyle, etc.), title, author, date -- are used to predict the next content for the user. Note that the visitor ID is ignored in this task, meaning the model does not learn browse history for a particular visitor. Just predict the next content based on the current content.

The dataset is pulled from the publicly avialable Kurier.at dataset in BigQuery using SQL queries. Kurier.at is an Austrian newsite. The data have already separated to training set (179,092 records) and test set (25,599 records, some records may belong to the same visitor).

The accuracy is 0.06 and the top 10 accuracy is 0.32.
