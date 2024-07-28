Deep Learning Report

The report should contain the following:
1.	Overview of the analysis: Explain the purpose of this analysis.
2.	Results: Using bulleted lists and images to support your answers, address the following questions:
•	Data Preprocessing
o	What variable(s) are the target(s) for your model?
    - Used "IS_SUCCESSFUL," which had binary [0] and [1] responses from application_df
o	What variable(s) are the features for your model?
    - Features are the other columns from the same dataframe. This includes Status, ASK_AMT, APPLICATION_TYPE_Other, APPLICATION_TYPE_T10	APPLICATION_TYPE_T19, APPLICATION_TYPE_T3, APPLICATION_TYPE_T4, APPLICATION_TYPE_T5	APPLICATION_TYPE_T6	..., INCOME_AMT_1-9999, INCOME_AMT_10000-24999, INCOME_AMT_100000-499999, INCOME_AMT_10M-50M, INCOME_AMT_1M-5M, INCOME_AMT_25000-99999, INCOME_AMT_50M+, INCOME_AMT_5M-10M, SPECIAL_CONSIDERATIONS_N, SPECIAL_CONSIDERATIONS_Y. Processing was completed through the dropping of the "IS_SUCCESSFUL" column for those analyses. 

o	What variable(s) should be removed from the input data because they are neither targets nor features?
    - "EIN" and "NAME" columns 
•	Compiling, Training, and Evaluating the Model
o	How many neurons, layers, and activation functions did you select for your neural network model, and why?
    - I used 16 hidden nodes from layer1 and 16 in layer 2. I had decided to try these numbers based on some class practices, but this had been a random guess and I was hoping to use that for future further optimization.

o	Were you able to achieve the target model performance?

    I did not achieve the target model performance of 75%. 

o	What steps did you take in your attempts to increase model performance?

    I attemped to increase model performance by amending activation functons associated with the layers, change in epoch numbers. 

3.	Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.

My deep learning model had approximately 72% accuracy in prediction of Classifciation. To improve this accuracy, we should consider data analysis by a different classification model. 