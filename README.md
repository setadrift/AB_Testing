# AB_Testing
A hypothetical scenario testing which promotion is most effective for a retail store.


A/B Testing Marketing Promotions
Which promotion was the most effective?

SCENARIO

A retailer plans to add a new product to its catalogue. However, they are still undecided between three possible marketing campaigns for promoting the new product. In order to determine which promotion has the greatest effect on sales, the new item is introduced at locations in several randomly selected markets. A different promoition is used at each location and the weekly sales of the new items are recorded for the first four weeks.

The description of the dataset: Our data set consists of 548 entries including:

MarketId: an inhouse tag used to describe market types, which we won't need to use.

AgegOfStores: Age of store in years (1-28). The mean age of a store is 8.5 years.

LocationID: Unique identifier for store location. Each location is identified by a number and the total number of stores is 37.

Promotion: One of 3 promotions that were tested (1,2,3). We don't really know the specifics of each promotion. Nor does it really matter.

Sales In Thousands: Sales amount for a specific LocationID, promotion and week. The mean amount of sales are 53.5 thousand dollars.

Market size: There are 3 types of market size: small, medium, large.

Week: One of four weeks when the promotions were run (1-4)

Null Hypothesis

There is no difference between the different promotions
Alternative Hypothesis

One of the promotions is (B) is better than the other (A)

## EDA and Visualizations

# Comparing Promotion 1 vs Promotion 2 in an A/B Test

## Analysis of P and T-Values

Our **P-Value is close 0** which suggests that there is good evidence to **REJECT the Null Hypothesis** -- meaning that there is a statistical difference between the two groups. 

Our threshold for rejecting the null hypothesis is usually less than 0.05

Our **t-test** shows that the marketing performances for these two groups are significantly different and that promotion group 1 out-performs promotion group 2. 

The one with the larger mean is group 1.

# Comparing Promotion 1 vs Promotion 3 in an A/B Test

## Analysis of P and T-Values

We note that the avg sales from promotion group 1 (58.1) is higher than those from promotion group 3 (55.36).

But after running the t-test between these two gruops, we get a t-value of 1.556 and a p-value of 0.121. 

The computed **p-value is a lot higher than 0.05**, past the threshold for statistical significance. 

We can't conclude anything from these results to reject our null hypothesis. The null hypothesis always states that there is no difference. So we accept the null hypothesis because our p-value is so high. The difference between the means, because they're relatively close, we can say the difference is purely due to random chance - probably because we don't have enough stats
