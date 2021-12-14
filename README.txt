DESCRIPTION

App link: https://songseeker.herokuapp.com/
Descriptive video link: https://youtu.be/3JCVpfjqDfs

SongSeeker is an interactive web app that allows a user to submit a song and receive recommendations for similar songs via a force graph. After a user has selected a song, he can determine the extent to which various, Spotify-defined, song features take precedence for song recommendation through the use of interactive sliders. 

SongSeeker has visible sliders for each of the top 5 features as determined through clustering analysis (i.e., danceability, energy, loudness, acousticness, and instrumentalness), and the rest of the features are available via an "Edit Sliders" button. The user assigns each visible slider a value from 0-100 (default 0); the value assigned to each slider determines the weight multiplier for that feature, with larger weights being assigned to those features that the user has deemed more valuable. The default slider value of 0 corresponds to a weight multiplier of 1, and each slider that is not visible has the default slider value.

A user can change as many of the sliders as he wishes, and the final output is not be computed until he presses the “Run” button. This generates the aforementioned force graph, complete with the top ten song recommendations based on the sliders' values. The user is then free to experiment with different slider values and/or entirely different song selections.


INSTALLATION

None required; SongSeeker is a fully-functional web app.


EXECUTION

1. Visit https://songseeker.herokuapp.com/ (not recommended for use with mobile phone)
2. Type a song title into the search bar and pick from the available options.
3. Decide which sliders you would like to use via the “Edit Sliders” button. Default sliders are Danceability, Energy, Loudness, Acousticness, and Instrumentalness.
4. Move each slider to the desired number. Default value for each slider is 0; the larger each feature’s slider value becomes, the more the recommendation algorithm is weighted towards that particular feature. E.g., moving the Danceability slider to a value larger than 0 will bias the recommendation algorithm towards songs that are closer to the selected song’s Danceability value.
5. Click the “Run” button. This may take around 20 seconds.
6. Songs are displayed via a force graph in the center of the screen. The central node is the selected song; the other nodes are the recommended songs. Songs that are more highly recommended have larger nodes and are closer to the central node.
7. After hovering over a song you can: play a sample of the song, visit the song’s page on Spotify, visit the artist’s page on Spotify, or visit the album’s page on Spotify.
8. Click the “Reset” button to move the sliders back to their default values. Ghost markers show the slider values prior to reset. You must click “Run” again to see the newly recommended songs after a reset.
9. Try different values of the sliders and click “Run” for different song recommendations for the same selected song. Alternatively, go back to step 2 and start over with a new song.
10. Click the “Feedback?” button at the bottom of the screen to take a short survey about your experiences with SongSeeker.
