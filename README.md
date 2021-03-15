# Capstone Project 1: Car Price Analysis
![](images/Introduction.png)

In this work, we looked at the price of different cars across several states (i.e., Texas, California, and New York State).
* fsd

## Web Scraping
In this project, we started to web scrape the CARMAX website. The file that used to scrape the website is called "Test_scraping.ipynb". It is worth mentioning that two popular car brands (Ford and Toyota) currently availble for sale on CARmax in Texas, California, and New York state between the years of 2012-2020 were the filtering criteria for data extraction.


The follwoing figure shows the summary of the workflow:

<img src="images/Workflow.jpg" width=800 height = 400>

As can be seen, BeautifulSoup is used to scrape the data from CARmax website. Then, the scraped data is stored in Mongo database. Afterwards, python libraries were used for data cleaning, analysis, and visualization. 


## EDA Analysis
After loading the data into pandas dataframe format, we performed data-preprocessing on the data and made sure that the formatting and values are reasonable. The following tasks are examples of data preprocessing job that has been done:
* **Remove Outliers**: Price, Model, Depreciation value
* **Handle Null Values**: Remove/replace values based on the feature importance
* **Handle columns data type**
* **Grouping**: Grouping columns based on car make, model, and year

Features that were extracted and used in this study include:
* Car mileage
* Car price
* Car mpg
* Car model
* Car model year
* Car make
* Car color
* Car transmission type
* Car engine size
* Car horse power
* Car engine cylinder
* Car msrp price
* State




## Data Insights


![](images/Mileage_per_state.png)

* Average miles driven per year for each state:
    * TX: 9,900 miles
    * CA: 9,200 miles
    * NY: 8,900 miles
    * US Department of Transportation: 13,500 miles



![](images/Ford_Toyota.png)



## Statistical Analysis
###  

The analysis would help in evaluating/comparing the impact of car features on car price. 



![](images/Age_depreciation.png)
![](images/Car_Distribution.jpg)



### Statistical Analysis-Q1
**Is the average listing price of Ford Explorer in TX, CA, and NY different**

![](images/Ford_Explorer_state_price.png)




### Statistical Analysis-Q2
**Is the average listing price different for different colors? (Black/Gray/White)**

![](images/Price_color.png)

![](images/P_Value_Car.png)




## Future Work
* Include more car data from CARmax into the database
* Include data from other used car retailers
* Web scraping the CARFAX dataset to include the # of accidents and services for each car
* Apply machine learning algorithms to predict the price of cars on CARMAX
