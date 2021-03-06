# Amazon_Vine_Analysis

## Overview of the analysis:

The purpose of this project is to analyze customer review dataset from Amazon. Using PySpark, the ETL process is performed to extract the dataset, transform the data, and connect to an AWS RDS instance. The transformed data is then loaded into pgAdmin.Then  determine if there is any bias toward favorable reviews from "Amazon Vine" members in the dataset.

## Results: 

Finally, two more DataFrames are created to separate Filter  between reviews written as part of the Vine program (paid) and reviews not part of the Vine program (unapid). After creating these final DataFrames, the following metrics are determined:

- The total number of reviews.
- The number of 5-star reviews.
- The percentage of 5-star reviews (Paid and Unpaid).


![image](https://github.com/NadaAdem/Amazon_Vine_Analysis/blob/main/Resources/total.png)

 ### Paid Review 
 
![image](https://github.com/NadaAdem/Amazon_Vine_Analysis/blob/main/Resources/paid.png)

 ### Unpaid Review 
 
![image](https://github.com/NadaAdem/Amazon_Vine_Analysis/blob/main/Resources/unpaid.png)

### Vine reviews (paid)
-  There are 613  Vine reviews.
  - 222 of Vine reviews gave 5-stars.
  - Approximately 36.21% of Vine reviews were 5-stars.
  
### Non-Vine reviews (unpaid) 
-  There are 64968 non-Vine reviews.
  - 30543 non-Vine reviews gave 5-stars.
  -  Approximately 47.01% of non-Vine reviews were 5-stars.



## Summary:
Based on this analysis, we can say that the 5 stars reviews are not the majority in the paid review. 


### Recommendations additional analysis

One additional analysis that could be performed on this dataset to further research the possibility of positivity bias  , By analysis specific products, that we could minimize the results and create a different dataset on just Vine products.
