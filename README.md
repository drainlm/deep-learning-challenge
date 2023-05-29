# deep-learning-challenge ReadMe

The purpose of this analysis was to create a binary classifier to predict whether or not an applicant will be successful if funded by the Alphabet Soup charity. The goal was to achieve an accuracy above 75%.

1. What variable(s) are the target(s) for your model?
   IS_SUCCESSFUL
2. What variable(s) are the features for your model?
   APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT
3. What variable(s) should be removed from the input data because they are neither targets nor features?
   'EIN' and 'NAME'
4. How many neurons, layers, and activation functions did you select for your neural network model, and why?
   This varied across the attempts. I attempted to use Keras Tuner to give me the best model summary, though it still fell short.
5. Were you able to achieve the target model performance?
   No, 73% was the highest achieved accuracy.
6. What steps did you take in your attempts to increase model performance?
   I removed USE_CASE as a column (later adding it back in), created more bins for rare occurrences in columns, increased the number of values for each bin, added more neurons to hidden layers, added more hidden layers, used different activation functions for the hiddne layers, and added the number of epochs to the training regimen.

Summary:
Overall, accuracy above 75% was not achieved. Perhaps a decision tree or random forest would perform bettr. There may also be more sophisticated Hyperparamater tuning available.
