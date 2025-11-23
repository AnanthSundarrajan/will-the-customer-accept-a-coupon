# **Will-the-customer-accept-a-coupon**

## *A project for “Berkeley's Professional Certificate in Machine Learning and Artificial Intelligence” by Ananth Sundarrjan* 

### Required Assignment 5.1: Will the Customer Accept the Coupon?

## Context

Imagine driving through town and a coupon is delivered to your cell phone for a restaurant near where you are driving. Would you accept that coupon and take a short detour to the restaurant? Would you accept the coupon but use it on a subsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaurant? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about if it was just you and your partner in the car? Would weather impact the rate of acceptance? What about the time of day?

Obviously, proximity to the business is a factor on whether the coupon is delivered to the driver or not, but what are the factors that determine whether a driver accepts the coupon once it is delivered to them? How would you determine whether a driver is likely to accept a coupon?

## Overview

The goal of this project is to use what you know about visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not.

## Data

This data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he will accept the coupon if he is the driver. Answers that the user will drive there ‘right away’ or ‘later before the coupon expires’ are labeled as ‘Y = 1’ and answers ‘no, I do not want the coupon’ are labeled as ‘Y = 0’. There are five different types of coupons -- less expensive restaurants (under $20), coffee houses, carry out & take away, bar, and more expensive restaurants ($20 - $50).

## Findings from analysing drivers who accepted coupons from a “Bar”
1. The complete dataset comprises 12,684 entries, with 7,210 drivers (56.84%) having accepted a coupon across all categories.
2. Of the total coupons issued, bar coupons accounted for 2,017 offers. The acceptance rate for these coupons was 41% (827 drivers), which is notably elevated.
3. The 41% acceptance rate for the provided bar coupons significantly surpasses the average coupon acceptance rate of approximately 7% reported for the general U.S. population (Source: https://www.opensend.com/post/promotional-redemption-rate-statistics-ecommerce).
4. Drivers who reported visiting a bar three or fewer times demonstrated an acceptance rate 4.4 times higher than those who frequented a bar four or more times per month. This observation is consistent with the hypothesis that individuals with lower visitation frequency are more amenable to discounts.
5. Drivers under the age of 25 exhibit twice the acceptance rate compared to those aged 25 or older. This insight is valuable for bar proprietors seeking to understand their primary consumer demographic and subsequently tailor their services, such as music and food offerings, to this segment.
6. The coupon acceptance rate reached 47.52% for drivers who were not widowed, had no child passengers, and frequently visited bars.
7. Drivers under the age of 30 who visit bars multiple times monthly accepted the coupon at a rate of 30.11%.
8. Drivers with an income below $50,000 who frequent restaurants more than four times a month showed a coupon acceptance rate of 18.86%.
9. A substantial proportion of the population attracted to these coupons is under the age of 30. This demographic suggests opportunities for service refinement, such as updating music and food selections. Given that this younger cohort often has an income below $50,000, price sensitivity is a likely determinant in their decisions, indicating that a more cost-effective menu could potentially broaden the customer base.

## Findings from analysing drivers who accepted coupons from a “Coffee House”
1. Of the total coupons issued, Coffee houses distributed 3,996 coupons, resulting in an acceptance by 1,995 drivers (approximately 50%).
2. Weather Analysis
   - Rainy weather correlates with the highest acceptance rate at 52.21%, suggesting a heightened inclination to accept coffee coupons during inclement weather.
   - Snowy weather showed the lowest acceptance rate (43.23%). It is inferred that severe weather conditions might discourage drivers from making a detour, even for a coffee coupon.
3. Time-of-day analysis
   - 10 AM shows the highest acceptance rate at 64.07%, which strongly suggests a preference for coffee coupons during the mid-morning, likely coinciding with typical breaks or commute patterns.
   - Coupons offered during evening hours, specifically 6 PM (41.26% acceptance) and 10 PM (42.42% acceptance), are associated with significantly lower acceptance rates. This indicates a diminished propensity for coffee consumption late in the day.
4. Next steps for owners:
Target Rainy Days and Mid-Morning: Marketing efforts for coffee house coupons would achieve maximum efficacy when disseminated around 10 AM on days experiencing rain.
Owners may consider reducing operating hours during late evening and snowy conditions to realize cost savings.

## Link to notebook
[Link to notebook](Customer_coupon.ipynb)
[Link to project report](Project Report-Coupons.pdf)
