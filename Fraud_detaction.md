                            ML Problem Framework: Credit Card Fraud Detection System


Step 1: Understand the Business Problem

        A Institute process approximately 10 million credit card transactions every day.
        Around 0.1% of transactions are fraud. Institute wants to identify fraud transaction before they are approved  
        Cost of average fraud  $100, Cost of one fraud detection $5
        Current fraud detection: Random 

Step 2: Frame as ML Problem

        Type: Binary Classification
        Target:- Is Transaction correct or not (Card details correct or not)
        Recall >= 95% (Every missed fraud cost $100, catch 95% fraud) 
        Precision >= 70% (out of all model prediction how many correct)
        Why:- missing a fraud detection cost is $100, and cost of fraud detection = $5

Step 3: Data Requirements

        customer info (Customer id, Age, Gender, Credit card score, customer location)
        transaction info (transaction amount, Merchant id, transaction timestamp, payment method)
        Device Info (device id, Ip Address, OS)
        Historical info (previous transaction history, Avg transaction amount)
        Location info (city, country, GPS Location)

Step 4: Feature Engineering 

        Average transaction amount
        Transaction in last hour
        Location of last merchants visited 

step 5: PitFalls
        1) Data leakage 
            -> do not use information that after the transaction
            Bad information  => Future account balance
            Good information => current tranction details,device information
        
        2) Class Imbalace:- fraud represent only 0.1% 
                solution :- threshold tuning,training data only
        
        






 




