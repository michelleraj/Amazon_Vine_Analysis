# Amazon Vine Program Analysis: An ETL Pipeline for Bias Detection
This project involves analyzing Amazon Vine reviews to detect potential biases in product ratings. The analysis was conducted using an ETL process with PySpark to extract, transform, and load data into an AWS RDS instance. The goal was to assess the sentiment of Vine and non-Vine reviews, identify any biases, and provide actionable insights for improving review transparency on Amazon.

[Click here to view the Jupyter Notebook - Amazon Review ETL](https://github.com/michelleraj/Amazon_Vine_Analysis/blob/main/Amazon_review_ETL.ipynb)

[Click here to view the Jupyter Notebook- Vine Review Analysis](https://github.com/michelleraj/Amazon_Vine_Analysis/blob/main/Vine_Review_Analysis.ipynb)


## 📌 Overview
This project engineered a **scalable ETL pipeline** to process over **1.8 million Amazon product reviews**. The goal was to assess potential rating bias in **Amazon's Vine program** (where reviewers are compensated) versus organic customer reviews.  

The project automated the data processing and validation workflow, transforming raw data into a clean, analyzable dataset hosted in the cloud. It culminated in a **data-driven report on review sentiment**.

**Key Question:**  
_Do Vine members show a statistically significant bias towards 5-star reviews compared to non-paid reviewers?_

---

## ⚙️ Project Architecture & Workflow
- **Extract**: Raw review data sourced from [Amazon’s public datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt).  
- **Transform & Clean**:  
  - Used **PySpark** for large-scale data processing.  
  - Performed data cleaning, deduplication, and standardization.  
  - Improved data quality, reducing anomalies by **98%**.  
- **Load**: Cleaned data stored in **PostgreSQL** on **AWS RDS** for efficient querying.  
- **Analysis & Reporting**:  
  - Analyzed structured data using **SQL** and **Pandas**.  
  - Generated visualizations to uncover review bias patterns.  

---

## 🛠 Tools & Technologies
- **ETL & Big Data Processing**: PySpark  
- **Cloud Database & Hosting**: AWS RDS  
- **Database Management**: PostgreSQL, pgAdmin  
- **Analysis & Visualization**: SQL, Pandas, Matplotlib, Seaborn  
- **Version Control**: Git, GitHub  

---

## 📊 Key Findings & Business Impact
The analysis provided quantifiable insights into review patterns:

- ✅ **Positive bias detected**: Vine reviews had a **higher percentage of 5-star ratings** compared to organic reviews.  
- 💡 **Actionable insight**: Highlights potential incentives in review systems, important for **transparency and consumer trust**.  

---

## 📈 Visualizations
The findings were summarized with dashboards and charts, including:

- Total Review Volume (Vine vs. Non-Vine)  
- Comparison of 5-Star Review Counts  
- Percentage of 5-Star Reviews by Group (key bias metric)  

---

## 🚀 Business Value
This pipeline provides Amazon (and similar platforms) with a **scalable, automated method** to detect review bias, supporting **fairness, transparency, and data-driven decision-making**.



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


