---
layout: page
title: Projects
---


## The Trash Panda

This app applies image recognition AI,training an Artificial Neural Network to identify recyclable materials and other waste objects. 
On the application you can use a search bar, click-through categories, or the image recognition AI to identify and properly recycle your trash item. Disposal information will be provide based on user location.
I worked in a brilliant team of four Web Developers, another three Data Scientists and two UX Designers. We worked together researching, preparing, finding the best tools to use, defining important aspects of the application and making sure all pieces would connect properly in one only application. We took many decisions and as a group our decisions were stronger and solidified.

For the Data Science portion, we had a few different specific phases: develop an Image Auto Annotation Tool, collect and preprocess images for training, train the Artifical Neural Networks and present the final results, develop the Flask back-end API to send results to the front-end.
For our Image Auto Annotation Tool we put together a few scripts and then worked together to merge them: naming script to improve unique naming and avoid duplicates, resizing script to reduce dimensionality of images and save space, discern images script to check image images have background or not, an add background script to add background for the images with no background, a forecut Mask R-CNN to remove background of images with background and a bounding box script. I worked mostly in the first two scripts and into merging all the scripts together. 
All of us, in the Data Science part of the team,had to collect, pass our images through the Auto Annotation Tool and adjust manually with labelIMG the labels. We had nearly 70 classes to identify with a minimum of 1000 images per class, all divided by the four of us. It was a tough process but very well accomplished. To make sure we would have enough time to finish everything, one of my colleagues took care of the API, while we work on the pending images and training the model. I set up our S3 bucket and investigate the EC2 instances on AWS and then worked in training the ANN with one of my colleagues to make sure we would have results in the expected time. Our training stopped earlier than we would like, due to budget constrictions but still we were able to get 54.71 % of mean average precision as a final total with some classes very well identified.  

<a href="https://github.com/VeraMendes/trashpanda-ds/" target="_blank">GitHub DS repository</a>

<a href="https://github.com/VeraMendes/trashpanda-ds-api" target="_blank">GitHub DS API repository</a>

<a href="https://play.google.com/store/apps/details?id=com.thetrashpanda.twa" target="_blank">Progressive Web Application on Google store</a>

<a href="https://thetrashpanda.com" target="_blank">The Trash Panda website</a>

<a href="https://www.youtube.com/watch?v=kB3NLykXT6A&feature=youtu.be" target="_blank">The Trash Panda app demo</a>


## Spotify Song Suggester

A simple Back-end Flask API to suggest spotify songs in the Spotify Song Suggester app based on a track_id chosen by the user or a list of favorite songs. The API utilizes the Spotify Audio Features dataset, uploaded to Kaggle joined with webscraped genre. A KNN model that utilizes Natural Language Processing was integrated into the Flask app.

<a href="https://github.com/Build-Week-Spotify-Song-Suggester-1/Data-science" target="_blank">GitHub DS API repository</a>


## MediZen

A simple back-end Flask API that utilizes Natural Language Processing to provide recommended cannabis strains in the MediZen app based on desired effects.

<a href="https://github.com/VeraMendes/medizen_ds_api" target="_blank">GitHub DS API repository</a>


## Twitoff

Toy app that consumes data from Twitter API. The app receives a tweet, and utilizing basilica.ai sentence embeddings, it compares between two users, who is more likely to write that specific tweet.

<a href="https://github.com/VeraMendes/veramendes-twitoff" target="_blank">GitHub repository</a>

<a href="https://veramendes-twitoff.herokuapp.com/" target="_blank">Flask Web Application</a>


## Life expectancy: how Past trends influences the Future?

A data analysis on life expectancy based on past trends applying and investigating different Machine Learning models. Results were communicated via a Blog Post and a Dash Plotly Web application.

<a href="https://github.com/VeraMendes/Life-expectancy-project" target="_blank">GitHub repository</a>

<a href="https://medium.com/@veramendes10/life-expectancy-how-past-trends-influences-the-future-4e0dc2a3c4fd" target="_blank">Medium Blog Post</a>

<a href="https://life-expectancy-project.herokuapp.com/" target="_blank">Dash Plotly Web Application</a>
