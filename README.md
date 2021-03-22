# Content-based-DNN-Recommender

The goal of this project is to recommend an article for a visitor to the site. The information of current content -- content ID, category (news, lifestyle, etc.), title, author, date -- are used to predict the next content for the user. 

Input variables:
-- Embedded content_id;
-- Embedded author;
-- Category;
-- Embedded title;
-- Date.

Target variable:
-- The next recommended content for the user.

The neural network has four hidden layers.

The dataset is pulled from the publicly avialable Kurier.at dataset in BigQuery using SQL queries. Kurier.at is an Austrian newsite. The train and test sets are pulled through the PullData.ipynb file and stored under this directory. The training set has 179,092 records and test set has 25,599 records (some records may belong to the same visitor).

The accuracy is 0.06 and the top 10 accuracy is 0.32.
