# Amazon_Vine_Analysis

## Project Overview

Analyzing Amazon reviews written by members of the paid Amazon Vine program - a service that allows manufacturers and publishers to receive reviews for their products. Using the ETL process, SQL & PySpark we will determine if there is any bias toward favorable reviews from Vine members in the dataset.

## Resources

- Data Source: [Automotive Reviews](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Automotive_v1_00.tsv.gz)
- Software/Applications: Amazon Web Services, pgAdmin 4.28,  Google Colab 

## Results

### Performing ETL on Amazon Product Reviews

#### Customers Table
<p align="left">
  <img src="Resources/PGA_customers_table.PNG"/>
</p>

#### Products Table
<p align="left">
  <img src="Resources/PGA_products_table.PNG"/>
</p>

#### Review ID Table
<p align="left">
  <img src="Resources/PGA_review_id_table.PNG"/>
</p>

#### Vine Table
<p align="left">
  <img src="Resources/PGA_vine_table.PNG"/>
</p>

---

### Vine Review Analysis

Based on analyis of Automotive product reviews with 20+ total votes:

- There is total of **27,014** Automotive product reviews.
- **48.37%** of product reviews are 5 star for a total of **13,066** reviews

<p align="left">
  <img src="Resources/review_analysis.PNG"/>
</p>

---

#### Vine (Paid) Reviews

- **0.31%** of product reviews are from the Vine program for a total of **84**reviews.
- **0.25%** of Vine Reviews have a 5-star rating for a total of **33** reviews.

<p align="left">
  <img src="Resources/vine_analysis.PNG"/>
</p>

---

#### Non-Vine (Unpaid) Reviews

- **99.69%** of product reviews are not from the Vine program for a total of **26,930** reviews.
- **99.75%** of non-Vine reviews have a 5-star rating for a total of **13,033** reviews.

<p align="left">
  <img src="Resources/non_vine_analysis.PNG"/>
</p>

## Summary
- Based on the results, the Vine program has only contributed **0.31%** to the total reviews, and only **0.25%** to reviews with a 5-star rating. Therefore, we can conclude that there is no evident positivity for bias in the Vine reviews for Automotive products.

#### Additional analysis to support review validity:
- Analysis of the verified purchases for the products with 5-Star ratings 
- Analysis of the verified purchases in comparison to reviews left by vine members vs non vine members
