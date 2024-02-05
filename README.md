# Movie Analysis
Documentation on Python correlation project
About Dataset

#### Project overview
Is the movie industry dying? is Netflix the new entertainment king? Those were the first questions that led me to create a dataset
focused on movie revenue and analyze it over the last decades. But, why stop there? More factors intervene in this
kind of thing, like actors, genres, user ratings, and more. And now, anyone with experience (you) can ask specific questions about the
movie industry, and get answers.
###Data Sources
https://www.kaggle.com/datasets/danielgrijalvas/movies

### Content
There are 6820 movies in the dataset (220 movies per year, 1986-2016). Each movie has the following attributes:
###Tools
-Python: this was used for data cleaning and visualization

[Download here](https://www.anaconda.com/download)



budget: the budget of a movie. Some movies don't have this, so it appears as 0

company: the production company

country: country of origin

Director: the director

genre: main genre of the movie.

gross: revenue of the movie

name: name of the movie

rating: rating of the movie (R, PG, etc.)

released: release date (YYYY-MM-DD)

runtime: duration of the movie

score: IMDb user rating

votes: number of user votes

star: main actor/actress

writer: writer of the movie

year: year of release

### Data Cleaning and Wrangling
1. import the packages we will use in this project
2. import the Data we will use in this project
3. Check for any missing data
4. loop through the data and see if there is anything missing
5. Check Data Types for our columns
6. Are there any Outliers?
7. Remove Duplicates

### Exploratory Data Analysis
1. What is the correlation between Budget and Gross Earnings
2. What is the degree of correlation between both

   <img width="773" alt="Scatter plot" src="https://github.com/godiyap/Python-Correlation-Project/assets/158599025/3de89c8f-2244-40d7-81b0-034402e2da4b">


### Results/Findings
We found a high correlation of 0.632 between votes and gross revenue.

### Data Analysis
Python
```correlation_matrix = df_numerized.corr(method='pearson')
sns.heatmap(correlation_matrix,annot=True)
plt.title('Correlation matrix for numeric features')
plt.xlabel('Mpvie Features')  
plt.ylabel('Movie feature') 
plt.show()```


