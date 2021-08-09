# clothes_size_prediction
mutliclass classification task


the objective of the task is to predict the cloth size (from XXS to XXXL, 7 different sizes overall) based on 3 available variables: age, height, weight.
I first performed EDA in order to idnetify relevant variables and potential outliers (found several rows with not realistic combination of values for the different features which I decided to remove)
I then identify relevant variables (I ended up discarding the age variable as it was not proving to be helpful in predicting the size and I applied some transformations to the remaining variables).
With the remaining variables I performed PCA and created different models using the new Principal components rather than the original variables.
I then created different models with the original variables and compared results of all models.

I obtained the best results with KNN using the original variables (accuracy, weighted precision and weighted recall all equal to 57%).
