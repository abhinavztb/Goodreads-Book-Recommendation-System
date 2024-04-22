# Goodreads-Book-Recommendation-System
Goodreads-Book-Recommendation-System 
Recommender systems are systems that help users discover items they may like. They help users discover new books, movies, and products, and help companies by promoting relevant products to prospective customers.

### Why Goodreads?
The Goodreads book dataset is a collection of data about books and ratings from the Goodreads website. It can be used to build recommendation systems or to analyze trends and patterns in book ratings and reviews. The Goodreads book dataset includes information about the books themselves, such as the title, author, publisher, and genre, as well as ratings and reviews from users. It also includes information about the users themselves, such as their location and the books they have rated and reviewed.

### Approach

In our project we used two different approaches: Popularity–based Recommendation as well as Collaborative filtering approach to analyze and make suitable recommendations.
A population-based recommendation system is a type of recommendation system that makes recommendations based on the overall preferences of a large group of users, rather than the individual preferences of a single user. This approach is often used in situations where there is a large dataset of user ratings or preferences, and the goal is to identify items that are popular or well-liked by a broad audience. In our project, we use a population-based recommendation system based on metrics like ratings and review count.
Collaborative filtering is a technique used to make recommendations based on the preferences of a group of users. It works by analyzing the past behavior of a group of users and identifying items that are highly rated by similar users.
There are two main types of collaborative filtering: user-based and item-based. In user-based collaborative filtering, recommendations are made based on the preferences of similar users. For example, if Alice and Bob both rated a particular movie highly, and Alice also rated a second movie highly, the system might recommend the second movie to Bob.
In item-based collaborative filtering, recommendations are made based on the similarity between items. For example, if Alice and Bob both rated a particular movie highly, and the movie is similar to a second movie that Alice also rated highly, the system might recommend the second movie to Bob.

### Dataset description

For the reviews dataset, we have 7 columns and 1378033 rows. Sample head of the data is:

![image](https://github.com/abhinavztb/Goodreads-Book-Recommendation-System/assets/28789570/2901469e-eb83-4bfc-b4b5-aa85dbf5414c)
![image](https://github.com/abhinavztb/Goodreads-Book-Recommendation-System/assets/28789570/eb46cc92-64aa-45be-841f-de1e1cb89427)

### Dataset Preprocessing and Feature selection
The dataset contains has_spoiler (boolean feature) which we convert into a numerical feature for better analysis.
● Similarly, the review_sentences is a list of all the reviews given (categorical attribute) and for this we take the number of review_sentences given to a certain book for estimating impact.
● We also draw a T-SNE plot for all the numerical features projected into two components.
T-SNE (t-distributed stochastic neighbor embedding) is a dimensionality reduction technique that is often used for visualizing high-dimensional data. It is particularly useful for visualizing data in which there are many features (i.e. dimensions), as it can reduce the data down to just two or three dimensions for easy visualization.
In the context of feature selection, t-SNE can be used to identify the most important features in a dataset. By visualizing the data with t-SNE, you can see which features are most strongly correlated with one another and which are less important. This can help you identify the most relevant features for a particular task, such as building a machine learning model.
To create a t-SNE plot, you first need to select a set of features from your dataset and then apply t-SNE to reduce the data down to two or three dimensions. The resulting plot will show you how the features are related to one another, and you can use this information to identify the most important features for your task.
 
  <img width="1200" alt="image" src="https://github.com/abhinavztb/Goodreads-Book-Recommendation-System/assets/28789570/f8c57edc-a869-4ca4-8f1d-26d892f75d23">

