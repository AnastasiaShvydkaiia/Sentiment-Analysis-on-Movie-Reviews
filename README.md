# Sentiment Analysis on Movie Reviews
## About
This is a NLP project focused on developing a NLP system for sentiment analysis of movie reviews using supervised machine learning techniques.

The pipeline includes data preprocessing steps such as lowercasing, removal of HTML tags and URLs, punctuation, tokenization, stop word removal, and stemming. Models, such as Logistic Regrssion, Naive Bayes and SVM are then evaluated to achieve the best results. Assessments include accuracy, precision, recall, F1 score, and AUC score. 

## Project Structure
- data: Contains the datasets used for training and testing the sentiment analysis models.
- sentiment-analysis.ipynb: Jupyter notebook with data preprocessing, model development, and evaluation.
- models: Saved models after training, including the best-performing one.

## Datasets

| Dataset 	| Description	| 
|----	|---	|
| [IMDB](https://ai.stanford.edu/~amaas/data/sentiment/)  	| The dataset used to develop the binary sentiment classifiers. It consists of 50K movie reviews labeled as positive or negative.| 
| [Cornel Review Polarity](https://www.cs.cornell.edu/people/pabo/movie-review-data/)| The dataset used for testing the trained models. This dataset collected from Cornell movie reviews.It includes 1000 positive and 1000 negative movie reviews.
| [Rotten Tomatoes Reviews](https://www.kaggle.com/datasets/mrbaloglu/rotten-tomatoes-reviews-dataset?select=data_rt.csv)   	|  The dataset used for testing the trained models. It consists of 5,331 positive and 5,331 negative processed sentences from Rotten Tomatoes movie reviews |
| [SAR14](https://github.com/daiquocnguyen/SAR14)   	|  The dataset used for testing the trained models. It contains 234k IMDB movie reviews. Particularly, this dataset consists of 167k reviews with positive sentiment(score is greater than or equal to 7) and 66k reviews with negative sentiment (score is less than or equal to 4) |
| [Letterboxd Reviews](https://www.kaggle.com/datasets/joyshil0599/movie-reviews-dataset-10k-scraped-data?select=letterboxd-reviews.csv)   	|  The dataset used for predicting with the best model. It contains 3560 rows of data, with each row representing a movie review on the Letterboxd platform. The columns in the dataset include the movie name, release year, rating, reviewer name, review date, review text, comment count, and like count. |




## Results
Evaluation results on the datasets can be seen in the tables below.

|Model            | IMDB   | Cornel Review Polarity | Rotten Tomatoes Reviews | SAR14|
|-----------------|--------|------------------------|-------------------------|------|
|Linear Regression|	90.9%  |88.2%                   |74.1%                    |89.5% |
|Naive Bayes      |	88.1%  |83.4%                   |75.3%                    |84.6% |
|SVM              |	90.8%  |88.0%                   |74.0%                    |89.4% |

## Conclusion
Through the use of machine learning techniques, this sentiment analysis project has been successful in understanding public attitude regarding movie reviews. Classifiers above identify sentiments from the review dataset according to the users opinions.