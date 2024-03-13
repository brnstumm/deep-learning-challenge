# deep-learning-challenge

**1.	Overview of the analysis:** The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. The focus of the project is to identify the type of application that will be successful donors to the charity.  To accomplish this, we focused on the application type and the classification of the donors. The goal was to have a success rate of at least 75%. 
**2.	Results: 
Data Preprocessing**
o	What variable(s) are the target(s) for your model?
The variable target is “IS Successful”.  
o	What variable(s) are the features for your model?
APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT
o	What variable(s) should be removed from the input data because they are neither targets nor features?
EIN and NAME

**Compiling, Training, and Evaluating the Model**
o	How many neurons, layers, and activation functions did you select for your neural network model, and why?
o	Neurons: 80 and 30 in the original code
o	Layers: 2 layers
o	Activation functions: relu, sigmoid, & leaky_relu
o	Were you able to achieve the target model performance?
No.  I altered many factors in the process to increase the accuracy with no success!
o	What steps did you take in your attempts to increase model performance?
In the first attempt, I group all application types less than 1000 into one group titled ‘other’.  For classifications, I grouped any that were less than 1000 together.  I got a 72.47% accuracy with my first attempt.
In the second attempt, I changed the grouping for both application and classification hoping to limit the number of features being used in the model.  I adjusted the nodes to 110 and 40 in an attempt to increase the first layer and reduce the number of nodes in the second layer.  (I lowered the epochs from 100 to 75; however, nothing changed so I changed the epochs back to 100) (accuracy was 72.39%)
In the third attempt, I changed the activation functions and used leaky_relu hoping to provide better results.  It did increase the accuracy; however, it was very minimal (72.73%).
**3.	Summary: **
Although I did not reach the goal of 75%, the results would make me reconsider a new model to use for this data.  Increasing and decreasing the epochs did nothing to the accuracy.  Changing the groupings for larger columns did little to the accuracy as well.  (perhaps I should create more groups!).  Playing around with the nodes again did little to the accuracy percentage.  In attempt 2, I saw the accuracy decrease when I changed the nodes for both first and second.  From my testing, I would look into another model to see if I got better results.
