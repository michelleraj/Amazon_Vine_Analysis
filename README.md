# Amazon_Vine_Analysis
This project involves analyzing Amazon Vine reviews to detect potential biases in product ratings. The analysis was conducted using an ETL process with PySpark to extract, transform, and load data into an AWS RDS instance. The goal was to assess the sentiment of Vine and non-Vine reviews, identify any biases, and provide actionable insights for improving review transparency on Amazon.

[Click here to view the Jupyter Notebook - Amazon Review ETL](https://github.com/michelleraj/Amazon_Vine_Analysis/blob/main/Amazon_review_ETL.ipynb)

[Click here to view the Jupyter Notebook- Vine Review Analysis](https://github.com/michelleraj/Amazon_Vine_Analysis/blob/main/Vine_Review_Analysis.ipynb)


## Project Objectives
Data Extraction and Loading: Extract and load over 1.8 million product reviews from Amazon's Vine program and non-Vine sources using PySpark.

Data Transformation: Clean and standardize the data to ensure consistency, reducing anomalies by 98%.

Sentiment Analysis: Conduct sentiment analysis to compare the distribution of 5-star reviews between Vine members and non-Vine members.

Reporting: Summarize findings in a comprehensive report with visualizations to provide actionable insights.

## Tools and Technologies
PySpark: Used for the ETL process and data manipulation.

AWS RDS: Hosted the PostgreSQL database for storing transformed data.

pgAdmin: Managed and queried the database for analysis.

Pandas: Utilized for data analysis and handling.

SQL: Used for complex querying and data management.

Matplotlib/Seaborn: Created visualizations to represent data trends and biases.

## Dataset
The dataset consists of reviews from Amazon's Vine program and non-Vine reviews across various product categories. The dataset includes:

Vine Reviews: 1,494,401 reviews (82.94% of total)
Non-Vine Reviews: 307,571 reviews (17.06% of total)

<img width="1975" alt="Screenshot 2024-08-09 at 4 50 34 PM" src="https://github.com/user-attachments/assets/89c7e255-9c2d-4a11-8bf3-5691df1c4084">

<img width="1090" alt="Screenshot 2024-08-09 at 4 50 49 PM" src="https://github.com/user-attachments/assets/602a96b1-9dab-4169-a07b-c538890eaf2f">

## Results

Number of Vine reviews and non-Vine reviews

<img width="546" alt="Screen Shot 2021-10-30 at 3 00 55 PM" src="https://user-images.githubusercontent.com/57809798/139555470-b5c4db1a-a83a-442c-ac5f-2b04318cbed1.png">

Number of  Vine/non-Vine reviews with 5 stars

<img width="844" alt="Screen Shot 2021-10-30 at 3 01 33 PM" src="https://user-images.githubusercontent.com/57809798/139555484-3837a68c-8588-4356-a969-cccaeb1c07c3.png">


Percentage of Vine/non-Vine reviews with 5 stars
<img width="1239" alt="Screen Shot 2021-10-30 at 3 04 52 PM" src="https://user-images.githubusercontent.com/57809798/139555553-4bce391c-c541-432d-997b-ced03d8f47a5.png">

The above percentage shows that there is a postive bias for reviews in vine program


