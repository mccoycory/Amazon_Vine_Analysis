# Amazon Vine Analysis

## Overview 

The overview of this project was to use our new learned skills of dealing with Amazon Web Services data storage and using Pgadmin to have it stored on a local host. Additionally, we were tasked to work through a ETL process of cleaning and reviewing Amazon product reviews. This analysis will help Amazon with their paid vs unpaid services and the value it is adding to their business. The paid service we studied during this analysis was a product called Vine. This a service where experts are paid to review products and regular folks can pay for their reviews. The dataset chosen in this analysis was for outdoor products. 

## Results 

We used python and pandas to run this analysis. The data was pulled from Amazon online review link, imported into PgAdmin, then a CSV was exported from PgAdmin and imported into python. 

# 1. Vine vs non Vine 

The total dataset contained over 230k reviews! What a great dataset. 

## Main Dataset

![Main Dataset](https://github.com/mccoycory/Amazon_Vine_Analysis/blob/main/Vine_df.png)

From there, we filtered the products with over 20 reviews, which narrowed the dataset down to around 40k. After that, we wanted to see all the reviews that were deemed "helpful" so we kicked out anything that was below 50% helpful.  

## Product count over 20

![20 review](https://github.com/mccoycory/Amazon_Vine_Analysis/blob/main/Votes%20more%20than%2020%20.png)

## Greater than 50% helpful 

![50% helpful](https://github.com/mccoycory/Amazon_Vine_Analysis/blob/main/Helpful%20votes%20over%2050_percent.png)

From the refined dataset, there were only 103 Vine reviews and over 37k non vine reviews. Please reference data set below.

## Vine Reviews Count

![Vine Dataframe](https://github.com/mccoycory/Amazon_Vine_Analysis/blob/main/Paid%20for%20vine%20df.png)

## Non Vine Reviews Count

![Non vine review count](https://github.com/mccoycory/Amazon_Vine_Analysis/blob/main/Did%20not%20pay%20for%20vine.png)

# 2. 5 Star Vine Reviews vs 5 Star Non Vine Reviews 

Performing a quick groupby, we were able to determine the count of reviews by stars. From the data set, there were 55 - 5 star vine reviews and over 19k - 5 star non vine reviews. However, to normalize the dataset due to the different count in datasets, we took a an overall percentage of 5 star reviews vs total reviews. Both datasets are reflect just a little bit over 50% of the vote. This is important data point for Amazon. Depending on when the program started, if it is matching non vine stats, then as the data set grows, they should expect the vine program to grow as well. Please reference the tables below. 

## Vine Program Percent vs Non Vine Percent

![Vine vs non percent](https://github.com/mccoycory/Amazon_Vine_Analysis/blob/main/Percent%20of%205%20star%20reviews%20and%20count.png)

# Summary 

Even though the dataset is small, I believe there is merit to the Vine program. With both programs coming in around 50% of the total votes then this program should continue. One analysis that would be good to look into is if this trend exisits among all product lines within Amazon. If there is a higher % of Vine users in a product line, then I would double down on that product line and dive into why people trust the experts rather than the general public. It would also be neat to determine if the law of averages exisit. Meaning if the expert says the product is not any good does the general public agree with the statement. 






