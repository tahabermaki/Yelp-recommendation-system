# Yelp-recommendation-system

Based on a Yelp database containing multiple data sets, I'm attempting to build a recommendation system for both users and businesses

The database provided by Yelp contains a lot of useful information, whether it be with details about the businesses and their activities, as well information about the users and their involvement in terms of reviews and comments. The following link gives a detailed overview of the content of each table : https://www.yelp.com/dataset/documentation/main

## The business table

The business table contains a lot of different information about each establishement :
  - Adress and geolocalisation information
  - Some attributes about the activity of the establishement
  - The business categories that the establishement falls into
  - Opening hours
  - Reviews and grade metrics

<p align="justify">This particular table will be of the utmost importance for the first step of the analysis, which is grouping all the businesses into classes (clustering). This way, we'll be able to get a clearer idea about the different business categories in the data, as well as understand the purchasing behavior of the users and thus determine what they like and what they usually go for.</p>
  
<p align="justify">Considering how messy the data was initially, a thorough preprocessing phase was executed to extract every relevant feature, after which I used some NLP methods, as most of the data is in text format, which I followed up with a K-means to create my clusters. It is worth noting that some of the variables that were extracted proved to quite useful for the creation of these classes, notably I managed to isolate all businesses related to catering (restaurants, cafes, bars ...) from those that aren't, and thus do the clustering more efficiently.</p>
  
<p align="justify">At the end, I ended up creating 7 distinct clusters which will later come into play for the recommendation system.</p>
