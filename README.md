# Amazon-Recommender-System and Data analysis using Map reduce
#### Deployed single node cluster to perform analysis using map reduce
### /**

### author Sayali Walke

### **/

# Dataset used for analysis:
The Amazon Customer Reviews Dataset is a large dataset with size > 20GB. 
However, for this analysis, I’ve used a subset of this dataset named
“amazon_reviews_us_Beauty_v1_00.tsv” 

### Here’s the detailed description of dataset and its contents. 
marketplace: 2 letter country code of the marketplace where the review was written. 

customer_id: Random identifier that can be used to aggregate reviews written by a single author. 

review_id: The unique ID of the review. 

product_id: The unique Product ID the review pertains to. In the multilingual dataset the reviews for the same product in different countries can be grouped by the same product_id.

product_parent: Random identifier that can be used to aggregate reviews for the same product. 

product_title: Title of the product. 

product_category: Broad product category that can be used to group reviews 
(also used to group the dataset into coherent parts). 

star_rating: The 1-5 star rating of the review. 

helpful_votes: Number of helpful votes. 

total_votes: Number of total votes the review received. 

Vine: Review was written as part of the Vine program. 

verified_purchase: The review is on a verified purchase. 

review_headline: The title of the review. 

review_body: The review text. 

review_date: The date the review was written.

# Apache MAHOUT
#### Created a recommender system using Mahout. It serves the functionality of recommending similar products based on the similar items bought by other customers.(People who bought this….also bought this…..)

# Hadoop
#### I have created a single node Hadoop cluster on virtual machine and carried out following data analysis 
#### using various Map-reduce Algorithms:
#### 1.	 Top 100 Products based on average of reviews: (Filtering Pattern )
#### 2.	 Average chaining and Sorting Of reviews: (Chaining and Sorting )
#### 3.	 No of reviews per product: (Numerical Summarization)
#### 4.	 Inner join on Average of reviews and no of reviews for each product(Inner Join)
#### 5.	 Customer list for each product: (Inverted Index)
#### 6.	 Created 5 bins for 1,2,3,4,5 ratings: Binning (Organization Pattern)
#### 7.	 Partitioned the data into different files for each day in 2015-08:  Partitioning (Organization Pattern)
#### 8.	 Distinct Reviews Counter:  (Numerical Summarization Pattern)
#### 9.	Percentage of Helpful votes: (Numerical Summarization Pattern)

# Apache HIVE
#### 1. Top 10 Products based on Average ratings
#### 2.	Most Valuable Customer based on number of products bought
#### 3.	Most popular product based on number times product bought
#### 4.	Number of products bought per day
#### 5.	Number of products per ratings

# Apache Pig
#### 1.	 Number of reviews given per day
#### 2.	 Number reviews given per product



