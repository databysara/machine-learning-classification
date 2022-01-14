### My Linear Classification Submission

#### Challenge

To look at the Lending Club data set and predict whether the loan will be "Fully Paid" or "Charged Off". 


#### What I did?
I developed a template for Linear Classification Projects including hyperlinked table of contents for easy flow.

### Import and Inspect Data:
- This helped me to understand the data. I researched the meaning of some of the terms like loan grade.
- I prerformed an initial linear correlation with uncleaned data and then reperform the linear correlation a cople times after data cleaning.
    - To manage analysis project I separated the analysis of Numerical values (Interest Rate, Annuual Income and Loan Amount) and Highly Correlated values (Interest Rate, Loan Grade and Loan Term.
- At this stage I also made decisions on:
    - On hot encoding:
        - How to group the data for e.g. Purpose of the loan - I grouped credit card payments and debt consolidation vs all others.
        - *IMPROVEMENT: In hindsight I should have split purpose into more groups.
        - loan grade was converted from A to G to 6 to 0.  
        - histplot helped show that to normalize annual income distrubution I had to limit income to 300,000  
            - *IMPROVEMENT: Use log scale
            
### Data Cleaning
- Then I actually carried out the data cleaning based on the decisions made in inspection.
- Once the data was cleaned I took only those parameters that had an absolute correlation of higher than 0.1 into the regression model.

### Visualization
- Used confusion Matrix to visalize results
- All or Most results were positive i.e. high no. of false positives and hence model is unable to predict if someone could not pay.

### Model Building
- Was very challenging. Was unable to find a model with AUC higher than 0.5

### Next Steps
- Try decision tree and random forest models.
- Reinspect and clean data: for e.g. improve one hot encoding for purpose and other parameters. 

