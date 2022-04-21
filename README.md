# Amazon Vine Analysis
## Purpose of the Analysis
The purpose of this analysis is to evaluate Amazon reviews for products in the pet products category. Specifically, vine and non-vine reviews are compared for bias.
## Resources
- Data Source: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Pet_Products_v1_00.tsv.gz

## Analysis
Results were first filtered by total votes. Reviews with at least 20 votes were kept for further analysis.


![image](https://github.com/MDHetrick/amazon_vine_analysis/blob/main/Resources/DF1.png)

Then, results were filtered by helpful votes. Results with at least 50% of the votes voted to be helpful were kept for further analysis.

![image](https://github.com/MDHetrick/amazon_vine_analysis/blob/main/Resources/DF2.png)

Finally, the results were split into two dataframes, one containing non-vine reviews, and the other containing vine reviews.

![image](https://github.com/MDHetrick/amazon_vine_analysis/blob/main/Resources/DF3.png)



## Results
- How many Vine reviews and non-Vine reviews were there?
  - Vine Reviews: 170
  - Non-Vine Reviews: 37,840 

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
  - 5-star Vine Reviews: 65
  - 5-star Non-Vine Reviews: 20,612 


- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
  - % 5-star Vine Reviews: 38%
  - % 5-star Non-Vine Reviews: 54%

## Summary
#### Is there positivity bias for reviews in the Vine program?
 There does not seem to be any positivity bias within the vine program. There was a smaller percentage of 5 star vine reviews than non-vine reviews (38% vine, 54% non-vine), indicating that vine reviews are not biased toward the positive. However, vine reviews accounted for just 170 (or about 4%) of the 38,010 total reviews considered, so it may not be accurate to do a direct percentage comparison.
#### Additional Analyses
To support this analysis, I would suggest combining reviews from many products, and comparing vine and non-vine reviews. This could provide a larger dataset of vine reviews. With this dataset, it would also be advantageous to look at reviews by each star level to compare distributions. 

