# Cryptocurrencies
Cryptocurrencies
Unsupervised Machine Learning of Crytocurrency data with Scikit-learn preprocessing and KMeans clustering.Visualizations with Plotly Express and Pandas hvplot.

Challenge
Given a list of available cryptocurrencies and information such as algorithm(s) used, trading status, total coins mined and total coin supply; use unsupervised machine learning to group the cryptocurrencies into distinct and useful classifications.

Execution
Preprocessing:

Used pandas to reduce dataset of 1,252 cryptocurrencies to 532 that could be used for machine learning.
Filtered dataset by removing all currencies that are not trading, removing all currencies with no mined coins, and any records with null values.
Dataset also reduced to four fields of algorithm type, proof type, total coins mined and total coin supply.
Made necessary transformations to prepare remaining data into scaled data.
Principle Component Analysis

Used SKLearn to reduce the scaled data to three components for three dimensional modeling.

Clustering Cryptocurrencies using K-Means.

Used SKLearn Kmeans to produce an elbow curve that shows the value of '5' will serve best as the K value in the KMeans model.
Created and ran the KMeans function on the scaled and transformed data to generate a class of five clusters.
Created a combined dataset of the original filtered data with the scaled data and the cluster class values for visualization purposes.
Visualizations

Please see: Challenge_Module_18_Unsupervised_Learning.ipynb for code to generate plots.

A three dimensional Plotly Express scatter plot showing the clusters with markers identifying Coin name and Algorithm.
An hvplot table containing Coin Name, Algorithm, ProofType, Total Coin Supply and class. This data set can be used for additional analysis and visualizations by the five clusters.
A scatter plot using hv.plot presenting total coins mined and total coins supplied.
Conclusions

Bitcoin is in a class by itself. This is obvious in both the three dimensional cluster modeling and the scatterplot. This is obviously useful as Bitcoin can be studied as an exemplar.
It would be very instrumental to run this analysis again without the Bitcoin data, so see if the elbow curve finds a different optimal cluster value and so that we can see the distribution of the data better in the three dimensional plot. Essentially there are two classes, Bitcoin and all others.
We can use these findings to compare all cryptocurrencies against Bitcoin, and to re-run the unsupervised machine learning without Bitcoin to more fully understand the rest of the cryptocurrency market.
​
