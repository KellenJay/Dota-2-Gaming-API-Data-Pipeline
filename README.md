
# Dota 2 OpenDota API Data Pipeline

This project builds a complete data pipeline using Python and the OpenDota API to extract, transform, and analyze player and match data from Dota 2.

## Project Goals

- Analyze performance metrics (GPM, XPM, kills, deaths, assists) at the player and hero level
- Enrich match data with hero, item, game mode, and region constants
- Prepare clean, structured datasets for downstream analytics and ML models
- Build a scalable ETL architecture using modular scripts and a Kimball-style schema

## What’s Been Done

- ✔️ 12,000+ player-level records pulled across 1,100+ matches
- ✔️ Live match data and hero usage tracking
- ✔️ Rankings and distributions normalized for tier analysis
- ✔️ Constants data (heroes, items, game modes, regions) fetched for joins
- ✔️ EDA, validation, and profiling completed

## Next Steps

- [ ] Modularize ETL pipeline (`extract.py`, `transform.py`, `load.py`)
- [ ] Define star schema and load into SQL database
- [ ] Add scheduler (e.g., Airflow) for automation
- [ ] Deploy BI dashboard for visual insights

## Sample Datasets

- `match_details_500matches.csv`
- `live_matches_players.csv`
- `heroes.csv`, `items.csv`, `game_modes.csv`, `rankings_hero11.csv`

## API Used

- https://docs.opendota.com/

