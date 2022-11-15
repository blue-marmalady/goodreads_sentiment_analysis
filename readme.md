## Project Goals

To identify whether or not review sentiments are a good indicator of book approval/popularity. To check whether they are as good or better than star ratings as a predictor.\
\
As such, I focused on thre questions:\
Q1 - Do reviewer's ratings of the work differ from their sentiments?\
Q2 - Do review sentiments change over time? I.e. will reviews given up to 6 months after publications differ in sentiment from those given after 6 months for the same book?\
Q3 - Which feature, ratings or reviews, is a better predictor of overall popularity (approximated by number of reviews)?


## Frameworks

tensorflow \
keras \
scikit.learn \
scipy.stats

## Data Sets

[UCSD Bookgraph](https://sites.google.com/eng.ucsd.edu/ucsdbookgraph/home) \
[Stanford AI Lab IMDB dataset](https://ai.stanford.edu/~amaas/data/sentiment/)

## Process

A BERT model was trained on the IMDB reviews, this can be found in the training folder. \
\
This model was then applied to the Goodreads data. The data was prepared as per the data_preparation folder. The files c_splitter and e_combiner only serve to break the data into chunks for easier processing.\
\
The three questions are answered by analyses in the following files:\
Q1 - rev_rating_diff\
Q2 - early_late_review\
Q3 - feature_imp

