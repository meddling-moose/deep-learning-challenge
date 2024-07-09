# deep-learning-challenge

The data we used here has been used multiple times throughout the class. We got it from UCBerkeley teachers.

This assignment challenged me to push my neural network above 75% accuracy, and I was unable to accomplish this.

I learned, however, that adding hidden layers helped the accuracy increase. I also learned that I shouldn't take huge steps between number of nodes in a hidden layer from layer to layer. I learned that the tanh activation function was not very good for the final layer, and I learned that the selu activation function was pretty decent in the hidden layers.

I also messed about with decreasing some of the rarer cases in the categorical columns by binning them into other categories. It was unclear if this helped the accuracy, but it did not hurt it.

Data Preprocessing:
1. What variables are the target(s) of your models?

I selected is-successful as the target of my model; the column that represents the success of the venture.

2. What Variables are the features of your models?
- APPLICATION_TYPE
- AFFILIATION
- CLASSIFICATION
- USE_CASE
- ORGANIZATION
- STATUS
- INCOME_AMT
- SPECIAL_CONSIDERATIONS
- ASK_AMT

3. What variables should be removed from the input data because they are neither inputs nor features?

I removed EIN and NAME.

Compliling, Training, and Evaluating the Model

1. How many neurons, layers, and activation functions did you select for your neural network model, and why?

I selected at first 2, then 4, and then anywhere between 5 and 8 hidden layers. I wasn't able to get a good grasp on how many I should be using or why, but it seemed like the more the better.

I used between 40 and 80 neurons, almost always descending through the layers. This too was a bit of a shot in the dark. I followed some guiding principles online, but wasn't able to find a solution that worked.

2. Were you able to achieve the target model performance?

No I was not, but I was as close as 74%

3. What steps did you take in your attempts to increase model performance?

I added hidden layers, changed the number of nodes, switched up activation functions, and binned rare occurances of some categories.