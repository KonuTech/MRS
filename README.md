Movie Recommender System


The primary goal of the project was to develop Movie Recommender System. However before that could have been possible development of Data Science Pipeline turn out to be needed too.

Being aware of additional challanges the final strategy involved following objectives:
•	scrapping the data from web,
•	storing the data as RDMS,
•	building views for data exploration and data visualisation,
•	development of few classifiers.

To scrap the data I have used API service provided by themoviedb.org . Desiging scrappers of iterative nature proved to be very helpful since each query returned single JSON document. The collections of documents were appended and saved under following data sets: Movies, Genres, Production Countries, Keywords, Cast, and Crew . Predefined SQLite views were used to clean the outputs once each new batch of data entries was appended to already stored data. Hence to above the data sets used for later data processing -  including multiple joins - stored only unique rows. Once the amount of downloaded data turned to be large enough  the Exploratory Data Analysis was perfomed to familliarize myself with information collected .
	
Although development of classifiers was not expected or even used by recommender engines the part is added to exhaust the list of steps expected from typical Data Science Pipeline. Decission trees, logistic regression, neural networks, and XGBOOST classifiers were provided mainly to enhance exploratory part of the project .

Content Based Recommenders  and Collaborative filtering  are perceived as two major methods for building recommender systems. Although both are used and assessed in the project the combination of the two called Hybrid  method  was not successfuly explored due to lack of data.

Both primary and secondary objectives of the project are dimed to be achieved.
