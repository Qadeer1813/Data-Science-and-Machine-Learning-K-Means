# Data-Science-and-Machine-Learning

**Student Name: Qadeer Hussain**

**Student ID: C00270632**

**Lecture: Greg Doyle**

**K Means Clustering**

# Project Description
The purpose for this project is to cluster movies by genres and ratings to improve movie recommendations.

# Data Source
The dataset that was used for this project can be downloaded from https://grouplens.org/datasets/movielens/

# Data 
Ratings Data File Structure (ratings.csv)
- userId
- movieId
- rating: Ratings are made on a 5-star scale, with half-star increments
- timestamp: Timestamps represent seconds since midnight Coordinated Universal Time (UTC) of January 1, 1970.

Tags Data File Structure (tags.csv)
- userId
- movieId
- tag: Tags are user-generated metadata about movies. Each tag is typically a single word or short phrase. The meaning, value, and purpose of a particular tag is determined by each user.
- timestamp: Timestamps represent seconds since midnight Coordinated Universal Time (UTC) of January 1, 1970.

Movies Data File Structure (movies.csv)
- movieId
- title
- genres

Links Data File Structure (links.csv)
- movieId
- imdbId
- tmdbId

# Processing
After downloading this dataset, a test print was conducted using the following pieces of code ```movies = pd.read_csv('dataset/movies.csv')```, ```ratings = pd.read_csv('dataset/ratings.csv')```, ```tags = pd.read_csv('dataset/tags.csv'),```,
```links = pd.read_csv('dataset/links.csv')```, ```movies.head(), ratings.head(), tags.head(), links.head()```. The loaded data was then displayed. A check was done to find missing values in the dataframes using the following pieces of code 
```missing_values_movies = movies.isnull().sum()```, ```missing_values_ratings = ratings.isnull().sum()```, ```missing_values_tags = tags.isnull().sum()```, ```missing_values_links = links.isnull().sum()```. missing vlaues were fund in ```tmbId``` column.
The rows werer dropped. The average rating and the number of ratings for each movie was calculated. This was done to provide insights into the popularity and the viewer's consensus about movies. Then a check was done see if there any missing values in average ratings and number of ratings. The rows were dropped if they were found. One hot encoding was applied to the ```genres``` column. The average rating and number of ratings were normalized to ensure equal weighting for clustering. The elbow method was applied to get the optimal number of clusters. 

# Data Understanding and Visualisation 
After processing the data and finding the optimal number of clusters which was 4. The model was fitting excluding the ```movieId```, ```title```.

1. The model below is a cluster by Genres

   ![image](https://github.com/user-attachments/assets/3b85a2c0-8f68-4bcb-aa9a-3dd3c372f677)

2. The model below is the number of clusters in each movie

   ![image](https://github.com/user-attachments/assets/a14a2ea6-2a69-41b1-a84b-8409697cd475)

# Algorithims:
K Means Clustering: This is a unsupervised machine learning algorithm that groups data into a number of clusters. In this project it clustered movies by genres and ratings to improve movie recommendations

# Online Sources:
1. User guide# (2025) User Guide - pandas 2.2.3 documentation. Available at: https://pandas.pydata.org/docs/user_guide/index.html (Accessed: Feb 2025).
2. Matplotlib 3.9.2 documentation# (2025) Matplotlib documentation - Matplotlib 3.9.2 documentation. Available at: https://matplotlib.org/stable/ (Accessed: Feb 2025).
3. User guide (2025) scikit. Available at: https://scikit-learn.org/stable/user_guide.html (Accessed: Feb 2025).
4. Jakevdp (2023) Pythondatasciencehandbook/notebooks/05.11-K-Means.ipynb at master · JAKEVDP/Pythondatasciencehandbook, GitHub. Available at: https://github.com/jakevdp/PythonDataScienceHandbook/blob/master/notebooks/05.11-K-Means.ipynb (Accessed: Feb 2025).

# Tools and Tech Used: 
1. K Means Clustering
2. Jupter Notebook
3. Pandas Library - Loading the data and analysing it
4. Matplotlib - Plotting and Visualising the graph 
5. Scikit Learn(Sklearn) - Implementing K means model.
 
