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
```links = pd.read_csv('dataset/links.csv')```, ```movies.head(), ratings.head(), tags.head(), links.head()```. The loaded data was then displayed.

# Data Understanding and Visualisation 

# Algorithims:


# Online Sources:

# Tools and Tech Used: 
1. Linear Regression
2. Jupter Notebook
3. Pandas Library - Loading the data and analysing it
4. Numpy Library - Processing the data
5. Matplotlib - Plotting and Visualising the graph 
6. Scikit Learn(Sklearn) - Implementing linear regression model.
 
