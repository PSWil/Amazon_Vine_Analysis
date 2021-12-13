# Amazon_Vine_Analysis

## Overview

The purpose of this project is to analyze Amazon reviews written by members of the Amazon Vine program. I used vine review data relating to the video game subcategory of Amazon to conduct my analysis. Using AWS, Google Colaboratory, PostgreSQL, and PySpark I performed the ETL (extract, transform, load) process on the data. Then, I analyzed in depth one of the tables made during the ETL process regarding the vine reviews to determine if there was any positivity bias for reviews in the Vine Program.

## Results

During this analysis I wanted to answer a few key questions.

1. How many Vine reviews and non-Vine reviews were there?
2. How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
3. What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

Here are my answers to these questions.

1. There are 94 vine reviews and 40,471 non-vine reviews for a total of 40,565 reviews.

![total_reviews](https://github.com/PSWil/Amazon_Vine_Analysis/blob/main/images/reviews_count.png)

2. There were 48 5-star vine reviews and 15663 5-star non-vine reviews for a total of 15,711 5-star reviews.

![percentage_5_stars](https://github.com/PSWil/Amazon_Vine_Analysis/blob/main/images/helpful_count.png)

3. 51.06% of paid reviews are 5-stars and 38.7% of unpaid reveiws are 5-stars.

![5_star_reviews](https://github.com/PSWil/Amazon_Vine_Analysis/blob/main/images/paid_unpaid.png)

## Summary

Looking at the results, its clear that there is a positivity bias for reviews in the Vine program. While the non-vine sample size was very large, the vine sample size was less than 100 entries, 94 entires is enought data points to sample with, it could lead a less signifcant result. For further analysis, we could see the percentage of those who purchased the product by filtering through the verified_purchase column to either confirm or fail to confirm if there is a positivity bias for reviews in the Vine program.
