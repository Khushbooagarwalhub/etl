# ETL - FIFA WORLD CUP ,COUNTRY PERFORMANCE AND RANKING

## INTRODUCTION
ETL is a type of data integration that refers to three steps(extract,transform,load) used to blend data from multiple sources.This process involves extracting data from a source system,converting into a format that can be analysed and stored into a data warehouse.

### DATA SOURCES 
For the ETL project we have used data two different sources
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
1.WORLD CUP CSV - The first file is the worldcup csv file used.We extracted the following columns from the csv file -
Year
Country
Winner
Runners-up
Third 
Fourth
GoalsScored

From this file we extracted the latest 5 event from 1998 to 2014.The reason to do this was that the rank file have 5 events from 1998 to 2014.























