# Project 4 - Data Visualization of Prosper Loans Dataset

This is the fourth (last) project of the Udacity Data Analytics Nano degree.

### Goal: 
Use Python data science and data visualization libraries to explore Prosper Loans dataset’s variables and understand the data’s structure, oddities, patterns and relationships.

### Dataset:
I used the ProsperLoans dataset that contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others.


### Other files:

1. Data_Visualization_of_Prosper_Loans_Data.ipynb file is where I have performed all exploratory data analysis along with data visualizations. This is a Jupyter Notebook file and contains univariate, bivariate and multivariate exploration. 

2. Data_Visualization_of_Prosper_Loans_Data.html is an HTML file converted from Data_Visualization_of_Prosper_Loans_Data.ipynb Notebook.

3. Data_Visualization_ProsperLoans_SlideDeck.ipynb is where I have used a Slide deck format to only display the visualizations I want to see in the deck. 

4. Data_Visualization_ProsperLoans_SlideDeck.slides.html is the slide deck for this project.

5. output_toggle.tpl file was used to convert Data_Visualization_ProsperLoans_SlideDeck.ipynb file into a slide deck format without including code.

### Exploratory Findings:

Univariate Analysis
1. Plotted a bar chart of Number of loans by borrower's employment status and observed that maximum number of borrowers (~ 68,000) are within employed status. 
2. There are about 25,000 borrowers who are employed full-time while the least number of borrowers are retired.

Bivariate Analysis
1. Plotted a heat map for a set of numeric variables (Term, BorrowerRate, StatedMonthlyIncome, LoanOriginalAmount, BorrowerAPR)
  a. Borrower's monthly income and borrower's interest rate are negatively correlated with a value of -0.329. <br/>
  b. Borrower's original loan amount is negatively correlated with Borrower's APR. Thus we can say that borrowers who take a loan for large amounts will be receiving smaller APR and corresponding interest rate. <br/>
  c. It can also be seen that monthly income of the borrower is positively correlated with the loan original amount. <br/>
  d. The highest positive correlation is between borrower's interest rate and borrower's APR which makes sense as APR is nothing but interest rate plus fees. <br/>
2. Plotted a clustered bar chart of number of loans by borrower's employment status across loan term and observed the following:
  a. Maximum number of borrowers were under employed status and had taken 36 month term loan, followed by those with employment status as full time. <br/>
  b. In every category, it can be observed that 36 month term loan is most common. Most frequently used term for loans borrowed was 36 months by employed and full time borrowers. <br/>
3. Plotted a scatter plot of borrower's original loan amount versus borrower's APR and observed that the range of APR is wider for smaller amounts of loan. This range becomes smaller and the APR reduces with large amounts of loan amount. Thus it can be seen that loan original amount is negatively correlated to Borrower's APR.
4. Borrowers lending a large loan amount seem to take a longer loan term.
5. Borrower's APR is higher for those rated lowest by Prosper Loans. (HR) Prosper Loan Rating has an impact on Borrower's APR.
6. Self-employed, employed and full time employed borrowers have a higher monthly income compared to others.

Multivariate Analysis
1. Maximum borrowers took a loan for the term of 36 months.
2. The range of Borrower's APR for the term 36 months is the broadest compared to other loan terms and most of the loan's original amount is between 0 to 10K.
3. We can also see that with larger amounts of the loan, the range of borrower's APR decreases across all loan terms.
4. It is interesting to see that borrower's APR is less for those rated in the AA category. This keeps increasing as we go through all rating categories. The borrower's APR is the highest for categories D, E and HR.
5. It is also interesting to see that very few borrowers fall in category HR. Maximum borrowers fall in the category A, B, C and D.
6. At the same time as we go through plots for Prosper Rating A, B, C and D, the range of borrower's APR keeps increasing with the maximum range for borrowers categorized with rating HR. The smallest range for APR is for those borrowers categorized in rating AA.

### Key Insights: 

1. Borrower's original loan amount and Prosper Loan's rating have an important effect on predicting borrower's APR. This makes sense as the more a borrower borrows from Prosper Loans, the lesser the APR. Borrowers rated less by Prosper Loans are least credible and end up paying more APR compared with those rated really high.
2. As Prosper Loans ratings decreases, the range of borrower's APR increases. This is a possibility as those with less ratings become less credible. Hence they may receive a higher APR.
3. Self-employed, employed and full time employed borrowers have a higher monthly income compared to others.
4. Maximum borrowers prefer a loan term of 36 months followed by 60 months. Borrowers lending a large loan amount seem to take a long loan term.
