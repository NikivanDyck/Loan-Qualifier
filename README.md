# Loan Qualifier Application 

![home, money image](https://www.crcu.org/assets/files/CS5QBqdL/CalculatorandHand1330x400.png)
### The application will allow users to input key data points to quickly obtain a list of qualified loans.  The application can be used mortgage brokers and loan servicing professionals, to support their customers 

---
## User Expectations 
### Steps a user must take to use the loan qualifier application. 

1)	Save a daily rate sheet that contains all lender offerings as a CSV file on your computer.  This file must contain a header that reflects Lender,Max Loan Amount,Max LTV,Max DTI,Min Credit Score,Interest Rate.  An example is located here:  file path 
2)	Enter the file path of the location of the daily rate sheet, here is an example of what your path should look like in Microsoft File Explorer  C:\Users\Desktop\Bank_Rates\daily_rate_sheet.csv
3)	You will be prompted for the following items:  Credit Score, Monthly Debt, Monthly Income, Loan Amount, Home Value. 
4)	You will be notified of the number of loans that the applicate is qualified for and the results will be print in a CSV file for your review. 

---
## Technology Overview

The application relies on a daily rate sheet of banking vendors.  The data is then parsed into 4 different qualifying filters to review applicants criteria.  1) Credit Score 2) Debt to Income 3) Loan to Value 4) Max Loan size. (criteria definitions in Appendix A).   Utilities required for calculations used to determine loan to value and debt to income are held within “calculations”.  Tools used to read and save CSV data are stored in “fileio”.  The applicatication is to run in appy. 
```
Tip:  Update the "daily rates sheet" for the loan qualifier application to be accurate.
```

---
## Technology Mapping

![<diagram of app mapping> (https://github.com/NikivanDyck/Loan-Qualifier/main/mapping.PNG)]  

---
## Definitions

| Term | Description | Calculation/ or Value |	
| :--- | :--- | :---: |
|*Credit Score*| The applicants credit score ass reported by the credit bureau | Value | 
|*Loan to Value Ratio (LTV)*|The % of home value the applicant to requesting. | Loan to Value = Loan Amount / Home Value |
|*Debt to Income Ratio (DTI)*|The % of free cash the applicant has available.|Debt to Income = Monthly Debt Payments / Monthly Income |
|*Monthly Debt Payment*|The applicants total monthly debt| Value | 
|*Monthly Income:*|The applicants total monthly income| Value | 
|*Loan Amount*|The requested loan amount| Value | 
|*Home Value*|The homes market value| Value | 
|*Max Loan Size*|The maximum amount a bank will lend| Value | 

---


