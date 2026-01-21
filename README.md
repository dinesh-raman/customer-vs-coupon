# Will the customer accept the coupon 
##### Project Juptier Notebook: https://github.com/dinesh-raman/customer-vs-coupon/blob/main/prompt.ipynb
##### Project Data Source: 

## What is the Problem
The goal of this project is to s to distinguish between customers who accepted a driving coupon versus those who did not. The project uses data  visualizations and probability distributions to uncover the findings.

## What is the Data
This project uses data from the UCI Machine Learning Repository which was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios, including the destination, current time, weather, and passenger, and then asks people whether they will accept the coupon if they are the driver. 
There are three possible answers people can choose from:
##### 1. “Right away”
##### 2. “Later, before the coupon expires”
##### 3. “No, I do not want the coupon”
The first two responses are labeled as “Y = 1,” and the third is labeled as “Y = 0.”

There are five different types of coupons:
###### 1. Less expensive restaurants (under $20)
###### 2. Coffee houses
###### 3. Carryout and takeaway
###### 4. Bars
###### 5. More expensive restaurants ($20–$50)

### Data Attributes:

The attributes of this data set include:
##### 1. User attributes
    -  Gender: male, female
    -  Age: below 21, 21 to 25, 26 to 30, etc.
    -  Marital Status: single, married partner, unmarried partner, or widowed
    -  Number of children: 0, 1, or more than 1
    -  Education: high school, bachelors degree, associates degree, or graduate degree
    -  Occupation: architecture & engineering, business & financial, etc.
    -  Annual income: less than \\$12500, \\$12500 - \\$24999, \\$25000 - \\$37499, etc.
    -  Number of times that he/she goes to a bar: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
    -  Number of times that he/she buys takeaway food: 0, less than 1, 1 to 3, 4 to 8 or greater
    than 8
    -  Number of times that he/she goes to a coffee house: 0, less than 1, 1 to 3, 4 to 8 or
    greater than 8
    -  Number of times that he/she eats at a restaurant with average expense less than \\$20 per
    person: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
    -  Number of times that he/she goes to a bar: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
    
##### 2. Contextual attributes
    - Driving destination: home, work, or no urgent destination
    - Location of user, coupon and destination: we provide a map to show the geographical
    location of the user, destination, and the venue, and we mark the distance between each
    two places with time of driving. The user can see whether the venue is in the same
    direction as the destination.
    - Weather: sunny, rainy, or snowy
    - Temperature: 30F, 55F, or 80F
    - Time: 10AM, 2PM, or 6PM
    - Passenger: alone, partner, kid(s), or friend(s)

##### 3. Coupon attributes
    - time before it expires: 2 hours or one day


## What are the Findings
Here are the key findings of this project.
#### Overall Acceptance Rate of the coupon is : 56.84
#### Acceptance by Coupon Catagory :
Coupon Category | Acceptance % 
--- | --- | 
Carry out & Take away|73.5%
Restaturant(<$20>|70.7%
Coffee House| 49.9%
Restaurant($20-$50)|44.1%
Bar|	41.0%

#### Bar Coupon Analysis

Here are the observations for Bar Coupons:-

-Regular bar-goers, especially those who visit bars more than once a month, are significantly more likely to accept bar coupons.
the trend is further amplified when combined with factors like being over the age of 25, having adult passengers, and having occupations outside of farming, fishing, or forestry.

-The conditions also suggests that a combination of frequent bar visits, fewer family responsibilities, and specific income/restaurant habits correlates with higher acceptance.
Therefore, a hypothesis could be:-

-Drivers who exhibit a lifestyle indicative of regular social drinking, characterized by frequent bar visits, older age (e.g., over 25), and fewer immediate family obligations (e.g., no kids as passengers, not widowed), are considerably more likely to accepting bar coupons.


#### Independent Investigation - Coffee House Coupon Analysis

##### Overall Acceptance Rate of the Coffee House coupon is : 49.92%
-Cofee House Coupon has the hightest acceptance rate amount the *age group* : Below 21 at 69.6%
-Coffee House Coupon has highest acceptance rate in the *income group* : 87,500-99,999
-Drivers tend to accept more Coffee House Coupons  when the *Weather* is : Rainy
-Coffee House Coupon has good acceptance rate in the morning 10AM



## Next Steps
1. Perform futher fine grained EDA - Convert non numeric features to numeric features 
2. Methodically balence the dataset and select the right classification model
3. Conduct Feature Engineering
4. Come up with a feature rich ML model 
 

