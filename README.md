# Bank Transaction Analysis for Fraud Detection 📊

A Comprehensive analysis I conducted on a bank transaction dataset, aiming to detect potential fraudulent activities. The project utilized Python for data manipulation, visualization, and implementing fraud detection mechanisms. Below are the details of the project.

## 📁 Dataset Overview
I worked with the Bank Transaction Dataset which contains 2,512 transaction records with various attributes such as transaction amounts, transaction types, customer ages, channels, and timestamps.Directly import dataset from kaggle.

## 🛠️ Methodology

### Data Loading and Initial Inspection:

The necessary libraries, such as Pandas, Numpy, Matplotlib, and Seaborn, were imported.
Loaded the dataset and performed initial inspections to understand its structure, check for missing values, and analyze date columns.

### Feature Engineering:

Time Since Last Transaction: Calculated the time difference between consecutive transactions for each account.

Transaction Frequency: Analyzed how often transactions occurred within a 30-day window.

Last and Cumulative Transaction Amounts: Derived metrics to summarize the financial behavior of accounts.

## Data Visualization:

### Transaction Amount Distribution: 
Utilized histograms to visualize the distribution of transaction amounts across different transaction types.

![Transaction Amount by Type](https://github.com/user-attachments/assets/ada8828d-bd9e-4c36-9c6a-66d6469368a2)


![transaction by card type](https://github.com/user-attachments/assets/1bd4340f-3582-40e0-b90c-b55d94324a33)


![distribute of amount](https://github.com/user-attachments/assets/7aedf180-91e1-4dcc-8ccb-19031cab1ffb)



### Channel Usage Patterns:
Created bar plots to show the number of transactions per channel.

![channel used](https://github.com/user-attachments/assets/73fb2856-f96a-4329-834a-21e2850f3781)


### Heatmap of Transactions:
Visualized transaction activity across different days and hours to identify peak transaction times.

![by day and hour](https://github.com/user-attachments/assets/4812a5e4-8e87-456a-bba1-39afd68ad059)

### Transaction by age Group
![by age](https://github.com/user-attachments/assets/b82f5a40-a82a-46d3-af85-9d92f8f3d1dc)


## Fraud Detection Mechanism:

Established criteria for identifying potential fraud:
-High transaction amounts (99th percentile threshold).

-Excessive login attempts (more than 3).

-Rapid transactions within a short time frame (less than 0.1 hours).

-Created a PotentialFraud column based on these rules.

## Analysis of Potential Fraud:

#### Counted fraudulent transactions per account and visualized the top accounts with the most potential fraud.

![Fraudulent acount](https://github.com/user-attachments/assets/c0edc256-78e5-4445-9765-8941e72c4566)


#### Box plots were used to compare transaction amounts between non-fraudulent and potentially fraudulent transactions.

![Fruad vs non-Fruad](https://github.com/user-attachments/assets/9a950ab8-4a44-42ef-bd11-1c7f4782fa18)


#### Analyzed the locations associated with potential fraud and visualized the data using bar plots.

![fraud by loc](https://github.com/user-attachments/assets/5416b806-95af-4ee8-ac59-ee82992a14ad)


#### Developed a pie chart to illustrate the proportion of transaction channels used in potentially fraudulent transactions.

![fraud by channels](https://github.com/user-attachments/assets/02221bbd-3e7a-4a23-8a51-009946d60936)



## 📊 Key Findings
### Transaction Behavior: 
The analysis revealed significant patterns in transaction behaviors based on account activities, such as high transaction amounts correlating with potential fraud.

### Potential Fraud:
Fraud accounts were found more than the non-fraud ones

### Time Sensitivity:
Quick successive transactions were a strong indicator of potential fraudulent activities.

### Channel Preference:
Certain channels exhibited higher transaction counts for potential fraud Like Branch and Online contain higher transactions then ATM, offering insights into which channels might need closer monitoring.



## 🚀 Tools and Technologies Used
Programming Languages: Python

Libraries: Pandas, NumPy, Matplotlib, Seaborn

Data Analysis Techniques: Data cleaning, feature engineering, and data visualization

📝 Conclusion

This project enhanced my skills in data analysis and provided a deeper understanding of fraud detection mechanisms within financial datasets. I look forward to applying these insights and techniques in future endeavors to enhance security measures in the banking and financial sectors.
