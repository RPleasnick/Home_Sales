# Home_Sales
 Module 22: Big Data



## Overview


_Home_Sales_colab.ipynb_ pulls the dataset from _https://2u-data-curriculum-team.s3.amazonaws.com/dataviz-classroom/v1.2/22-big-data/home_sales_revised.csv_.  The average price for a house was calculated given different criteria.  The spead of a calculation was also observed when using a temporary view, when cached data is used, and when the parquet DataFrame is used.


## Results

The average price of a four-bedroom house sold:

![Screenshot 2024-08-10 211152](https://github.com/user-attachments/assets/b49b6aca-d640-4be7-92b3-dc9d09856432)


The average price of a home that has three bedrooms and three bathrooms, by the year it was built:


![Screenshot 2024-08-10 211225](https://github.com/user-attachments/assets/292fcc8d-b5af-42ed-9c73-84809b814636)


The average price of a home that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet, by the year the home was built:


![Screenshot 2024-08-10 211249](https://github.com/user-attachments/assets/68f429d0-2b8e-458d-b295-785737f0abae)



When the average price of home priced greater than or equal to $350,000 grouped by "view" was calculated, the run time was: 

+ 1.159203290939331 seconds using a temperary view

+ 0.5786299705505371 seconds with cached data

+ 0.9989454746246338 seconds with a parquet DataFrame

## Summary

As seen from the run time, calculations using the cached data was the quickest.  The next quickest calculations used the parquet DataFrame.
