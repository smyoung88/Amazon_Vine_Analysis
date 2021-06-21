# Amazon_Vine_Analysis

## Overview of the analysis
The purpose of this project was to analyze Amazon reviews written by members of the paid Amazon Vine program which is a service that allows manufacturers and publishers to receive reviews for their products. In this analysis, a home improvement dataset was selected where an ETL process was used to extract the dataset, transform the data, connect to an AWS RDS instance, and load the stransformed data into pgAdmin. Pandas was then utilized to determine if there was any any bias toward favorable reviews from Vine members in the selected dataset. The results are below.

## Results

<b>How many Vine reviews and non-Vine reviews were there?</b>
The total Vine (paid for) and non-Vine (unpaid for) reviews were 266 and 38,829 respectively as shown below in the pandas analysis screenshots:


<img src="https://github.com/smyoung88/Amazon_Vine_Analysis/blob/main/Resources/vine_reviews.png">
<img src="https://github.com/smyoung88/Amazon_Vine_Analysis/blob/main/Resources/non_vine_reviews.png">


<b>How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?</b>
The total 5-star Vine (paid for) and non-Vine (unpaid for) reviews were 125 and 18,246 respectively as shown below in the pandas analysis screenshots:


<img src="https://github.com/smyoung88/Amazon_Vine_Analysis/blob/main/Resources/fivestar_vine_reviews.png">
<img src="https://github.com/smyoung88/Amazon_Vine_Analysis/blob/main/Resources/fivestar_non_vine_reviews.png">

<b>What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?</b>
The total percent of 5-star Vine (paid for) and non-Vine (unpaid for) reviews were both 46.99% as shown below in the pandas analysis screenshots:

<img src="https://github.com/smyoung88/Amazon_Vine_Analysis/blob/main/Resources/fivestar_vine_pct.png">
<img src="https://github.com/smyoung88/Amazon_Vine_Analysis/blob/main/Resources/fivestar_non_vine_pct.png">


## Summary
In summary, there does not appear to be any positivity bias for reviews in the Vine program since both Vine and non-Vine reviews had the same percentage of 5-star votes. To further validate this, analysis should be done on each 'star-rating'. We validated that the high end of the star-rating did not appear to show any signs of bias, but it may also be useful to see where the percentage differences are between each tier for the non-Vine and Vine program.
