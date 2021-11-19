# Amazon_Vine_Analysis

## Overview of Analysis 
The objective of this project was to analyze Amazon reviews written by members of the paid Amazon Vine program. The analysis was performed with Pyspark on the Health Personal Care dataset which was pulled from s3 on AWS and later pushed onto an AWS database. The dataset also included non vine members to test for bias in reviews.

## Results
The data frame was filtered out to only factor for reviews that had atleast 20 total votes then filtered even further for votes that had over a 50% helpful to total vote ratio. The final dataframe looked like this below.

![image](https://user-images.githubusercontent.com/85713568/142544733-df0fdf8f-4c5f-40ad-9cd6-2f325cc6e00f.png)


The resulting vote count for helpful reviews came out to 121,360. 

![image](https://user-images.githubusercontent.com/85713568/142545785-497db369-39a1-4f84-b804-2e2cabf37b6c.png)

The count of five 

