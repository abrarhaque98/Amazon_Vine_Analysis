# Amazon_Vine_Analysis

## Overview of Analysis 
The objective of this project was to analyze Amazon reviews written by members of the paid Amazon Vine program. The analysis was performed with Pyspark on the Health Personal Care dataset which was pulled from s3 on AWS and later pushed onto an AWS database. The dataset also included non vine members to test for bias in reviews.

## Results
The data frame was filtered out to only factor for reviews that had atleast 20 total votes then filtered even further for votes that had over a 50% helpful to total vote ratio. The final dataframe looked like this below.

![image](https://user-images.githubusercontent.com/85713568/142544733-df0fdf8f-4c5f-40ad-9cd6-2f325cc6e00f.png)


![image](https://user-images.githubusercontent.com/85713568/142545785-497db369-39a1-4f84-b804-2e2cabf37b6c.png)

The resulting vote count for helpful reviews came out to 121,360. 

![image](https://user-images.githubusercontent.com/85713568/142548844-adff66e1-ae8d-4eed-963c-13945eb36cbd.png)


The count of five star reviews, count of paid five star reviews and nonpaid reviews were counted from the helpful vote filtered vine data frame. Their results are shown above.

![image](https://user-images.githubusercontent.com/85713568/142549208-81597536-991d-455d-9454-12c740043866.png)

The percentage calculated are above.


## Summary 

In summary from the analysis it does not seem like there is much analysis bias for reviews in the Vine program. Although these reviews were paid for only 220 of the 74,690 five star reviews came from Paid reviewers, whereas 74,440 came from non paid reviewers. On a percentage scale it was .295% and 99.705% respectively. 

Another analysis I would perform would be counting the vine and non vine reviews for each star rating along with the average star rating amongst the vine and non vine groups. 




