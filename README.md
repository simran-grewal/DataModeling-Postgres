## Data Modeling with Postgres and ETL pipeline using Python for Music Streaming app
### Project Description
Data is extracted from a directory of JSON logs on user activity and a directory with JSON metadata on the songs in the app. Database is consisted of mainly five tables (songplays, users, songs, artists, time) and is designed to optimize queries on song play analysis. Songplays is the Fact table while other four are Dimension tables.

### Run the Project
Open the terminal and go inside the project directory and run the following commands

#### This will execute the queries to create tables (structure of tables is defined in sql_queries.py)
```
python create_tables.py 
```
#### This file will extract the data from JSON files and transform it  according to the tables and then load the data into tables
```
python etl.py
```

You can use test.ipynb file to check the data stored in tables.
