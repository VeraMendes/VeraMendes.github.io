---
layout: post
title: The Trash Panda
image: img/trash_panda2.PNG
---

From all the projects I worked on as a Data Scientist, The Trash Panda is the project I feel more passionate about.
The Trash Panda was a project idea that was submitted by one of my colleagues in the Data Science program, Trevor. When I initially saw the project proposal, I thought maybe ambitious but a great idea, and I would like to be part of it.

![](/img/trash_panda.PNG)

Recycling is not as straightfoward as we wish, The Trash Panda main objective is to make this task easier and quicker.

How does it work?  
Different countries, states, counties, cities have different regulations which makes the recycling process really hard and even frustrating.  
To help the users and consequentely the environment, *The Trash Panda comes* in the game. 
The application uses your location to provide you with correct disposal information if you are in the US, still if you are not in the US or decide not to share location, you get good tips and information about general recycling of your items.  
You can look out for materials via a category exploration, search bar or via AI image recognition using your camera to take a photo of the object to dispose. The AI technology recognizes the item and correct disposal information will be provided. 

This application is meant for mobile devices and can be found on the <a href="https://play.google.com/store/apps/details?id=com.thetrashpanda.twa" target="_blank">Google Play Store</a> for android users. 
IOS users will be able to use it on Safari.

What was my role in this application? How did I fit in this team?  
Our <a href="https://thetrashpanda.com/splash/team" target="_blank">team</a> consists of two UX designers, fours Web developers and four data scientists.   
As a Data Scientist, I focused on the image recognition side of this application. The Data Science goal was to be able to train an AI image recognition model that could identify different classes of objects.

Inittialy, we worked on a pipeline auto-annotation tool that helped us pre-processing the images. 
The tool was able to: 
1. rename the images based on md5sum, avoiding duplicates
2. resize the images to take a resonable space in memory
3. discern between transparent background and non transparent background
4. remove background from images with background
5. automate bounding boxes to identify the object
6. add background to images with no background

I was responsible for the first two points of this tool, <a href="https://tclack88.github.io" target="_blank">Trevor</a> took care of points 3 & 5, <a href="https://www.gamesbytim.com/p/home.html" target="_blank">Tim</a> took care of point 6 and implementing the image downloader and <a href="https://tobias.fyi/" target="_blank">Tobias</a> worked on point 4 and the API.   
Then we collected images in various ways from the web, each of us had around 17 classes and 1K+ images per class to take care of.    
We passed the images through the auto-annotation tool and then adjusted mannualy with *labelImg*.  
The dataset was saved in a S3 bucket on AWS and then using an AWS EC2 instance, we runned our images though an ANN model using YOLO and darknet framework.  
Our weights reached a total  average precision of 54.71% within 2.5 days, breaking down into classes, there are some classes with a lower average precision due to the variety of object forms and colors but some other classes had great average precision such as ~95%.  

Our project was presented in the cohort and was selected to be presented school wide on a Lambda School version of the Shark Tank. You can watch the final presentation in the following video:  
<iframe width="100%" height="360" src="https://www.youtube.com/embed/7g_kUKm5QIY?start=1365" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>




