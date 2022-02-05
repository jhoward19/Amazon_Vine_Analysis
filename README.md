# Amazon_Vine_Analysis
# Overview of Analysis 

The task in this project was to analyze amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. In order to complete the analysis, I selected a dataset on baby products. After the selection I used PySpark to perform the ETL process, connected tow AWS RD instance, and load the data into pgAdmin. Finally, once that process was completed, I used PySpark again to determine if there were any bias towards favorable reviews from Vine members in the data.


# Results 
In order to perform certain calculations, I first cleaned the data to remove the null values, then I filtered it by reviews that received 20 or more votes and that were 50 percent helpful.

<img width="777" alt="Screen Shot 2022-02-04 at 10 56 47 PM" src="https://user-images.githubusercontent.com/91230916/152627856-466a420b-d73e-4d40-832a-dec2d3d8f3f0.png">


* After I filtered the data by the parameters mentioned above, I used that filtered data to perform the remaining calculations for the analysis. In the vine analysis you will find that there was a total of 463 vine reviews and a total of 25,079 of non-vine reviews out of 25,542 total reviews. 

     <img width="733" alt="Screen Shot 2022-02-04 at 10 57 44 PM" src="https://user-images.githubusercontent.com/91230916/152627880-10e4c0c9-0277-49e4-b815-5b232fa1e8f0.png">


* Furthermore, there were 202 five star paid Vine reviews and 12,028 five-star unpaid Vine reviews out of 12, 230 five-star rating reviews. 

     <img width="733" alt="Screen Shot 2022-02-04 at 10 59 20 PM" src="https://user-images.githubusercontent.com/91230916/152627913-8fdf6820-bd94-42b1-b2fd-950db76eb670.png">


* Finally, out of 463 total paid vine reviews only 202(1.65%) were 5-star rating and out of 25,079 total unpaid vine reviews 12,028 (98.35%) were 5-star rating. 

     <img width="864" alt="Screen Shot 2022-02-04 at 10 59 53 PM" src="https://user-images.githubusercontent.com/91230916/152627919-b4c1935f-04d1-4bbf-a56f-3feb49ee4bae.png">


# Summary
In summary, this analysis does not support or provide any evidence that there is any bias towards favorable reviews from Vine members. From this analysis you can assume that the vine members reviews were not helpful and that the non-vine members reviews were useful in helping customers buy the product. To further the study, it could be helpful analyze the verified purchase with the vine column to determine if the review had an impact whether the product was purchased. 

