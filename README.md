# Sql-and-Python

In this guided project, we're going to learn how to:

    Import data into SQLite
    Design a normalized database schema
    Create tables for our schema
    Insert data into our schema

We will be working with a file of Major League Baseball games from Retrosheet. Retrosheet compiles detailed statistics on baseball games from the 1800s through to today. The main file we will be working from game_log.csv, has been produced by combining 127 separate CSV files from retrosheet, and has been pre-cleaned to remove some inconsistencies. The game log has hundreds of data points on each game which we will normalize into several separate tables using SQL, providing a robust database of game-level statistics.

In addition to the main file, we have also included three 'helper' files, also sourced from Retrosheet:

    park_codes.csv
    person_codes.csv
    team_codes.csv

These three helper files in some cases contain extra data, but will also make things easier as they will form the basis for three of our normalized tables.

An important first step when working with any new data is to perform exploratory data analysis (EDA). EDA gets us familiar with the data and gives us a level of background knowledge that will help us throughout our project. The methods you use when performing EDA will depend on what you plan to do with the data. In our case, we're wanting to create a normalized database, so our focus should be:

    Becoming familiar, at a high level, with the meaning of each column in each file.
    Thinking about the relationships between columns within each file.
    Thinking about the relationships between columns across different files.

We have included a game_log_fields.txt file from Retrosheet which explains the fields included in our main file, which will be useful to assist our EDA. You can use !cat game_log_fields.txt in its own Jupyter cell to read the contents of the file.

If you're not familiar with baseball some of this can seem overwhelming at first, however this presents a great opportunity. When you are working with data professionally, you'll often encounter data in an industry you might be unfamiliar with - it might be digital marketing, geological engineering or industrial machinery. In these instances, you'll have to perform research in order to understand the data you're working with.

Baseball is a great topic to practice these skills with. Because of the long history within baseball of the collection and analysis of statistics (most famously the Sabermetrics featured in the movie Moneyball), there is a wide range of online resources available to help you get answers to any questions you may have.

Let's get started exploring the data by using pandas to read and explore the data. 
