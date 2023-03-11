# Data Analysis on call centre data.

Here we'll be performing data analysis on call center data. The data is sourced from data.world and I've also added the raw file in the files.
Our dataset contains 32941 entries and 12 columns. 
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
The description of dataset is mentioned below:
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
1. id - Unique id of each contact.
2. Customer Name
3. Sentiment - Customer sentiment throughout the call ( Neutral, positive ,negative, very negative or very positive).
4. csat score - Customer satisfaction score from 1 - 10
5. call timestamp - Date of contact
6. Reason -  Contact reason (Billing, Service outage or Payments)
7. City
8. State
9. Channel - Point of contact (Call center, chatbot, email or web)
10. Response time - Respone time to customer query from our end from time of contact (Above SLA, below SLA or within SLA) (SLA - service level agreement)
11. Call Duration in minutes
12. Call Center - Call center location
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
OBJECTIVES : 
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
We need to set a research goal which we have to achieve from the dataset given to us. We can get different analysis from same dataset and some of the objectives which I've extracted are mentioned below:

1. Lines chart for call trends - It will tell us how much contacts we receive on a daily bais. ( Columns used are - call timestamp and count_id)
2. A bar graph for the call channel which will help us to know which channels are most frequently used by customers. ( columns - channel and count_id)
3. A map for states showing the number of contacts depending upon the region. ( columns - state and count_id).
4. Column chart for reason of contact -  to know which are the most common reasons for contact. ( columns - reason and count_id)
5. Bar chart for the response time- it will inform us whether we're able to resolve the customer queries within the SLA time. ( columns - response time and count_id)
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
DATA CLEANING : 
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
Now, we've got a basic understanding of our dataset. Next we'll review our dataset and do the cleaning and transformation part. Some of the issues encountered by me are mentioned below:

-- In csat score column a number of entries are NULL, but it isn't mandatory to change it since we've sentiment column which we can use if we need to perform sentiment analysis. 

-- Next, in call timestamp dates are stored in two formats (mm - dd - yyyy) and (mm / dd / yyyy) format. Due to this excel don't directly convert all the entries in date format which is required. To resolve this, we need to select the column and then follow these steps ( data > text to columns > Date : MDY > Finish).

-- In next steps we'll convert the required columns in number format e.g. csat_score and call duration in minutes.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
DATA ANALYSIS : 
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
Since our data is cleaned now and we've a clear set of objectives that we need to find from this data. We'll move further and use the Pivot table function of excel to create the required line chart, map or bar chart. We can also add filters to the dashboard using slicers.

Once we've created the required charts we'll create a simple dashboard to show these insights in a presentable format to our client or Senior representative. 
