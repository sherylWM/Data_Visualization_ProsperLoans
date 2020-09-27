# Project 4 - Data Visualization of Prosper Loans Dataset

This is the fourth (last) project of the Udacity Data Analytics Nano degree.

## Goal: 
Use Python data science and data visualization libraries to explore Prosper Loans dataset’s variables and understand the data’s structure, oddities, patterns and relationships.

### Dataset:
I used the ProsperLoans dataset that contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others.


### Other files:

Data_Visualization_of_Prosper_Loans_Data.ipynb file is where I have performed all exploratory data analysis along with data visualizations. This is a Jupyter Notebook file and contains univariate, bivariate and multivariate exploration. 

Data_Visualization_of_Prosper_Loans_Data.html is an HTML file converted from Data_Visualization_of_Prosper_Loans_Data.ipynb Notebook.

Data_Visualization_ProsperLoans_SlideDeck.ipynb is where I have used a Slide deck format to only display the visualizations I want to see in the deck. 

Data_Visualization_ProsperLoans_SlideDeck.slides.html is the slide deck for this project. 

### Exploratory Data Analysis:

I did an initial prelimiary data wrangling and included only columns/variables that I would like to explore to understand their impact on predicting the main variable of interest. 

#### Research Question: 
What are the most important features to predict a borrower's APR?

#### Univariate Analysis:
1. Borrower's APR and Interest rate are unimodal and similar in nature. Most of the values for APR were between 0.05 and 0.42. Borrower's monthly income is unimodal in nature and right skewed. Borrower's original amount of the loan had a peak at 5000 and some peaks at 10K, 15K, 20K.

#### Bivariate Analysis:
1. The highest positive correlation is between borrower's interest rate and borrower's APR which makes sense as APR is nothing but interest rate plus fees. <br/>
2. The loan original amount is negatively correlated with Borrower's APR. Thus we can say that borrowers who loan for large amounts will be receiving smaller APR. It can be seen that the range of APR is wider for small amounts of loan in the scatter plot. This range becomes smaller and the APR reduces with large amounts of loan amount. <br/>
3. Lastly, Borrower's APR is higher for those rated lowest by Prosper Loans. (HR) Prosper Loan Rating has an impact on Borrower's APR.
Thus overall I can say that loan original amount and ProsperLoanRating do have an impact on Borrower's APR and are features that can help predict a Borrower's APR. <br/>

For non-main features of interest there were some interesting relationships that could be observed.

1. The monthly income of the borrower is positively correlated with the loan original amount.
2. The highest positive correlation is between borrower's interest rate and borrower's APR which makes sense as APR is nothing but interest rate plus fees.
3. Maximum number of borrowers were employed and had taken 36 month term loan.
4. Most frequently used term for loans borrowed was 36 months by employed and full time borrowers followed by self employed borrowers.
5. The range of APR is wider for small amounts of loan. This range becomes smaller and the APR reduces with large amounts of loan amount. Thus it can be seen that loan original amount is negatively correlated to Borrower's APR.
6. There seems to be a relationship between Loan original amount and term. Borrowers lending a large loan amount seem to take a longer loan term.
7. Self-employed, employed and full time employed borrowers have a higher monthly income compared to others.

#### Multivariate Analysis:

### Explanatory Analysis:
