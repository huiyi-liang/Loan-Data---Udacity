# Udacity Project: Prosper Loan Data Exploration

## Dataset

The data contains information regarding 113,937 loans, including interest rate, loan risk rating, borrower credit score, and other credit and loan attributes. The dataset can be found in [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv), with feature documentation available [here](https://docs.google.com/document/d/e/2PACX-1vQmkX4iOT6Rcrin42vslquX2_wQCjIa_hbwD0xmxrERPSOJYDtpNc_3wwK_p9_KpOsfA6QVyEHdxxq7/pub?embedded=True). For the analysis, the dataset was filtered to 15 attributes that could be used to predict loan interest rate. 17,113 data points were also removed from the dataset due to inconsistencies or missing information.

## Summary of Findings

In exploration, I found that there is strong relationships between loan interest, loan risk rating, and the borrower credit score. Interestingly, relationships between utilization rate, loan risk rating, and borrower credit score display similar patterns. I had initially surprising results where lower credit scores were associated to lower interest rates for more risky loans. After incorporating the loan origination year into the analysis, I discovered that these types of loans were only provided prior to 2009, which leads me to believe that this may be related to stricter lending regulations after 2009.

Outside the main variables of interest, I found an interesting interaction of credit score, risk rating, and income on loan original amount. As credit score, risk rating, and income decrease, loan original amount shows a more narrow distribution centered around low amounts.

## Key Insights for Presentation

For the presentation, I focused mainly on the influence of loan risk rating and credit score, leaving out most of the intermediate derivations. I started by introducing the distribution of the interest rate, risk rating, and credit score variables. Then, I used violin plots to introduce the intereactions between the interest rate and these two categorical variables. Afterwards, I used a count plot to show the intereaction between risk rating and credit score. From there, I leveraged point plots to demonstrate the clear influence of risk rating, credit score, and loan origination year on interest rate.