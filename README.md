# Amazon_Vine_Analysis
## Overview
We have been tasked with analyzing Amazon reviews written by members of the paid Amazon Vine program. This program is a service that allows manufacturers and publishers to receive reviews for their products. We are being paid to select a dataset, conduct ETL (extract, transform, load), and determine whether or not there is any bias toward favorable reviews from Vine members.

## Results

The selected dataset was a dataset of US book reviews (https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Books_v1_02.tsv.gz). We employed PySpark for this anaylsis. <br/>

We refer to the "vine_table" - a table with information on Vine Members who reviewed books listed in the above url (seen below). <br/>
![image](https://user-images.githubusercontent.com/72320203/155050326-934554a9-a7be-4981-88a6-d9c5c79b81ec.png)

### How many Vine reviews and non-Vine reviews were there?
#### Vine Reviews
![image](https://user-images.githubusercontent.com/72320203/155051390-b4ea6c40-58d3-413b-991f-dd5c7b4bb5f6.png)
The Numbers: <br/>
-Total Number of Vine Reviews: 0 <br/>
-Total Number of 5-Star Vine Reviews: 0 <br/>
-Percentage of 5-Star Vine Reviews: 0% <br/>

#### Non-Vine Reviews
![image](https://user-images.githubusercontent.com/72320203/155052535-de7749b4-97e6-4082-8d0c-ca4531aa47ca.png)
The Numbers: <br/>
-Total Number of Non-Vine Reviews: 403807 <br/>
-Total Number of 5-Star Non-Vine Reviews: 242889 <br/>
-Percentage of 5-Star Non-Vine Reviews: 60.14977452099642 % <br/>

## Summary
In this particular dataset, there does not seem to be a positivity bias in the Vine Program. However, it is important to note that there were zero Vine Reviews in this dataset. This is abnormal when comparing the numbers with other datasets; cursory looks at these other datasets depict that there are many Amazon Vine members submitting reviews. The lack of Amazon Vine member reviews is most likely an abnormality. 
