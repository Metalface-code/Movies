# Movies

![image](https://user-images.githubusercontent.com/105470937/215615465-cefca8c6-f7cb-4900-ad9e-f08aca958ed3.png)


## The stakeholder's business problem: What makes a successful movie and can we get good recomendations from the data we have? 
 
 # Phase 1 
 
 ### The stakeholder only wanted to include information for movies based on the following specifications:

Exclude any movie with missing values for genre or runtime
Include only full-length movies (titleType = "movie").
Include only fictional movies (not from documentary genre)
Include only movies that were released 2000 - 2021 (include 2000 and 2021)
Include only movies that were released in the United States
 
 
 ## The data that was used 
 
 ### IMDB Provides Several Files with varied information for Movies, TV Shows, Made for TV Movies, etc.
### Overview/Data Dictionary: https://www.imdb.com/interfaces/
### Downloads page: https://datasets.imdbws.com/

## Phase 1 Deliverables 

After filtering out movies that do not meet the stakeholder's specifications:

Before saving, I ran a final .info() for each of the dataframes to show a summary of how many movies remain and the datatypes of each feature

Save each file to a compressed csv file "Data/ to be used in later phases. 

# Phase 2 
## The stakeholder realized that there is no financial information included in the IMDB data (e.g. budget or revenue).

### This will be a major roadblock when attempting to analyze which movies are successful and must be addressed before you will be able to determine which movies are successful.
### The stakeholder identified The Movie Database (TMDB) as a great source of financial data (https://www.themoviedb.org/). Thankfully, TMDB offers a free API for programmatic access to their data!

### The stakeholder wants to extract the budget, revenue, and MPAA Rating (G/PG/PG-13/R), which is also called "Certification".

### Specifications - Financial Data
### Your stakeholder would like you to extract and save the results for movies that meet all of the criteria established in part 1 of the project (You should already have a filtered dataframe saved from part one as a csv.gz file)

### As a proof-of-concept, they requested I  perform a test extraction of movies that started in 2000 or 2001

## Deliverables 
### How many movies had at least some valid financial information (values > 0 for budget OR revenue)?

![image](https://user-images.githubusercontent.com/105470937/219760964-e336f593-7d1a-44f3-a979-f1b2f4fe3c54.png)

![image](https://user-images.githubusercontent.com/105470937/219760777-c6aa3995-fc61-419a-b80a-a69e6cb09862.png)

### How many movies are there in each of the certification categories (G/PG/PG-13/R)?

![image](https://user-images.githubusercontent.com/105470937/219762331-51f238e8-53dd-49e4-868d-e9cbc3fc4020.png)

### What is the average revenue per certification category?

![image](https://user-images.githubusercontent.com/105470937/219762740-bec48afa-18da-4549-a4ab-cfd4e22b7681.png)

### What is the average budget per certification category?

![image](https://user-images.githubusercontent.com/105470937/219763004-9630ccea-bea8-4ab4-bf15-0d6431412558.png)






# Phase 3
## The stake holder asked for a MySQL database to be made for 2001 and 2002
### Specifically, they want the data from the following files included in your database:
Title Basics:
Movie ID (tconst)
Primary Title
Start Year
Runtime (in Minutes)
Genres
Title Ratings
Movie ID (tconst)
Average Movie Rating
Number of Votes
The TMDB API Results (multiple files)
Movie ID
Revenue
Budget
Certification (MPAA Rating)

### Derliverables 
![image](https://user-images.githubusercontent.com/105470937/219759368-e781eeef-2c28-45a8-8c94-887f5420ab95.png)

![image](https://user-images.githubusercontent.com/105470937/219759019-ccbac2d8-f113-4912-8c50-3b5100d3595c.png)

