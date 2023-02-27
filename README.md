# Amazon_Vine_Analysis
## Overview
This analysis was done to determine the effectiveness of the Amazon Vine program, which is a service that Amazon provides that allows sellers and providers to get more reviews through Amazon. In this analysis we looked at a dataset of reviews of books on amazon, specifically the most recent/updated dataset of books from this list of 50 datasets: [Amazon Datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt). As will be seen, this dataset was not a good choice for this analysis, and in the future, a different dataset should be chosen. With these reviews, however, we can attempt to see how the reviews that are made through the Vine program differ from those that are not.

## Results
As mentioned above, this was a poor dataset to chose, because no book reviews were made through the Vine program. The data was first filtered to get rid of reviews that did not have a high number of votes and get rid of reviews that were deemed unhelpful (more than 50% of votes were "Unhelpful" instead of "Helpful"). After this, two dataframes were made, one with reviews made through the Vine system and one with reviews that had not paid for the Vine program. The first, however, yielded 0 reviews, as can be seen below:
<p align="center">
<img src="https://github.com/bchillman/Amazon_Vine_Analysis/blob/main/Images/paid_dataframe.png" width="809" height="102">
</p>
Since there were 0 of these reviews, no analysis can be made of the Vine Program. The second dataframe is shown below with its results:
<p align="center">
<img src="https://github.com/bchillman/Amazon_Vine_Analysis/blob/main/Images/unpaid_dataframe.png" width="426" height="197">
</p>
This dataframe can be analyzed and it is found that, after filtering, there were 375,353 total un-paid reviews, 226,910 of which were 5-star reviews. This gives us a percentage of 60.5% of reviews that were not through the Vine Program that were five stars.

## Summary
Since we found 0 reviews, which were made through the vine program in this dataset, we are unable to make any conclusions about the program and its effect on reviews. Certainly more anlysis would need to be done, specifically through a dataset more properly vetted to make sure that there are Vine reviews made in it. After this is done, we could look at not just five-star reviews, and create a barchart that allows us to see the percentage of reviews both in and out of the program at each star-level. This will allow us to make further conclusions about any bias that may be affecting the Vine Program reviews.
