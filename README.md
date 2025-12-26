# Spotify Playlist Clustering
A Python project that analyzes Spotify playlists by clustering songs based on their audio features and genres, helping you understand the vibe of long playlists without listening to every track.

# How It Works

1. Export playlist data from Spotify using Chosic's Playlist Analyzer
2. Extract audio features like BPM, energy, happiness, danceability, acousticness, and loudness
3. Encode genre diversity as an additional feature
4. Normalize all features using StandardScaler
5. Apply K-means clustering to group similar songs (default: 4 clusters)
6. Visualize clusters using PCA and t-SNE dimensionality reduction

# Tools & Libraries used in this project

- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- scipy