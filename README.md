# Customer-complaint-analysis
mini project as a part of Edurekha machine learning and data science internship
----------------------------------------------------------------------------------------------------
_Scenario_: 

Product review is the most basic function/factor in resolving customer issues and 
increasing the sales growth of any product. We can understand their mindset toward our service 
without asking each customer.
When consumers are unhappy with some aspect of a business, they reach out to customer 
service and might raise a complaint. Companies try their best to resolve the complaints that they 
receive. However, it might not always be possible to appease every customer.
So Here, we will analyze data, and with the help of different algorithms, we are finding the best 
classification of customer category so that we can predict our test data.

_Objective_:

Use Python libraries such as Pandas for data operations, Seaborn, and Matplotlib for 
data visualization and EDA tasks, Sklearn for model building and performance visualization, and
based on the best model, make a prediction for the test file and save the output.
The main objective is to predict whether our customer is disputed or not with the help of the given 
data.

_Dataset Description:_

Customers faced some issues and tried to report their problems to customer care.
Dispute: This is our target variable based on train data; we have two groups, one with a dispute 
with the bank and another that doesn’t have any issue with the bank.
Date received: The day the complaint was received.
Product: different products offered by the bank (credit cards, debit cards, different types of 
transaction methods, accounts, locker services, and money-related)
Sub-product: loan, insurance, other mortgage options
Issue: Complaint of customers 
Company public response: Company’s response to consumer complaint
Company: Company name
State: State where the customer lives (different state of USA)
ZIP code: Where the customer lives
Submitted via: Register complaints via different platforms (online web, phone, referral, fax, post 
mail) 
Date sent to company: The day the complaint was registered
Timely response?: Yes/no
Consumer disputed?: yes/no (target variable)
Complaint ID: unique to each consumer

_Tasks to be performed:_

The following tasks are to be performed:
- Read the data from the Excel file.
- Check the data type for both data (test file and train file)
- Do missing value analysis and drop columns where more than 25% of data is missing 
- Extracting Day, Month, and Year from the Date Received Column and creating new fields for a 
month, year, and day 
- Calculate the Number of Days the Complaint was with the Company and create a new 
field as “Days held”
- Drop "Date Received"," Date Sent to Company", "ZIP Code", and "Complaint ID" fields
- Imputing Null value in “State” by Mode
- with the help of the days we calculated above, create a new field 'Week_Received' where 
we calculate the week based on the day of receiving.
- store data of disputed people into the “disputed_cons” variable for future tasks 
- Plot bar graph of the total no of disputes of consumers with the help of Seaborn
- Plot bar graph of the total no of disputes products-wise with the help of Seaborn
- Plot bar graph of the total no of disputes with Top Issues by Highest Disputes, with the 
help of seaborn
- Plot a bar graph of the total no of disputes by State with Maximum number of Disputes
- Plot bar graph of the total no of disputes Submitted Via different source
- Plot a bar graph of the total no of disputes where the Company's Response to the 
Complaints
- Plot a bar graph of the total no of disputes where the Company's Response Leads to 
Disputes
- Plot a bar graph of the total no of disputes. Whether there are Disputes Instead of Timely 
Response
- Plot bar graph of the total no of disputes over Year Wise Complaints
- Plot bar graph of the total no of disputes over Year Wise Disputes
- Plot bar graph of Top Companies with Highest Complaints
- Convert all negative days held to zero (it is the time taken by the authority that can't be 
negative)


