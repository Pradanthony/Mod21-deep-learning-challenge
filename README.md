Analysis of Alphabet Soup’s funding for ventures

Overview of the analysis

Alphabet Soup has provided funds to many organizations to help them succeed in their ventures. In this analysis we will be using the historical data from the funds provided in the past for many different ventures and their outcome to predict the outcome of the applicants ventures if funded by Alphabet Soup in the future. The analysis involved data processing, compiling a model, training and testing and evaluation of this model against the outcome. A deep learning model using neural networks was used to solve this classification problem. Our target performance evaluation is 85% accuracy.

Results

Data Processing:

•	The target variable is the “IS_SUCCESSFUL” column which gives the result of whether the venture was successful or not.

•	The Features of the model are variables ’APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS and ASK_AMT'

•	The variables "EIN" and "NAME" were removed from the input data as these variables are neither targets nor features.

Compiling, Training and Evaluating the Model:

•	Initially a basic model with 2 layers with 32 and 16 neurons respectively was used with activation function of relu and output layer activation function of sigmoid.

•	We were not able to achieve the target model performance of 85% with this model.

•	keras-tuner library was used to find the best model and even evaluating the best model did not help in achieving our target model performance.

•	The best model comprised of 11 neurons in the first layer and additional 5 layers with varying number of neurons in each layer and tanh activation function.

Summary

The deep learning model achieved a certain level of performance based on the analysis. However, the specific performance target of 85% could not be achieved. 
To solve this classification problem, a recommendation would be to consider using a Random Forest classifier. Random Forest models are effective for classification tasks and can handle a mix of numerical and categorical features. Additionally, Random Forest models offer interpretability and handle complex relationships within the data. It would be worth exploring this approach to compare its performance with the deep learning model.
