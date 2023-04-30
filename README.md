# fuzzy-match-using-tfidf-and-cosine-similarity  
APAN 5210 Python For Data Analysis - Group Project  

### Motivation
You work as a Data Analyst for a company that sells a Point of Sales (POS) system to small to medium businesses in the US. Your company has hundreds of thousands of clients and continues to grow. (Maybe you work for Square, maybe Shopify, maybe Stripe, etc…) One of the sales teams got their hands on a dataset of business names and locations and they were trying to identify the companies that are not on the platform, in other words prospective sales targets. You have been tasked with determining the overlap between the list of prospective businesses and the internal client list.

### Problem Statement
You are given two datasets:
- left_dataset.csv
- right_dataset.csv

These datasets contain business names and their addresses.
The goal of this project is to find the businesses that are common to both datasets, that is, the businesses that have a name and address that match between the left and right datasets. Here is an example of a match. It is a nearly perfect match, ignoring case, since the name and address have identical values:
|         | left_dataset                               | right_dataset                              |
|---------|--------------------------------------------|--------------------------------------------|
| id      | 47149                                      | 59483                                      |
| name    | Brothers Jewelry                           | BROTHERS JEWELRY                           |
| address | 837 W Lancaster Ave<br>Bryn Mawr PA, 19010 | 837 W Lancaster ave<br>BRYN MAWR PA, 19010 |
