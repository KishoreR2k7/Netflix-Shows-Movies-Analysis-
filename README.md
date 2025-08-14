#Netflix Shows & Movies Analysis:
##*Part 1 – Basic Data Understanding (Pandas)*
-Load the CSV file into a Pandas DataFrame.
-Display the first 10 rows of the dataset.(df.head(10))
**Show the shape, column names, and data types.
**Use .describe() for numerical and categorical columns.
**Get the number of unique values for each column.
**Display the most frequent value in the country column.


#*Part 2 – EDA (Exploratory Data Analysis)*
**Plot a bar chart for the count of Movies vs TV Shows.
<img width="742" height="565" alt="image" src="https://github.com/user-attachments/assets/91758f39-49f1-4077-b2f5-e61b14623a7d" />
**Find the top 10 countries producing the most content.
**OUTPUT:country
United States     1846
India              875
United Kingdom     183
Canada             107
Spain               91
Egypt               90
Nigeria             88
Japan               83
Turkey              79
Indonesia           76
Name: count, dtype: int64
**Find the top 10 most common genres in listed_in.
OUTPUT:listed_in
International Movies        2369
Dramas                      2293
Comedies                    1553
Action & Adventure           806
Independent Movies           740
Romantic Movies              579
Thrillers                    547
Children & Family Movies     503
Documentaries                391
Horror Movies                336
Name: count, dtype: int64

**Scatter plot: release_year vs count of titles.
<img width="713" height="569" alt="image" src="https://github.com/user-attachments/assets/a9896a5d-6079-4c07-acf3-44dc207e8969" />


**Create a histogram of movie durations (in minutes).
<img width="715" height="546" alt="image" src="https://github.com/user-attachments/assets/760709bc-2d55-481c-9f20-574503c55c0f" />


**Bar chart of the number of titles added per year (based on date_added).
<img width="698" height="542" alt="image" src="https://github.com/user-attachments/assets/5411d8f6-c6f5-4ed4-84d5-8c11eb4be30a" />

**Find the year with the highest number of releases.
OUTPUT:
type
Movie    5185
Name: count, dtype: int64

#Part 3 – Statistics
**Calculate the mean, median, mode of release_year.
OUTPUT:
Mean:2012.7421230307577
Median:2016.0
Mode:0    2017
Name: release_year, dtype: int64

**Find the variance and standard deviation of release_year.

<img width="729" height="734" alt="image" src="https://github.com/user-attachments/assets/7e1fc505-6ad3-49f5-ac60-128479679b5e" />

**Percentage of titles added in the last 5 years.
**OUTPUT:94.50
**Find the most common rating for Movies and TV Shows separately.
Movie      TV-MA
TV Show    TV-MA
Name: rating, dtype: object

#*Part 4 – Linear Algebra & NumPy*

**Create a NumPy array of (release_year).
OUTPUT:[1993, 2021, 2021, ..., 2009, 2006, 2015], shape=(5332,)
**Create a NumPy binary array for (is_movie) (1 if type=Movie else 0).
OUTPUT:[1, 0, 1, ..., 1, 1, 1], shape=(5332,)
**Perform (vector addition of release_year array and is_movie array).
OUTPUT:[1994, 2021, 2022, ..., 2010, 2007, 2016], shape=(5332,)
**Compute (the dot product of release_year and is_movie arrays).
OUTPUT:[1993,    0, 2021, ..., 2009, 2006, 2015], shape=(5332,)
**Normalize the release_year column using vector normalization.
OUTPUT:[0.01356029 0.01375081 0.01375081 ... 0.01366916 0.01364875 0.01370998]


#*Part 5 – Calculus*
**Assume a function:
 Popularity_Score = (is_movie×release_year) + 0.5×(release_year−2000)^2
 Find the derivative with respect to release_year.
OUTPUT:is_movie + 1.0*release_year - 2000.0

#*Part 6 – Feature Engineering*
**Create content_age = 2025 - release_year.
**Create is_movie column (1 if type='Movie', else 0).
**Create recent_release (1 if release_year >= 2020, else 0).
**Create num_genres = count of genres in listed_in.
**Rank titles into quartiles based on release_year.

#*Part 7 – SQL Simulation in Pandas*

**Select all titles where type = 'Movie' and release_year > 2015.
**Sort movies by release_year descending and title ascending.
**Get the top 5 countries by number of titles, sorted by count descending.
**Get all titles released between 2000 and 2010.
**Count how many titles have “Drama” in their listed_in column.

#*Part 8 – Insights*

**Which country produces the most Netflix content?('United States')
**Which year had the highest content release?(2017)
**Are Movies or TV Shows more frequent?
output:
type
Movie      5185
TV Show     147
Name: count, dtype: int64
**Which genre appears most frequently on Netflix?('International Movies')

