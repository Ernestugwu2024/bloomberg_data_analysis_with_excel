# Analysis and visualization of P&L data in excel

## Preview of Data  
   This data is a detailed Bloomberg extraction, outlining financial information over multiple fiscal years from 2016 to 2023. It provides an in-depth view of revenues, segmented by product, brand and geographic area,along with a breakdown of operating expenses,gross profits,net income and earnings per share(EPS). Specific figures for wholesale,retail,and other businesses are detailed across various regions,offering a comprehensive insight into the financial performance of the ticker “ADS GY Equity.  

# PROCEDURE IN ANALYZING THE DATA.  

- ### Creation of P&L structure  
   Before preparing a concise P&L structure for the last five years,the source data and structure was examine and the following was observed at the outset of the data; company thicker,full company name,periodicity of financial statements,currency and measuring unit  

The Bloomberg spreadsheet has many details,but I focused on the following steps  


- identifying mnemonics that signal major P&L items,making the end of breakdown  
- Selecting the table and filtering non-blank cells in column B to hide deeper breakdowns  

#### This approach helps isolate essential information and streamlining the process of creating the P&L structure  
![solution picture ref](/images/Picture1.png)  

By filtering ,I obtained a structured that allows me to easily mark in yellow the figures I want to see in the report such as: Revenue ,Cost of Revenue,Gross profit,Operating Expenses and Operating income (equal to EBIT)  

![solution picture ref](./images/Picture2.png)  

To organize the P&L,the header containing the financial period from the source table was copied.  

![solution picture ref](/images/Picture3.png)  

To address the leading space issue a new column inside the report sheet that will be hidden was inserted,then I proceeded to removing the leading spaces to improve the formatting of the P&L table.  

![solution picture ref](/images/Picture4.png)  

As indicated in the task instructions,I changed the name  ‘operating income to EBIT. The P&L sheet was formatted properly by adding  an empty column for breathing space,by adding a clear indication of totals and subtotals and highlighting the header better and indicating the measurement units in the P&L header  

Populating of the new sheet,lookup source data, caculation of margings and growth rates
After formatting the P&L correctly,data was transferred from the source sheet into the new table. To ensure precision a nested lookup function was utilize considering two criteria; financial items on the left and the period under analysis in the table’s .  

**INDEX, MATCH,MATCH combination excel function was use to populate the Report shee**  

![solution picture ref](/images/Picture5.png)  

After transferring the numbers using lookup functions I added a check row at the bottom of my table, this allow me to determine whether I have made any mistakes,after which I compared these figures with those in my report .if the difference is zero,it confirms that I have worked correctly  

![solution picture ref](/images/Picture6.png)  

But it was not zero so I returned to the source sheet and observed i overlooked one of the items with a mnemonic code  

![solution picture ref](/images/Picture7.png)  

After including the row in the P&L statement and the check shows that the work is correct ,I added a few rows to make it easier to understand the firm’s Growth Profit and EBIT margins and their five-year revenue growth rate. CAGR was used as the measure for revenue growth.  
![solution picture ref](/images/Picture8.png)  

The CAGR was calculated using the following formula;  
![solution picture ref](/images/Picture9.png)  

The formula in excel appears as such  

![solution picture ref](/images/Picture10.png)  


# Visualization of the data  
  To illustrate how different business lines contributed to revenue,I created a stacked column chart,I selected the revenue breakdown figures and chose the following type of visualization from the insert tab  

  ![solution picture ref](/images/Picture12.png)  

  Additionally, to display a secondary line that allows us to see the company ‘s profitability (EBIT%)during the period under analysis.I edited the chart by right clicking on it and select Data option, I named it EBIT% and select the EBIT% from the P&L statement.After adding the EBIT% series to the chart,I indicated that i want it to displayed on a secondary axis.  
  This was achieved by right-clicking on one of the more extensive series in the chart,selecting format Data series,then going to series options and choosing the series with name EBIT%  

  ![solution picture ref](/images/Picture13.png)  

  ![solution picture ref](/images/Picture14.png)


