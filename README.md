# Movie Recommender System

## My first project ever
This was my first project completed in the year 2021 and it was my first choice due to its indulging subject and real-world applicability. The attached ipnyb file consists of a collaborative filtering-based recommender system that recommends movies based on the interests and interactions of the user rather than delving into the item and user types.

I would like to share the credit for this work with @krishnaik06

## Flow of the work
1. Reading data into my Jupyter Notebook through
```
df = pd.read_csv('https://raw.githubusercontent.com/krishnaik06/Movie-Recommender-in-python/master/u.data', sep='\t', names=column_names)
```
2. Sorting the data frame according to the mean ratings (in descending order to display the most highly rated recommendation at the top)
```
   movie_ratings = df.groupby('title')['rating'].mean().sort_values(ascending=False).head()
```
3. Sorting the movies by the number of ratings (good/bad to take into consideration the popular rating of a movie)
```
   ratings.sort_values('num of ratings', ascending=False).head(10)
```
4. Calculating and displaying the most correlated movie (find code in the ipnyb file)

## What I learned through this project 
- All about the different types of recommender systems (Chose to work on collaborative based recommender)
- How to deal with missing data and how to prepare or pre-process the data for a specific use
- Basic Python libraries including Numpy and Pandas
- Visualization libraries in Python (Matplotlib and Seaborn used)
- Most importantly, the flow of a project
