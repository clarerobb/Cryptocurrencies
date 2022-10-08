# Cryptocurrencies with Unsupervised Machine Learning

## Overview 
The client, Accountability Accounting, is interested in offering a new cryptocurrency investment portfolio for customers. This analysis uses unspervised machine learning to group cryptocurrencies that are on the trading market to create a classification system for Accountiablity Accounting. The data was first cleaned and the data dimensions were reduced using PCA. Then, the data was grouped using K-means and vizualized with hvplot and plotly. 

## Resources
**Data Source:** crypto_data.csv <br>
**Resources:** Python 3.7.13 (pandas, sklearn, hvplot, and plotly libraries), Jupyter Notebook 6.4.8

## Results

After the data was preprocessed to fit machine learning models, there was a total of 532 tradabele cryptocurrencies. 

#### Clustering Cryptocurrencies
The K-means algorithm clustered the cryptocurrencies into four classes (see below). <br>
![Screen Shot 2022-10-08 at 12 45 22 PM](https://user-images.githubusercontent.com/106405775/194721631-e3280585-afff-4b73-9ddd-e7af0569f927.png)

#### 3D Scatter Plot
PCA reduces the number of dimensions of datasets to increase preformance and interpretablity while minimizing information loss. After the data was cleaned in the preprocessing stage, the PCA algorgithm reduced the data's dimensions to **3 principal components.** The 3D scatter plot's axes are the 3 principal components, and the plots are grouped based on one of the four classes. <br>
![Screen Shot 2022-10-08 at 12 45 50 PM](https://user-images.githubusercontent.com/106405775/194721949-8eea5a0e-9a65-4242-93c5-99f48a90d55c.png)

#### Tradable Cryptocurrencies Table
The tables below shows all tradable cryptocurrencies with basic information like the algorithm, total coins mined, and class. <br>
![Screen Shot 2022-10-08 at 1 36 50 PM](https://user-images.githubusercontent.com/106405775/194722676-bbdb150e-d894-4cc4-900a-15eb869f08e4.png)

#### Scatter Plot with `TotalCoinMined` vs. `TotalCoinSupply`
The 2D scatter plot visualizes each cryptocurrencies' `TotalCoinMined` and `TotalCoinSupply` dimensions and orders them by class. However, unlike the 3D scatter plot, this graph does not efficiently segregate the different classes meaning the primary components works better to visualize the data. <br>
![Screen Shot 2022-10-08 at 1 41 58 PM](https://user-images.githubusercontent.com/106405775/194723008-84af69a7-ae82-48be-a972-df588e0e063c.png)



