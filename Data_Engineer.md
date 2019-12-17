# Data Engineer Interview

## Python Data Slice n' Dice Challenge (30-60 minutes)

### Description

This challenge involves munging a CSV of data to answer a few questions the product team has. You may do the exercise
in the language you are most comforatble with -- doing it in python or pandas gets bonus points!

### Questions to answer

1. For each row of the CSV, please convert the "genres" string into a list. Return a list of the rows, with the genres field modified. Return type List[List[String, Int, String, Int]]
2. What are all the unique genres of movies? Return type: List[String]
3. How many movies are there per genre? Return type:  Dict(String->Int)
4. Given a genre, return the list of movies from that genre. Return type: Dict(String->List[String])
5. For each year available, what are the top 5 grossing movies? Return both the movie name and the gross revenue for each result. Return type: Dict(Int -> Tuple(String, Int))
6. From the previous result, return the top 3 largest grossing movies (regardless of year). Return type: List[Tuple(String, Int)]
7. What are the top 10 biggest flops (i.e. movies that had the lowest revenue)? Return type: List[Tuple(String, Int)]
8. Of these 10 flops, what genres did they belong to? Return type: Dict[String->List[String]]
9. What was the year with the most flops? Return type: Int
10. What was the genre with the most flops? Return type: String
11. For each genre, What are the top 5 most common words used in the movie titles? Return type: dict(string->List[string]).

## SQL Analysis Challenge (30-60 minutes)

### Description

We are going to use the kaggle dataset about soccer to do some SQL analysis. The dataset can be downloaded here: https://www.kaggle.com/hugomathien/soccer/version/1 or from the `data` directory as `soccer.zip`. You will need to unzip this database. It is about 300mb in size.

This is a sqlite database, which has its own quirks but is easily installable on most systems. You are allowed to google and test out as much as you’d like (just share your screen so we can observe your problem solving process).

This is a series of questions designed to test your familiarity with SQL filtering, joining, and aggregations.  

#### A couple tips

You can use the `.schema ` or `.schema <tablename>` command in the sqlite console to see the schema for each sql table.

### Questions to answer

1. Tell me the name of the player who has the highest left-footed (`preferred_foot`), shot_power and free_kick_accuracy
2. Get me the roster (list of player names) for each team
3. BONUS: For each player that has been a member of more than 3 teams, tell me the player name, the team name, number of matches they have played for each team

#### Notes for the interviewer:

- Solutions for these queries are in the google doc: https://docs.google.com/document/d/1hzdCnx9QKWl4bBd9M4H-pr7JUUJVL3OWbVvUQ6V9zoI/edit?usp=sharing

## API Server Project

### Description

Build an API server in any language of your choosing (you are allowed to use a web-app skeletons / templates created beforehand) that uses the National Data Buoy Center Dataset to compute the following:

- given a STATION_ID, we want to pull the last 45 days of historical data for that buoy and return the largest 4 recorded waves in that height
- Each wave should include the unique day/month/year of when it was recorded. Each day should only return the largest wave (i.e. only one value per day)
