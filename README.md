# Amazon_Vine_Analysis
## Overview of the analysis: 
Analyzing Amazon reviews for the Camera Dataset written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Utilised PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Determined if there is any bias toward favorable reviews from Vine members in your dataset.

## Results

Number of Vine reviews and non-Vine reviews

<img width="546" alt="Screen Shot 2021-10-30 at 3 00 55 PM" src="https://user-images.githubusercontent.com/57809798/139555470-b5c4db1a-a83a-442c-ac5f-2b04318cbed1.png">

Number of  Vine/non-Vine reviews with 5 stars

<img width="844" alt="Screen Shot 2021-10-30 at 3 01 33 PM" src="https://user-images.githubusercontent.com/57809798/139555484-3837a68c-8588-4356-a969-cccaeb1c07c3.png">


Percentage of Vine/non-Vine reviews with 5 stars
<img width="1239" alt="Screen Shot 2021-10-30 at 3 04 52 PM" src="https://user-images.githubusercontent.com/57809798/139555553-4bce391c-c541-432d-997b-ced03d8f47a5.png">

The above percentage shows that there is a postive bias for reviews in vine program


