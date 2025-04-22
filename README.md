# Spotify SQL Analysis 

This project explores Spotify music data using SQL and SQLite, powered by DBeaver for querying and visualization.
As well as featuring a dashboard to visualize the trends that were found in 2023. 
## Project Structure

- `data/` - Raw CSV dataset(s) from Kaggle.
- `database/` - SQLite database with imported data.
- `dashboard`-PowerBI dashboard "spotify_dashboard.pbix"
- `queries/` - SQL scripts for analysis (e.g. popularity trends, genre breakdown).
- `README.md` - You’re here!

## Dataset Source
[Spotify Dataset (Kaggle)](https://www.kaggle.com/datasets/nelgiriyewithana/top-spotify-songs-2023)
[Supplementary dataset (Kaggle)](https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset)

## Tools Used
- SQLite
- DBeaver
- GitHub
-Power BI
## Sample Queries

```sql

-- Most popular tracks
SELECT track_name, "artist(s)_name", streams 
FROM spotify s 
ORDER BY streams DESC
LIMIT 10;
-- Popularity over time
SELECT track_name ,released_year , AVG(streams) AS avg_popularity
FROM spotify s 
GROUP BY released_year 
ORDER BY released_year ;
```
