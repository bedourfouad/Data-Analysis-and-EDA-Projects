# TMDB Movies Dataset Analysis

| Contents 											 	   	|  
| -------- 											 	   	|  
| [Dataset Description](#Dataset-Description)			   	|  
| [Columns Descriptions](#Columns-Descriptions) 		   		|  
| [Exploratory Data Analysis (EDA) Questions](#EDA-Questions) |  
| [Conclusion](#Conclusion)									|  
| [Built with](#Built-with)							   		|  

## Dataset Description
This dataset contains information about over 9,000 movies extracted from the TMDB API.

## Columns Descriptions
1. **Release_Date**: Date when the movie was released.
2. **Title**: Name of the movie.
3. **Overview**: Brief summary of the movie.
4. **Popularity**: A metric computed by TMDB developers based on views, votes, and user interactions.
5. **Vote_Count**: Total votes received from viewers.
6. **Vote_Average**: Average rating out of 10 based on votes.
7. **Original_Language**: Original language of the movies (not including dubbed versions).
8. **Genre**: Categories the movie can be classified into.
9. **Poster_Url**: URL of the movie poster.

## EDA Questions
- **Q1:** What is the most frequent `genre` in the dataset?
- **Q2:** Which `genres` have the highest `votes`?
- **Q3:** What movie has the highest `popularity`? What is its `genre`?
- **Q4:** Which year has the most films released?

___

## Environment Set-up
- Importing necessary libraries and getting the dataset file directory.

___

### Public Functions
Here, we define functions for categorizing columns in the dataset for better usability and functionality.

___

## Data Wrangling
We load our data from the CSV file and explore it to check for any required cleaning steps.
- The dataset contains 9827 rows and 9 columns, with no NaNs or duplicated rows.
- The `Release_Date` column needs to be converted to datetime format to extract the year.
- `Overview`, `Original_Language`, and `Poster_Url` columns may not be useful for analysis.
- The `Genre` column needs processing since genres are separated by commas.

___

## Data Cleaning
- Casting `Release_Date` column and extracting year values.
- Dropping unnecessary columns.
- Categorizing `Vote_Average` column into four categories: `not_popular`, `below_avg`, `average`, `popular`.
- Handling `Genre` column's comma-separated values.

Now that our dataset is clean, we have a total of 6 columns and 25,551 rows to analyze.

___

## Data Visualization
Using visuals, we create informative graphics to gain insights about our data.
- **Q1:** Visualizing the most frequent `genre` in the dataset.
- **Q2:** Visualizing which `genres` have the highest `votes`.
- **Q3:** Checking which movie has the highest `popularity` and its `genre`.
- **Q4:** Analyzing which year has the most films released.

___

## Conclusion
#### Q1: What is the most frequent `genre` in the dataset?
The `Drama` genre is the most frequent in our dataset, appearing over 14% of the time.

#### Q2: Which `genres` have the highest `votes`?
25.5% of our dataset consists of popular votes (6,520 rows), with `Drama` being the most popular genre at over 18.5%.

#### Q3: What movie has the highest `popularity`? What is its `genre`?
`Spider-Man: No Way Home` has the highest popularity rate with genres of `Action`, `Adventure`, and `Science Fiction`.

#### Q4: Which year has the most films released?
The year `2020` had the highest filming rate in our dataset.

___

## Built with:
| Tools 		|  
| -------- 		|  
| JupyterLab	|  
| Python3	   	|  
| Pandas		|  
| Numpy			|  
| Matplotlib	|  
| Seaborn		|  


