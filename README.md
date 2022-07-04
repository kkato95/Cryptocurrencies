# Cryptocurrencies

### Overview

We are analyzing cryptocurrencie data to determine which cryptos are trading on the market and how they could be grouped to create new investment.


### Method

We are using an unsupervised learning in machine learning because there is no output we are expecting. Using the clustering algorithm, we will group the cryptocurrencies and will visualize the results.



#### Deliverable 1: Preprocessing the Data for PCA

We cleaned and tranform the crypto_data.csv:

1. dropping columns
2. sorting values
3. removing crytpos defunct algorithms
4. dropping null values
5. maintain CoinsMined in df if > 0
6. created variables for text features



#### Deliverable 2: Redcuting Data Dimentions Using PCA

1. reduced dimentions to 3 principal components
2. turned index values into a list
3. created df with the 3 components



#### Deliverable 3: Clustering Cryptocurrencies Using Kmeans

1. determine what the best value for k is using the elbow curve
2. initialize model with K=4, based on the elbow curve
3. predict clusters
4. create 'class' column based on the model and its labels
5. concat the crypto_df and pcs_df
6. concat CoinName to clustered_df



#### Deliverable 4: Visualizing Cryptocurrencies Results

1. created 3d-catter plot with clusters based on components
2. create a table with tradable crypto with hvplot
3. Scaling datat ot create scatter plot with tradable cc
4. create a hvplot.scatter plot using x="TotalCoinsMined" and y="TotalCoinSupply".



### Result Summary

3D-Scatter with Clusters

![3d_scatter](https://user-images.githubusercontent.com/99375741/177218330-2965bf43-9617-4e29-9bdb-a3da93266dad.png)




'TotalCoinsMined' and 'TotalCoinSupply' hvplot.scatter

![hvplot_coins_mined_supply](https://user-images.githubusercontent.com/99375741/177218420-2d55afdc-6765-4706-ba8d-5bbad9b269e5.png)
