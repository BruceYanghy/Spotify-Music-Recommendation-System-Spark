# MusicBox

The goal of this project is to build a song recommendation system for users of MusicBox App with their listening and downloading history. The models are evaluted by how well they rank the songs in the test set.

The source data was provided by the company, which are play logs and download logs from 3/1/2017-5/12/2017. The data covers about 0.8 million users and 2 million songs. Because of the large size of the data, the project was built with Spark on Databricks platform.

The models are evaluated by the __Expected Percentile Ranking__, introduced by the backup paper for Spark MLlib ALS package for implicit feedback datasets [click here to view](http://ieeexplore.ieee.org/document/4781121/).

The project is carried out in 7 steps:
* Data Loading 
* Data Cleaning	
* Data Exploration		
* Model Evaluation
* Benchmarks		
* Build ALS Explicit Model	
* Build ALS Implicit Model	

Code with results are viewable at the links: [[__Part I__]](https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/8629604074238764/1737319951745339/1974396095314527/latest.html)  [[__Part II__]](https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/8629604074238764/1737319951745432/1974396095314527/latest.html)

A detailed explaination of the project is in the presentation.pdf file.
