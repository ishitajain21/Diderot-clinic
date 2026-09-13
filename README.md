# Diderot Clinic

Exploration toolkit for querying Bluesky data hosted in ClickHouse (`bluesky_ingest` on `ch.bsky.diderot.app`).

## Setup

1. Create the conda environment:

```bash
conda env create -f environment.yml
conda activate diderot-clinic
```

2. Add credentials in a `.env` file at the repo root (this file is and should be gitignored to prevent crendential leakage):

```bash
CLICKHOUSE_USERNAME=your_username
CLICKHOUSE_PASSWORD=your_password
```

3. Register the kernel (optional, for Jupyter / VS Code / Cursor):

```bash
python -m ipykernel install --user --name diderot-clinic --display-name "diderot-clinic"
```

## Getting started

Start with the tutorial notebook:

- [`data_exploration/clickhouse_bluesky_tutorial.ipynb`](data_exploration/clickhouse_bluesky_tutorial.ipynb) — connect, list tables, and run example queries for the core APIs (posts, reposts, likes, follows, profiles).

Bluesky HTTP API endpoints are also summarized at [endpoints.bsky.app](https://endpoints.bsky.app/#bluesky-app).
