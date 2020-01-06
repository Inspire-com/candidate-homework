# Data Engineer Interview

## SQL Analysis Challenge

### Description

We are going to use the kaggle dataset about soccer to do some SQL analysis. The dataset can be downloaded here: https://www.kaggle.com/hugomathien/soccer/version/1 or from the `data` directory as `soccer.zip`. You will need to unzip this database. It is about 300mb in size.

This is a sqlite database, which has its own quirks but is easily installable on most systems. You are allowed to google and test out as much as you’d like (just share your screen so we can observe your problem solving process).

This is a series of questions designed to test your familiarity with SQL filtering, joining, and aggregations.

For each of the questions below, please provide the SQL query AND the results for the question.

#### A couple tips

You can use the `.schema ` or `.schema <tablename>` command in the sqlite console to see the schema for each sql table.

### Questions to answer

1. Tell me the name of the player with the highest combined shot_power and free_kick_accuracy who happens to be left-footed
2. Get me the roster (list of player names) for each team
3. For each player that has been a member of more than 3 teams, return the player name, the team name, and the number of matches they have played for each team

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
