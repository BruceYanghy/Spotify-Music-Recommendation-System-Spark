# Spotify Muisc Recommendation System

The goal of this project is to build a song recommendation system for users of Spotify with their streaming history. The models are evaluted by how well they rank the songs in the test set.

The source data was provided by the company Spotify from Kaggle. 

## Datasets
([tracks.csv](tracks.csv)) - Contains the collection of the data where the customer is listening to a track, one event per line. The various attributes present in the dataset are
* Event ID : The unique identifier of the event where the customer is listening to the track (Integer)
* Customer ID : The customer Id of the customer listening to the track (Integer)
* Track ID : The track Id of the track currently being played (Integer)
* DateTime : The date and tim, the customer is listening to the track (String)
* Mobile : 1, if the customer is listening to the track on a mobile device else 0 (Integer)
* Listening ZIP : The approximate Zip location of the customer listening to the track (Integer)

([cust.csv](cust.csv)) - Contains the details about the customer
* Customer ID: The unique identifier of the customer (Integer)
* Name, Gender, Address, Zip : The information associated with the customer (String, Integer, String, Integer)
* Sign Date : The date the customer has been added to the service (String)
* Level : The level of subscription of the customer 0, 1, 2 for Free, Silver and Gold, respectively (Integer)
* Other fields: Which we are not interested in this example

([music.csv](music.csv)) - Contains the details about the song
* Track ID: The unique identifier of the tracker (Integer)
* Title: The Name of the track (String)
* Artist: The Artist of the track (String)
* Length: The Length of the track (Integer)




The project was built with Spark on Databricks platform.

The models are evaluated by the __Expected Percentile Ranking__, introduced by the backup paper for Spark MLlib ALS package for implicit feedback datasets [click here to view](http://ieeexplore.ieee.org/document/4781121/).

The project is carried out in 7 steps:
* Data Loading 
* Data Cleaning	
* Data Exploration		
* Model Evaluation
* Benchmarks		
* Build ALS Explicit Model	
* Build ALS Implicit Model	

Code with results are viewable at the links: [[__Part I__]](https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/6373109224204649/3283764495853970/2920490540025139/latest.html)  

A detailed explaination of the project is in the presentation.pdf file.
