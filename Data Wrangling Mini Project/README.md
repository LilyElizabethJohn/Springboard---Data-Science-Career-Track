SpringBoard Data Science Career Track

JSON Excercise

Goal - Read in JSON dataset, Normalize dataset, Replace missing values and Create aggregate counts

Demonstrates reading in a json file as a string and as a table

Uses file containing data about projects funded by the World Bank 

Data source: http://jsonstudio.com/resources/

Using data in file 'data/world_bank_projects.json',
1) Find the 10 countries with most projects
2) Find the top 10 major project themes (using column 'mjtheme_namecode')
3) In 2. above you will notice that some entries have only the code and the name is missing. Create a dataframe with the missing names filled in.

Approach
1) Read JSON into a DataFrame
2) Use groupby to get project count and get top 10 countries
3) Read JSON file as string to flatten nested dictionary
4) Normalize data
5) Get top 10 major project themes by using groupby on mjtheme_namecode
6) Map in missing theme names by getting a unique combination of code and name from the original dataset
7) Redo top 10 major project themes including the mapped in theme names
8) Remove duplicate associations of id and project theme code
9) Re calculate top 10 major project themes and compare-contrast
