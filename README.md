# Neural Network - Charity Analysis

## Project Overview
This project mainly aims to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. Utilizing a data that has more than 34,000 organizations that have received funding from Alphabet Soup over the years, a neural network model will be built, trained, and tested to project whether an applicant should get the funding or not. So this is basically a classification model.

## Results

According to the purpose of the project, the following are the variables of the model:
- The "Is_SUCCESSFUL" variable is the target variable for the model.

While the remaining variables are used as features of the model:
- APPLICATION_TYPE—Alphabet Soup application type
- AFFILIATION—Affiliated sector of industry
- CLASSIFICATION—Government organization classification
- STATUS—Active status
- INCOME_AMT—Income classification
- SPECIAL_CONSIDERATIONS—Special consideration for application
- ASK_AMT—Funding amount requested

While the remaining variables were left out as they were neither target nor features.

Upon examining the data, variables were checked to determine the number of unique values in each column.

![image](https://user-images.githubusercontent.com/116329396/230694623-48122af4-ae1f-45d9-b790-391accfb1e35.png)

After that, each variable was examined individually to see the categories and try an basket them to limit the number of categories and make them more manageable. For example, the application type variable was divided into nine categories instead of 17 simply because some of the categories were significantly less than the other ones, and therefore were bucketed into one single category, i.e., other.
![image](https://user-images.githubusercontent.com/116329396/230694774-452de759-0875-4542-a7d6-33209213fa73.png)

The same procedures were done for the remaining features. After that, using OneHotEncoder all features were reshaped and merged with the original dataset. The original variables were removed, as well. Followig that, data were split into train and test and all data were scaled to prepare them for the model. Finally, the model was compiled, trained and evaluated. The model loss was at 0.56 while the accuracy was at 0.73. 
![image](https://user-images.githubusercontent.com/116329396/230695873-555d4e66-a5c2-4694-a8f1-e19c58573e9f.png)

The following chart shows the model loss.

![image](https://user-images.githubusercontent.com/116329396/230702845-48561d7f-c3ec-4c6e-b0f7-67dffc073684.png)

The following chart shows the model accuracy.

![Untitled](https://user-images.githubusercontent.com/116329396/230702873-9a016767-f91c-4b30-9930-4ca7692494dc.png)

## Summary

Overall, the model was optimized three times to improve accuracy and reduce loss. Two hidden layers were constructed along with one output layer. In the first layer, there were 80 neurons while the second layer contained 30. Other procedures might help the model yield better results, but given the time constraint, this was the optimal possible model. I would recommend looking at the outliers and probably reduce some of the features.
