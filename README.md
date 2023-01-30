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


