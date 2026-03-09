# What Makes a Song Stream? Analysing 953 Spotify Hits

## Overview
As an active musician and data scientist, I wanted to understand what separates 
a highly streamed song from the rest. This project analyses 953 of Spotify's 
most streamed songs using SQL, Python, and Tableau to uncover patterns in audio 
features, release timing, and artist behaviour across streaming platforms.

📊 [View the Tableau Dashboard](https://public.tableau.com/app/profile/reiner.rillo/viz/WhatMakesaSongStreamAnalysing953SpotifyHits/Dashboard1)

## Tools Used
- **BigQuery** — data storage and SQL analysis
- **Python (Pandas)** — data cleaning and preparation
- **Tableau Public** — interactive dashboard and visualisation

## Dataset
[Top Spotify Songs 2023](https://www.kaggle.com/datasets/nelgiriyewithana/top-spotify-songs-2023) 
via Kaggle — 953 tracks with audio features including BPM, danceability, energy, 
valence, and cross-platform chart appearances.

**Data quirks noted:**
- A small number of pre-2000 tracks appear due to catalogue re-releases
- One encoding issue with "Señorita" displaying as "Se��o" in the raw data
- Streams column required type casting from string to integer

## Key Findings

### 1. Release timing matters more than you'd think
Songs released in **September and January** average significantly more streams 
than any other month — nearly double the streams of February releases. For 
independent artists, release timing may be as important as the music itself.

### 2. Sadder songs outperform happier ones
Contrary to expectations, songs with low valence (sad/melancholic) average 
**21% more streams** than very happy songs. Emotional depth appears to drive 
repeat listening behaviour more than positivity — listeners return to music 
that resonates with them during difficult moments.

### 3. Collaborations don't guarantee more streams
Solo artists average **23% more streams than duos** and 63% more than tracks 
with 3+ artists. This likely reflects the dominance of a small number of 
mega-artists rather than collaborations being ineffective — but the data 
challenges the assumption that features always boost performance.

### 4. Platform loyalty varies dramatically by artist
Apple Music chart appearances dwarf Spotify for most artists — The Weeknd 
accumulates 7x more Apple appearances than Spotify appearances, suggesting 
distinct listener demographics across platforms. Bad Bunny is a notable 
exception, performing more evenly across both.

## The Central Insight
Across mood, energy, danceability, and release timing — the data consistently 
points in one direction. **Streaming rewards emotional depth over energy.** 
The anatomy of a highly streamed song is restrained, melancholic, and released 
in autumn or January.
