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
         
  **Data Cleaning & Pre-processing**
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



  **Data Analysis and Visualization**
  some ofthe results are uploaded for detailed solution checkout the collab file
- Plot bar graph of the total no of disputes of consumers 
- Plot bar graph of the total no of disputes products-wise 
- Plot bar graph of the total no of disputes with Top Issues by Highest Disputes
![image](https://github.com/user-attachments/assets/83beb91b-6f91-42f5-8dd0-1183d5e7e087)

- Plot a bar graph of the total no of disputes by State with Maximum number of Disputes
- Plot bar graph of the total no of disputes Submitted Via different source
- Plot a bar graph of the total no of disputes where the Company's Response to the 
Complaints
- Plot a bar graph of the total no of disputes where the Company's Response Leads to 
Disputes
- Plot a bar graph of the total no of disputes. Whether there are Disputes Instead of Timely 
Response
![image](https://github.com/user-attachments/assets/83d0d487-282f-43c1-81b8-1853385075fc)

- Plot bar graph of the total no of disputes over Year Wise Complaints
- ![image](https://github.com/user-attachments/assets/d2a66730-24b5-4f8d-bcc2-0c27ea8b6ce9)

- Plot bar graph of the total no of disputes over each month
- Plot bar graph of Top Companies with Highest Complaints
  ![image](https://github.com/user-attachments/assets/1505fb2f-b18d-47c6-a8d6-180b2acd1e05)

- Convert all negative days held to zero (it is the time taken by the authority that can't be 
negative)




  **Data pre-processing and Machine learning model selection**
• Splitting the Data Sets Into X and Y by the dependent and independent variables (data 
selected by PCA)
• Build given models and measure their test and validation accuracy:

o LogisticRegression

o DecisionTreeClassifier

o RandomForestClassifier

o AdaBoostClassifier

o GradientBoostingClassifier

o KNeighborsClassifier

o XGBClassifier

• Whoever gives the most accurate result uses it and predicts the outcome is selected
![image](https://github.com/user-attachments/assets/9d61e60c-1d0b-48a4-adda-a0d2efba185f)

