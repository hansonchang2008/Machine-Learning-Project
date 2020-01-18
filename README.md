# Machine-Learning-Project
Project Title: Soundtrack genre and popularity prediction based on soundtrack features in Spotify

Group member names:
Hanxiang & Sonam

Project Description:
In this growing world of digital media, providing great user-experience is the foremost task. One of
the ways to do so in soundtrack world is to provide users with the most popular songs. In light of this
idea, we are going to take up this challenge by predicting genre and popularity of soundtracks using
Spotify dataset, and thereby suggests users with most popular soundtracks and their genres.
In order to achieve the above, we are going to predict the genre of songs using classification and to
predict the popularity of songs using regression. We planned to use K-nearest Neighbour and Support
Vector Machine to predict the genre whereas to predict popularity of soundtracks we are going to use
Linear Support Vector Regression and Stochastic Gradient Descent Linear Regression model. We will
be implementing these algorithms in Sci-kit learn using Python language and as for the dataset, we are
going to use Spotify data obtained from Kaggle website. More about dataset is in data set description
section.

Code description:
Genre file is the python code for genre prediction;
Popularity file is the python code for popularity regression.

Dataset Description:
The dataset is music database from Spotify including 232,725 tracks. There are 26 genres in total, and
each genre consists of about 10,000 tracks. There are 18 attributes for each soundtrack, including
track name, artist's name, track id, genre, popularity, acousticness, danceability, duration (ms),
energy, instrumentalness, key, liveness, loudness, mode, speechiness, tempo, time_signature and
valence. Note that the latter 13 attributes are the audio features as defined by Spotify.
The link to the dataset is as follows.
https://www.kaggle.com/zaheenhamidani/ultimate-spotify-tracks-db

Abstract:
In the digital music industry, providing a great user experience is the foremost task. One of the ways to do so in the soundtrack world is to provide users with the most popular songs and genres. Considering this idea, we took up the challenge to predict the genre and popularity of soundtracks using the Spotify dataset. This paper is divided into two sets of case studies. The first case study examines the performance of five machine learning classification algorithms, namely, Logistic Regression, Decision Tree, K-nearest Neighbour, JRip and Random Forest to classify genres. Similarly, the second case study examines the performance of five machine learning regression algorithms, namely, SGDRegressor, KNeighborsRegressor, Decision Tree, LightGBM and M5 to predict the popularity of soundtracks. In each test case, we applied the standard machine learning model testing method to analyze and evaluate the best algorithms. For the first test case, Random Forest turned out to be the best classifier with the training accuracy of 86.1%. Whereas, in the second test case, M5-Rules (rule-based algorithm) earned the lowest training root mean squared error (RMSE) of 0.147. However, the best performer for the second test case is held by LightGBM with RMSE of 0.149 because M5 took more than 15 mins in training and LightGBM took few seconds. 


Conclusion:
It is vital that we carefully pre-processed the noisy and inconsistent data, did feature selection and balanced the data.
Data Preprocessing is very important in our task.
In preprocessing, we reduced the skewness of some highly skewed features such as speechiness by transforming these features into distributions that are closer to normal distribution. 
And we also checked and solved the inconsistency of the genres, which are the classes to predict. We also removed the duplicated data points. Besides, feature transformation is employed to convert all the feature values into the same scale between 0 and 1. Feature selection is done using common sense and feature ranking with the recursive feature elimination algorithm. We balanced the data using oversampling on the training data, which improved the performance.
For genre classification, we successfully predicted the genre of soundtracks with an overall test accuracy of 84% for eight genres using the Ensemble machine learning algorithm Random Forest. Data preprocessing is a crucial part to improve the performance in this task.
For popularity prediction using regression, we managed to predict the popularity of soundtracks with a Root Mean Square Error of 0.149625 for testing by using the Ensemble method Light Gradient Boosting efficiently. Even though rule-based regressor M5-Rules is the best performant one based on the result from the paired t-test, it is, however, the slowest which took more than 15 mins, which is significantly longer than the other four models.
In conclusion, we found that the ensemble method works best comparably in terms of both performance and speed for both genre classification and popularity prediction using regression, based on the experimental result for the 5 different types of algorithms of both genre classification and popularity regression tasks. The reason could be that the ensemble method actually learns a set of models that provides diversity in learning styles which improved the performance.
