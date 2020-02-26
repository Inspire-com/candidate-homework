# Data Engineer Interview

## SQL Analysis Challenge

### Description
This is a series of questions designed to test your familiarity with SQL filtering, joining, and aggregations.

We are going to use the kaggle dataset about soccer to do some SQL analysis. The dataset can be downloaded from the `data` directory as `soccer.zip`. You will need to unzip this database. It is about 300mb in size. If you would like more information about the types of data (and the relationships between them), you can look at this [link](https://www.kaggle.com/hugomathien/soccer/version/1) -- however, please DO NOT use the database at the provided link, as the one provided in the data directory has been modified to handle NULLs more efficiently.

### Questions to answer

1. Tell me the full name and player_id of the player with the highest combined shot_power and free_kick_accuracy who happens to be left-footed
2. Get me the roster (list of player names) for each team, where "roster" is defined as the players listed for the team's most recent home game
3. [BONUS / Extra Credit] For each player that has been a member of more than 3 teams, return the player name, the team name, and the number of matches they have played for each team

#### Inputs
 - The SQLite DB is provided as input

#### Outputs
 - The outputs will be a set of .sql files with the SQL query required to solve the problem. The goal is to test your SQL skills, so if the answers to the question are provided in python / pandas / another language, it will not be counted.
- For each of the questions, please also provide results of the SQL query in a .tsv or .csv file. If you do not know how to do this, please provide the raw results in a .txt file
- [BONUS / Extra Credit]: Use SQL comments to describe the logic so that it would be understandable to a teammate. 

#### A couple tips
- You can use the `.schema ` or `.schema <tablename>` command in the sqlite console to see the schema for each sql table.

---

## API Server Project

### Description

Build an API server in any language of your choosing (you are allowed to use a web-app skeletons / templates created beforehand) that uses the National Data Buoy Center Dataset to compute the following:

#### Inputs

- These are all stations that we can get data from: https://www.ndbc.noaa.gov/to_station.shtml
    - An example link to get the Real time standard meteorological data for the last 45 days: https://www.ndbc.noaa.gov/station_realtime.php?station=42035
- Useful description of the fields returned by the data: https://www.ndbc.noaa.gov/measdes.shtml#stdmet


- given a STATION_ID, we want to pull the last 45 days of historical data for that buoy and return the largest 4 recorded waves in that height
- Each wave should include the unique day/month/year of when it was recorded. Each day should only return the largest wave for that day. In other words, if 2 of the largest waves happened in the same day, return the max from that day's waves. 
- You can expect the user to pass in a valid STATION_ID
- There may be no data available for a station in the past 45 days, or null values for some of the fields. Please handle accordingly and read the data descriptions _carefully_!
- [Bonus / Extra Credit]: Try to do this exercise without using external libraries. What is the runtime complexity of your application? What is the minimum bound necessary to compute this operation? Be prepared to discuss your solution in person. 
