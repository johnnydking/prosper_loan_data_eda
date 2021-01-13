# prosper_loan_data_eda.ipynb
## by John King


## Dataset

> The dataset used in this analysis contains detailed information on loans including borrower income and credit details, loan origination details, as well as loan status and loss information. It consists of appx 114,000 rows with 81 feature columns.


## Summary of Findings

> I found that Prosper's rating profile follows a normal distribution of ratings, with most loans being disbursed to average borrowers. Average credit score has a fairly linear relationship to Prosper Rating, although credit score does not have a strong relationship to borrower APR, suggesting that other credit factors play a role in determining Prosper Score.  
>
>A correlation matrix explores relationships between credit features and Prosper Rating/Score. Credit Score and available credit have positive correlations, while debt to income ratio, credit utilization and delinquency have negative correlations. Surprisingly, employment status duration and stated monthly income carry little to no weight in determining borrower rating. Prosper Rating and Score are highly determinative of a borrower's APR.
>
>Prosper Rating is much more accurate in predicting risk when compared to Prosper Score. Prosper Rating displays a linear relationship to chargeoff, default and delinquency, while Prosper Score displays very unexpected results. Prosper Rating has a much stronger correlation to APR than Prosper Score.
>
>While employment status duration and stated monthly income have no correlation, they do provide insight into where chargeoff typically occurs, and segmenting borrower population along these feature lines reveals instances where less risky borrowers are being rated lower than riskier borrowers and therefore paying a higher APR.



## Key Insights for Presentation

> The explanatory presentation focuses on credit feature correlation, the accuracy of rating systems in predicting risk, Prosper Rating's dominant role in determining borrower APR, the significance of employment status duration and stated monthly income, and revealing contradictions in the rating model by segmenting borrower population.
>
>Minor changes were made to polish plots created during EDA, to add titles and labels where needed.


## Resources

> The code used to create the clustered bar chart that displays chargeoff rate and APR for segmented borrowers was taken from Stack Overflow. The user's name is Paul H.  
https://stackoverflow.com/questions/40877135/plotting-two-columns-of-dataframe-in-seaborn
