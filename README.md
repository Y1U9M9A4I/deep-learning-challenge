# Deep Learning Report #

o	Please note all analyses and process work can be viewed under the file "AlphabetSoupCharity_Optimization.ipynb"

## Report Details ##

1.	Overview of the analysis: Explain the purpose of this analysis.
2.	Results: Using bulleted lists and images to support your answers, address the following questions:
   
### Data Preprocessing ###
o	What variable(s) are the target(s) for your model?
o	What variable(s) are the features for your model?
o	What variable(s) should be removed from the input data because they are neither targets nor features?

### Compiling, Training, and Evaluating the Model ###
o	How many neurons, layers, and activation functions did you select for your neural network model, and why?
o	Were you able to achieve the target model performance?
o	What steps did you take in your attempts to increase model performance?

### Results ###

** Data Preprocessing **

1. What variable(s) are the target(s) for your model?

   The variables I used as the target for my model is "IS_SUCCESSFUL," which had binary [0] and [1] responses from application_df.
   
2. What variable(s) are the features for your model?

   The features used in this model are the other columns from the same dataframe. This includes Status, ASK_AMT, APPLICATION_TYPE_Other, APPLICATION_TYPE_T10	APPLICATION_TYPE_T19, APPLICATION_TYPE_T3, APPLICATION_TYPE_T4, APPLICATION_TYPE_T5	APPLICATION_TYPE_T6	..., INCOME_AMT_1-9999, INCOME_AMT_10000-24999, INCOME_AMT_100000-499999, INCOME_AMT_10M-50M, INCOME_AMT_1M-5M, INCOME_AMT_25000-99999, INCOME_AMT_50M+, INCOME_AMT_5M-10M, SPECIAL_CONSIDERATIONS_N, SPECIAL_CONSIDERATIONS_Y. Processing was completed through the dropping of the "IS_SUCCESSFUL" column for those analyses.

3. What variable(s) should be removed from the input data because they are neither targets nor features?

   Variables "EIN" and "NAME" were removed from the input data because they were neither targets nor features.
   
** Compiling, Training, and Evaluating the Model **

1. How many neurons, layers, and activation functions did you select for your neural network model, and why?

   I used 16 hidden nodes in layer1 and 16 in layer 2. I had decided to try these numbers based on some class practices, but the intention was to use this as a baseline framework for which future optimization can be applied.
   
2. Were you able to achieve the target model performance?

   I did not achieve the target model performance of 75%. My modifications led to a target model performance of 72%, which did not increase in comparison to pre-modification.
   
3. What steps did you take in your attempts to increase model performance?

   I attemped to increase model performance by amending activation functions associated with the layers, as well as modifications in the epoch numbers.

### Overview ###

My deep learning model had approximately 72% accuracy in prediction of Classifciation. Optimization tuning of model parameters such as activation functions and epoch did not significantly improve the accuracy. To attempt for improved accuracy, other parameters such as neuron numbers and layer numbers could still be modified for obeservation of effect. Other classification models may also create a neural prediction model more suited for this dataset.  
