# Module 8: ETL - Extract, Load and Transform Movies Database Challenge

## Overview of the analysis: Explain the purpose of this analysis.
Amazing Prime loves the dataset and wants to keep it updated on a daily basis. Britta needs your help to create an automated pipeline that takes in new data, performs the appropriate transformations, and loads the data into existing tables. You’ll need to refactor the code from this module to create one function that takes in the three files—Wikipedia data, Kaggle metadata, and the MovieLens rating data—and performs the ETL process by adding the data to a PostgreSQL database.

This challenge consists of the following four technical analysis deliverables:

- Deliverable 1: Write an ETL Function to Read Three Data Files
- Deliverable 2: Extract and Transform the Wikipedia Data
- Deliverable 3: Extract and Transform the Kaggle data
- Deliverable 4: Create the Movie Database

## Challenge Desription: 
Deliverable 1:
- An ETL function is written to read in the three data files.
- The function converts the Wikipedia JSON file to a Pandas DataFrame, and the DataFrame is displayed in the ETL_function_test.ipynb file.
​- The function converts the Kaggle metadata file to a Pandas DataFrame, and the DataFrame is displayed in the ETL_function_test.ipynb file.
​- The function converts the MovieLens ratings data file to a Pandas DataFrame, and the DataFrame is displayed in the ETL_function_test.ipynb file. 

Deliverable 2:
- The TV shows are filtered out, and the wiki_movies_df DataFrame is created.
- A try-except block is used to catch errors while extracting the IMDb IDs with a regular expression and dropping duplicate IDs.
- The extraction and transformation of the Wikipedia data in the ETL function does the following:
-- A list comprehension is used to keep columns with non-null values.
-- The non-null box office data is converted to string values using the lambda and join functions.
-- A regular expression is used to match the six elements of "form_one" of the box office data.
-- A regular expression is used to match the three elements of "form_two" of the box office data.
-- The following columns are cleaned in the Wikipedia DataFrame: (8 pt)
. The box office column
. The budget column
. The release date column
. The running time column
-- The cleaned Wikipedia data is converted to a Pandas DataFrame, and the DataFrame is displayed in the ETL_clean_wiki_movies.ipynb file. (4 pt)

Deliverable 3:
- Using your knowledge of Python, Pandas, the ETL process, and code refactoring, extract and transform the Kaggle metadata and MovieLens rating data, 
- Then convert the transformed data into separate DataFrames. 
- Then, you’ll merge the Kaggle metadata DataFrame with the Wikipedia movies DataFrame to create the movies_df DataFrame. 
- Finally, you’ll merge the MovieLens rating data DataFrame with the movies_df DataFrame to create the movies_with_ratings_df.

Deliverable 4:
Use your knowledge of Python, Pandas, the ETL process, code refactoring, and PostgreSQL to add the movies_df DataFrame and MovieLens rating CSV data to a SQL database.
- The movies table has 6,052 rows and the ratings table has 26,024,289 rows, with a screenshot of each query and the output, saved as movies_query.png and ratings_query.png, respectively.



