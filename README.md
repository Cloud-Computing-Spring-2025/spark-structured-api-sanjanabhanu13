# Spark Assignment 3: Music Listener Behavior Analysis

This assignment explores user listening patterns using PySpark's Structured API. It involves joining listening logs with song metadata, performing aggregations, filtering, and generating insights across various behavioral dimensions.

---

## Dataset Description

### `input/songs_metadata.csv`
- Metadata for songs, including:
  - `song_id`: unique identifier
  - `title`: song title
  - `artist`: artist name
  - `genre`: genre category (e.g., happy, sad)

### `input/listening_logs.csv`
- User activity log containing:
  - `user_id`: unique user identifier
  - `song_id`: the song they listened to
  - `timestamp`: when the song was played
  - `duration_sec`: how long the user listened

---

##  Tasks & Output Folders

| Task | Description | Output Folder |
|------|-------------|----------------|
| **1** | Favorite genre per user (based on frequency) | `output/user_favorite_genres/` |
| **2** | Average listen time per song | `output/avg_listen_time_per_song/` |
| **3** | Top 10 most played songs this week (Week 12) | `output/top_songs_this_week/` |
| **4** | Recommend "Happy" songs to users who often listen to "Sad" ones | `output/happy_recommendations/` |
| **5** | Genre loyalty scores: Users with over 80% listening to one genre | `output/genre_loyalty_scores/` |
| **6** | Night owl users: Listening activity between 12 AM – 5 AM | `output/night_owl_users/` |
|      | Enriched logs (original logs joined with metadata) | `output/enriched_logs/` |

---

##  Output Screenshots

Screenshots of each output (as CSVs) and task results were displayed during execution in **Google Colab** notebooks. Outputs are saved and structured correctly in the `output/` folder.

---

##  PySpark Execution (Colab)

The assignment was executed using Google Colab with PySpark installed via:

```python
!pip install pyspark
