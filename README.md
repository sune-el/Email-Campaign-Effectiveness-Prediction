# Email-Campaign-Effectiveness-Prediction

![0x0](https://user-images.githubusercontent.com/105907502/185964862-63301526-4570-477d-a24f-78b97df61d0d.jpg)

#Problem Statement
Most of the small to medium business owners are making effective use of Gmail-based Email marketing Strategies for offline targeting of converting their prospective customers into leads so that they stay with them in Business. The main objective is to create a machine learning model to characterize the mail and track the mail that is ignored; read; acknowledged by the reader.

# Data description
# Email_ID - This column contains the email ids of individuals.
Email_type - Email type contains 2 categories 1 and 2. We can assume that the types are like promotional email or sales email.
Subject_Hotness_Score - It is the subject-line effectiveness score.
Email_Source - It represents the source of the email like sales,marketing or product type email.
Email_Campaign_Type - Campaign type
Total_Past_Communications - This column contains the previous mails from the source.
Customer_Location - Categorical data which explains the different demographic location of the customers.
Time_Email_sent_Category - It has 3 categories: 1,2 and 3 which are considered as morning,evening and night time slot.
Word_Count - It contains the no.of words in the mail.
Total_Links - Total links in the email body.
Total_Images - The banner images in the email body.
Email_Status - It is the target variable which contains the characterization of the mail that is ignored; read; acknowledged by the reader.

# Data Pipeline
# Data Processing
Understanding and cleaning the data
# Data Exploration
Analyse the data through visualization
# Model Performing
![1-2](https://user-images.githubusercontent.com/105907502/185966385-177da67e-d677-4dfe-9f01-1323502823c9.png)
Decission Tree
SVM 
Random Forest
XGBoost
#Conclusion
*   In EDA, we observed that Email_Campaign_Type was the most important feature. If your Email_Campaign_Type was 1, there is a 90% likelihood of your Email to be read/acknowledged.
*  It was observed that both Time_Email_Sent and Customer_Location were insignificant in determining the Email_status. The ratio of the Email_Status was same irrespective of the demographic or the time frame the emails were sent on.*   As the word_count increases beyond the 600 mark we see that there is a high possibility of that email being ignored. The ideal mark is 400-600. No one is interested in reading long mails !
*   For modelling, it was observed that for imbalance handling Oversampling i.e. SMOTE worked way better than undersampling as the latter resulted in a lot of loss of information.
*   Based on the metrics, XG Boost Classifier worked the best giving a train score of 89% and test score of 81% for F1 score.
