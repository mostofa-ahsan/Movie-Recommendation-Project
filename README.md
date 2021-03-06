# Movie Recommendation

### click here for the web application demo
https://mostofa-movie-recommendation.herokuapp.com/

Source Code: https://github.com/mostofa-ahsan/Movie-Recommendation-Project
 

## Project details

Content Based Recommender System recommends movies similar to the movie user likes and analyses the sentiments on the reviews given by the user for that movie.

The details of the movies(title, genre, runtime, rating, poster, etc) are fetched using an API by TMDB, https://www.themoviedb.org/documentation/api, and using the IMDB id of the movie in the API, I did web scraping to get the reviews given by the user in the IMDB site using beautifulsoup4 and performed sentiment analysis on those reviews.

## Note

Don’t worry if the movie that you are looking for is not auto-suggested. Just type the movie name and click on “enter”. You will be good to go even though if you made some typo errors.

 

## How to get the API key

Create an account in https://www.themoviedb.org/, click on the API link from the left hand sidebar in your account settings and fill all the details to apply for API key. If you are asked to give a URL for the website, just give “NA” if you don’t have one. You will see the API key in your API sidebar once your request is approved.


 

Sources of the datasets
IMDB 5000 Movie Dataset
The Movies Dataset
List of movies in 2018
List of movies in 2019
List of movies in 2020
 

##How the similarity works??

How does it decide which item is most similar to the item user likes? Here we use the similarity scores.

It is a numerical value ranges between zero to one which helps to determine how much two items are similar to each other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.

 

How the cosine similarity works??

Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, higher the cosine similarity.

![Cosine](https://user-images.githubusercontent.com/34641108/96538357-fb29a100-125d-11eb-81e6-35f8f55d7a00.PNG)


### More about Cosine Similarity :
Understanding the Math behind Cosine Similarity
https://www.machinelearningplus.com/nlp/cosine-similarity/
