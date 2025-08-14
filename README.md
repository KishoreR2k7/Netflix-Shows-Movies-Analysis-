# Netflix Shows & Movies Analysis

This project performs an in-depth analysis of Netflix’s movies and TV shows dataset using **Python**, **Pandas**, **NumPy**, **Matplotlib**, and **Seaborn**. The analysis includes data exploration, visualization, statistics, linear algebra operations, feature engineering, and SQL-like queries in Pandas.

---

## Dataset

The dataset `netflix_titles.csv` contains information about Netflix titles, including:

- `show_id`
- `type` (Movie/TV Show)
- `title`
- `director`
- `cast`
- `country`
- `date_added`
- `release_year`
- `rating`
- `duration`
- `listed_in` (genres)
- `description`

---

## Part 1 – Basic Data Understanding

- Load the CSV file into a Pandas DataFrame.
- Display the first 10 rows.
- Show the shape, column names, and data types.
- Generate descriptive statistics for numerical and categorical columns.
- Count unique values per column.
- Identify the most frequent country.

---

## Part 2 – Exploratory Data Analysis (EDA)

- Bar chart of **Movies vs TV Shows**.
- Top 10 countries producing most content.
- Top 10 most common genres.
- Scatter plot of **release year vs count of titles**.
- Histogram of movie durations.
- Bar chart of number of titles added per year.
- Identify the year with the highest number of releases.

---

## Part 3 – Statistics

- Calculate **mean**, **median**, **mode**, **variance**, and **standard deviation** of `release_year`.
- Percentage of titles released in the last 5 years.
- Most common rating for Movies and TV Shows separately.

---

## Part 4 – Linear Algebra & NumPy

- Convert `release_year` to a NumPy array.
- Create a binary array for movies (1 if Movie, else 0).
- Perform vector addition and dot product.
- Normalize the `release_year` array.

---

## Part 5 – Calculus

- Define a popularity score function:
