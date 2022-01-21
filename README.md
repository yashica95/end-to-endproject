# End-to-End Data Science Project: E-commerce Customer Lifetime Value

## Motivation: 
The project's purpose is to apply the knowledge of the data science lifecycle and build an end-to-end machine learning example of working an enterprise-grade data science problem - including problem framing, data extraction and exploration, model building and fine tuning and finally reporting the results and insights drawn from the ML model. 


## Overview: 
This project uses the Brazilian E-Commerce Public Dataset published by Olist on Kaggle to demonstrate the scoping and implementation of a real-world data science project. The dataset's description on Kaggle states:

### Context: 
This dataset was generously provided by Olist, the largest department store in Brazilian marketplaces. Olist connects small businesses from all over Brazil to channels without hassle and with a single contract. Those merchants are able to sell their products through the Olist Store and ship them directly to the customers using Olist logistics partners. 

After a customer purchases the product from Olist Store a seller gets notified to fulfill that order. Once the customer receives the product, or the estimated delivery date is due, the customer gets a satisfaction survey by email where he can give a note for the purchase experience and write down some comments.

### Data: 
The dataset has information of 100k orders from 2016 to 2018 made at multiple marketplaces in Brazil. Its features allows viewing an order from multiple dimensions: from order status, price, payment and freight performance to customer location, product attributes and finally reviews written by customers. We also released a geolocation dataset that relates Brazilian zip codes to lat/lng coordinates.

This is real commercial data, it has been anonymised, and references to the companies and partners in the review text have been replaced with the names of Game of Thrones great houses. 
More information can be found here: https://www.kaggle.com/olistbr/brazilian-ecommerce
![](https://github.com/yashica95/end-to-endproject/blob/main/data/Database%20Diagram.png)

### Goal:

The goal is to propose a supervised model that can predict the customer lifetime value (LTV) based on the purchase history of the customers. By knowing the LTV of the customers, the company can focus on the customers who have higher LTV and therefore have better ROI of marketing budget. The proposed solution will contain a csv of customers and expected LTV of the customers. 

## Project Structure: 

### Data:
The data retrieved from Kaggle as well as training and test sets.

* `data/`
   * [Original dataset and supporting documentation](https://www.kaggle.com/olistbr/brazilian-ecommerce) retrieved from Kaggle on 21st Jan, 2021
* `train.csv`
   * The dataset used for exploratory analysis to train machine learning models

* `test.csv`
   * The dataset used to evaluate the optimal model

### Models:

Serialized fine-tuned model

* `experiment-1-model.pk`
   * The final model with fine-tuned hyperparameters

### Notebooks: 

Exploratory data analysis (EDA) and building, analysing and fine-tuning the model

* `EDA.ipynb`
  * Exploratory data analysis of the given customer purchase data
  * Data wrangling, Feature Engineering
  * Testing and comparing the performance of supervised regression model
  * Fine-tuning the model and creating a serialised model object  

## Dependencies

Please download the requirements.txt file and run the following command to download the dependencies: 
```python3
pip install -r requirements.txt
```

