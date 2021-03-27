# Amazon Vine Analysis

Amazon has a service, called 'Vine' where it pays people to review products. While the number of reviews coming from this program vs. reviews overall is quite small (1.4% for our study), it is still significant. Of course, this begs the question of whether or not Vine members are reviewing products differently than non-Vine members. For this particular study we'll analyze the data to see if the Vine members are reviewing Software products more favorably than the general population. 

[Extract, Transform, and Load File Here](https://github.com/carlosjennings1991/Amazon_Vine_Analysis/blob/main/Amazon_Reviews_ETL.ipynb)
<br>
[Data Analysis File Here](https://github.com/carlosjennings1991/Amazon_Vine_Analysis/blob/main/Vine_Review_Analysis.ipynb)
<br>
[Source Data File Here](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Software_v1_00.tsv.gz)

## Tools Used
- [x] Python (Pandas, PySpark)
- [x] SQL (Postgres)
- [x] AWS (RDS)

___

## Results

After extracting, transforming and loading our data we have a base data frame. We then split it into two groups - reviews belonging to vine members, and the rest. Here are some key takeaways. 


### Number of Vine Reviews:

There are 231 vine reviews, we can see a screenshot from jupyter notebook confirming such below. 

<img src="https://github.com/carlosjennings1991/Amazon_Vine_Analysis/blob/main/vine_members.png" height="76" width="266">


### Number of Non-Vine Reviews:

There were 16,464 non-vine reviews, we can see a screenshot from jupyter notebook confirming such below. 

<img src="https://github.com/carlosjennings1991/Amazon_Vine_Analysis/blob/main/non-vine_members.png" height="75" width="290">


### Number of 5 Star Reviews from Vine Members:

There were 93 five star reviews from Vine Members. Screenshot below

<img src="https://github.com/carlosjennings1991/Amazon_Vine_Analysis/blob/main/vine_members_five_stars.png" height="75" width="493">


### Number of 5 Star Reviews from everyone else:

There were 4,867 five star reviews from people who were not Vine members. Screenshot below

<img src="https://github.com/carlosjennings1991/Amazon_Vine_Analysis/blob/main/non_vine_members_five_stars.png" height="75" width="522">


### Percentage of Vine Reviews that were 5 Stars

More than two thirds of the reviews from Vine members were 5 stars (67.4%). Screenshot below

<img src="https://github.com/carlosjennings1991/Amazon_Vine_Analysis/blob/main/vine_percentage_five_stars.png" height="120" width="684">


### Percentage of Non-Vine Reviews that were 5 Stars

4,867 5 star reviews came from Non-Vine reviewers, totalling about 42% of the total non-vine reviews. Screenshot below

<img src="https://github.com/carlosjennings1991/Amazon_Vine_Analysis/blob/main/non_vine_percentage_five_stars.png" height="120" width="724">

___

## Summary
