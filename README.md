# ETL - FIFA WORLD CUP ,COUNTRY PERFORMANCE AND RANKING

## Final files
Final pandas file -  rank_fifa-checkpoint_final_081019.ipynb

Final sql file - worldcup.sql

Final queries file - queries.sql

## INTRODUCTION
ETL is a type of data integration that refers to three steps(extract,transform,load) used to blend data from multiple sources.This process involves extracting data from a source system,converting into a format that can be analysed and stored into a data warehouse.

### DATA SOURCES 
For the ETL project we have used data from two different sources
1.Data.World
2.Kaggel
       link given here  https://www.kaggle.com/abecklas/fifa-world-cup/version/5#
                        https://data.world/jackspades42/worldcuprank/workspace/file?filename=wc_rank.csv#
  
  We got two csv files from kaggle and one csv file from Data.world
  

#### OBJECTIVE
The aim of this project was to compare the performance of the Countries in World Cup to the ranks given to them by FIFA before each tournament.
For this we use three csv files.The name of the files are listed below -
1.WorldcupMatches.csv
2.Worldcups.csv
3.wc_rank.csv

##### DATA CLEANUP AND ANALYSIS

1.WORLD CUP CSV WITH WINNER POSITIONS- The first file is the worldcup csv file used.We extracted the following columns from the csv file -
Year
Country
Winner
Runners-up
Third 
Fourth
GoalsScored

From this file we extracted the latest 5 event from 1998 to 2014.The reason to do this was that the rank file have 5 events from 1998 to 2014.


![Table showing the cleaned data for positions in World cup ](images_etl/winner_img.PNG)


2.RANK CSV -We used a file which had rank given to ech Country by FIFA.This file was used to extract rank of each country from 1998 to 2014.The rank was then added to the first file with winners position.


![Table showing the ranks ](images_etl/rank_1.PNG)

3.We made a new table using the above two table.The format of the first table to changed and rank added to it using for loop in pandas.
So we finally got the rank of the top four countries each year.

![Table showing the ranks ](images_etl/finalfile_consolidated.PNG)

4.We also wanted to find out the goals scored by each country each year.So we used another csv file .The file has been shown below

![Table showing the ranks ](images_etl/![Table showing the ranks ](images_etl/finalfile_consolidated.PNG)


















