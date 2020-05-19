---
layout: post
title: Spotify Song Suggester
---

This project was developped as part of the Lambda School Build Week Projects by a team of members from different tracks.
My main responsability in this project was as a Machine Learning Engineer with two other colleagues creating a model that could easily suggest you songs based on a specific song or a list of favorite songs.
Our objective was to make sure the suggested songs would be ideal based on the user taste. 
Exploring data, we found a data set on Kaggle called Spotify Audio Features Dataset that looked ideal, but when using it, with Natural Language Processing and a K-Nearest Neighbors model, we realized that was not enough to be accurate.
Together we decided to do some extra exploration and that is when we added the web scrapped genres to our dataset. This extra feature made a huge difference in our model accuracy, by testing we could realize the model was working much better giving out suggestions.
This model was brought forward and we created some visualization of the songs with a radar graph that looked amazing to show the musics' features. 

![](/img/spotify.PNG)

![](/img/spotify2.PNG)

Together with the Data Engineer team, we worked on making sure the model would work well on our Back-End API.
We achieve the expected results and were quite happy with them, but the Front-end of the application unfortunatelly did not come forward.

Our DS API with respective notebooks can be found <a href="https://github.com/VeraMendes/Spotify-Song-Suggester-Data-science" target="_blank">here</a>.
