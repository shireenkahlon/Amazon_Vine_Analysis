# Amazon_Vine_Analysis
This project will use PySpark and PostGres to perform the ETL process on data within a database in AWS

## Overview of the analysis
The purpose of this project is to analyze reviews written by vine members. Vine is a program consisting of Amazon’s invited and compensated reviewers; Vine members are provided products that they will write a review for in exchange for compensation. The analysis conducted will determine if there is any bias towards writing positive reviews from Vine members. 

## Results
* The total number of reviews from Vine members and non-Vine members were 170 and 37,840 reviews, respectively. 
![count_paid_unpaid](https://github.com/shireenkahlon/Amazon_Vine_Analysis/blob/main/Screenshots/paid_unpaid_count.png)

* There were 65 and 20,612 number of 5-star reviews from Vine members and non-Vine members, respectively.
![five_star_reviews_paid_unpaid](https://github.com/shireenkahlon/Amazon_Vine_Analysis/blob/main/Screenshots/paid_unpaid_five_star.png)

* 38.24% of reviews from Vine members were 5 stars; whereas 5 star reviews comprised 54.47% of total reviews from non-Vine members.
![paid_unpaid_percentage](https://github.com/shireenkahlon/Amazon_Vine_Analysis/blob/main/Screenshots/paid_unpaid_percent.png)

## Summary
From the statistics at our disposal, it appears there is no positivity bias from Vine members. Only 38% of reviews from Vine members were 5 stars — a little over 1/3 of the total reviews from Vine members. To compare, almost 20% more reviews (54.47%) from non-paid members were 5-star reviews. This tells us that it is not likely that Vine members used positivity bias when writing reviews. However, we cannot tell from this data alone. In order to get a bigger picture of if positivity bias played a part in the reviews, we could obtain 4-star ratings, — in addition to the 5-star ratings — from both, Vine and non-Vine members’ reviews. From this, we can get a more accurate picture of positivity bias considering many people may be hesitant to give a product a 5 star while still wishing to give a positive review. 
