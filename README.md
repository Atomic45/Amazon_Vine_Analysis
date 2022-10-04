# Amazon_Vine_Analysis

The Amazon Vine Program is a service that allows manufacturers and publishers to receive reviews for their products. This analysis is to determine if there is any bias toward favorable reviews from Vine members compared to non-Vine members. The dataset selected for this analysis is the Apparel dataset. This analysis was reviewed, filtered and transformed using PySpark, AWS RDS, and PostgreSQL. 

## Results
The Apparel dataset had more than three million reviews. This required filtering the dataset to provide an amount to be able to conduct the analysis. Using Google Colab as the tool to conduct the filtering produced the following results: 

- Percent of Votes equal or greater than 50%

![percent_votes_df](https://user-images.githubusercontent.com/30300621/193722279-3cc9a383-38ea-4758-9f34-36617766d289.PNG)

The dataset was reduced from over three million reviews to 45,279, which is a useful sample set to answer the analysis questions: 

1. How many Vine reviews and non-Vine revews were there?  As shown below, there were 33 total Vine reviews and 45,246 non-Vine reviews

![vine_reviews](https://user-images.githubusercontent.com/30300621/193722552-ae622c1c-a973-42a5-9d9a-b8a4a8367404.PNG)


![paid_votes](https://user-images.githubusercontent.com/30300621/193722840-81167120-7d90-4408-bbd4-6a6f0019714b.PNG)


![non_paid_votes](https://user-images.githubusercontent.com/30300621/193722853-426aeee9-a626-4a55-a840-dd8464a0fd4a.PNG)



2. How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars? 

There are not that many Vine reviews with 5 stars. 15 out of 33 of the Vine reviews have 5 stars. 

The non-Vine reviews have 23,639 5-star ratings out of 45,246 reviews. 

3. What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars? 

This means 45% of Vine reviews were 5 stars and 52.25% of non-Vine reviews were 5 stars. 

![vine_reviews](https://user-images.githubusercontent.com/30300621/193723336-9627bcbd-6cf0-4da5-b3dd-adb0563ac5dc.PNG)

## Summary
In summary, it is safe to say there is no bias between being a paid Vine member to conduct reviews on products, compared to non-Vine review members. The percentage difference is not substantial. 45% for Vine member reviews, and 52.25% for non-Vine reviews is less than a 10% difference. This is only for the Apparel category. Conducting further analysis on all products with a reasonable sample data sets from other categories can help make a definite determination and comparison. 

