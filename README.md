 **ATM Transaction Analysis**

I'm excited to share my latest Power BI project, where I developed a comprehensive dashboard to analyze ATM transactions across various states. 🏧 This project provides key insights into the performance and profitability of ATMs, helping stakeholders make data-driven decisions. Here’s a summary of what I worked on:

📊**Datasets Analyzed**
**Metrics:** Year, Month, Bank, ATM ID, State, Effective Days, Financial and Non-Financial Transactions, Monthly Revenue, MHA Revenue, Total Cost, Gross Profit, CRA, AMC, UPS AMC, and more.

🔄**Data Cleaning & Transformation:** I performed thorough data cleaning and transformation to ensure accurate analysis, including:Normalizing transaction data across multiple months

  **Measure**: Used Measures to calculate Gross profit % , Total Transaction , Revenue Per Transaction 

            Gross_Profit_Percentage = DIVIDE(SUM(Sheet1[ Gross Profit ]),SUM(Sheet1[Monthly Rev]),0)

            Total_transaction = Sheet1[Fin Txn]+Sheet1[Non Fin Txn]

            Revenue Per Transaction =  DIVIDE(
                                        [Revenue Performance - Copy],
                                        [Fin Txn] + [Non Fin Txn],
                                         0  -- Default value in case of division by zero
                                            )

 **key performance indicators:** Created KPI's such as average monthly transactions, revenue,uptime, Gross profit, gross profit percentage and total cost

 **Dashboard Template:** Created dashboard template using figma(https://www.figma.com/)
 
 
 <image src="https://github.com/Vijay-soundhariya/ATM-Transaction-Analysis-Dashboard/blob/main/ATM%20analytics%20template.png">


**Dashboard pictures**


💡**Key Insights:** Uncovered The analysis provided valuable insights such as:

  **>** **State-wise Revenue:** Identified top-performing states in terms of ATM revenue
  
  **>** **Monthly & MHA Revenue Trends:** Tracked revenue changes over time
  
  **>** **Cost Analysis:** Evaluated AMC and Spare UPS costs to optimize expenses
  
  **>** **Profitability:** Assessed gross profit and margin ranges for current months
