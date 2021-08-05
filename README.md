# Amazon_Vine_Analysis

## Project Overview
This project analyzes reviews of the Amazon Vine program, which is a paid service that allows manufacturers and publishers to receive reviews for their products.  The analysis will evaluate bias in Vine Program reviews and inform whether the client should invest in a gift for reviewers.

PySpark was used to perform ETL on available Tool product category reviews in an AWS RDS instance. Once the data was transformed it was loaded into pgAdmin and PySpark was used to perform the bias analysis.

## Results
In the vine review comparison summary table below we find the following insights...

- vine reviews are a relatively small portion of all reviews in the product category or approximately 1 out of every 100 reviews
- there are ~160 5-star vine reviews and 14.6K non-vine program 5-star reviews
- 5-star reviews make up a larger percent of vine program reviews (57%) when compared to non-vine program reviews (46%)

![image_name](https://github.com/Christopheremorgan/Amazon_Vine_Analysis/blob/main/vine_review_summary.png)


## Summary
Although vine program reviews are a relatively small percent of all reviews, the share of 5-star reviews for the vine program is slightly more than 10ppt higher than non-vine program reviews.   This indicates there may be some favorable bias associated with vine program reviews.

It is recommended to dive a little deeper and assess only products that have both vine program and non-vine program reviews to further test bias and ensure there are no product portfolio impacts associated with the higher vine program ratings.

## Data Files
[Amazon_Reviews_ETL.ipynb](https://github.com/Christopheremorgan/Amazon_Vine_Analysis/blob/main/Amazon_Reviews_ETL.ipynb)

[Vine_Review_Analysis.ipynb](https://github.com/Christopheremorgan/Amazon_Vine_Analysis/blob/main/Vine_Review_Analysis.ipynb)