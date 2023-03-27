## Song recommender

# Databases:
We have build a song recommender which base their recommendation in 2 databases:
- Hot songs: it has been build scraping the Billboard's top 100 song.
- Not hot songs: we took a random sample of 3000 song a huge database that can be found in the folder data as original_database.txt.

# Model:
In order to make right recommendations we got the audio features of each song from Spotify's API, then we apply some clustering model in order to classify each group of songs. We test some methods and finally pick the K-Means with K=14.

# Function:
Then we made a function which suggest recomendation regarding if the song is contained in our "hot song database" and according to our model, the function classifies the song regarding the clusters that we have and suggest a random sample of our database.

# Next Steps to follow:
- To create an app more friendly with the user.
- To add more songs to our database.
- To include additional features in the system, like genre or to make recommendations regarding the top trending songs of the user's country or the international top.
- To return to the user a plylist with the song recommended.  