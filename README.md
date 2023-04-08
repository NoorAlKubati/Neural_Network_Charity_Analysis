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

The same procedures were done for the remaining features.
