# Spotify SQL Analysis 

This project explores Spotify music data using SQL and SQLite, powered by DBeaver for querying and visualization.

## 📂 Project Structure

- `data/` - Raw CSV dataset(s) from Kaggle.
- `database/` - SQLite database with imported data.
- `queries/` - SQL scripts for analysis (e.g. popularity trends, genre breakdown).
- `README.md` - You’re here!

## 📊 Dataset Source
[Spotify Dataset (Kaggle)](https://www.kaggle.com/datasets/nelgiriyewithana/top-spotify-songs-2023)

## 🛠 Tools Used
- SQLite
- DBeaver
- SQL
- Git + GitHub

## 🧪 Sample Queries

```sql

-- Most popular tracks
SELECT track_name, "artist(s)_name", streams 
FROM spotify s 
ORDER BY streams DESC
LIMIT 10;
