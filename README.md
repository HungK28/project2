# project2
## ETL
Our Project 2 is about Extracting, transforming, and loading movie data on Netflix and IMDb. 
The datasets we will use are from Kaggle:

*	Netflix- https://www.kaggle.com/shivamb/netflix-shows
*	IMDb- https://www.kaggle.com/stefanoleone992/imdb-extensive-dataset 

# EXTRACT
* We took the csv files, *IMDb movies.csv* and *netflix_titles.csv*, turned them into dataframes using pandas.
# TRANSFORM
* For netflix data, we filtered the dataset by selecting column headers; title, director, release_year, country.
* we renamed the netflix data from release_year to year.
* For IMDb data, we filtered the dataset by selecting only title and average vote.
* For both dataframes on the title columns, we dropped the duplicates and NA values and set title as index.
# LOAD
* Created database movies_db in PgAdmin, then created an engine connection to load the IMDb and Netflix to the movies_db as table names imdb and netflix.
* We confirmed the data was added by query.
* We created this report on IMDb and Netflix to summarize netflix movies and series with an IMDb rating.
