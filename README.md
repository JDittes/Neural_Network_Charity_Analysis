# Neural Network Charity Analysis
Practice with unsupervised machine learning

## Overview of the analysis: 
All charities cite beneficial goals. Not all charities achieve them.

As I learned neural networking, I examined a dataset of more than 34,000 organizations that her fund, Alphabet Soup, had supported over the years. There was a lot of data, identifying information, classifications that identified the industry, type, and government classification of the ortaniations, among other factors. 

The key or target column of the dataset was "IS_SUCCESSFUL," the follow-up classification that Alphabet Soup had used to assess the impact of their donation.

My job was to look through the rest of the data to figure out if any criteria could help the organization predict the effectiveness of future donations.

## Results: 
Using bulleted lists and images to support your answers, address the following questions.

## Data Preprocessing
1. **What variable(s) are considered the target(s) for your model?**
- The target variable was pretty easy to figure out. **"IS_SUCCESSFUL"** was the key to the data. It was already set up in numerical data, with the successful grants receiving a "1" score and unsuccessful grants receiving a "0."
2. **What variable(s) are considered to be the features for your model?** 
- Since Neural Networking requires numeric data, I focused on the amount requested (ASK_AMT), the type of program (APPLICATION_TYPE), Income Amount, and any special considerations the grant had received.
3. **What variable(s) are neither targets nor features, and should be removed from the input data?**
- I removed the NAME nand EIN columns, as they were mere identifiers for the grants, and I was trying to look beyond specific grants to a bigger picture of the factors that affected the success of a grant.

### Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
Were you able to achieve the target model performance?
What steps did you take to try and increase model performance?
Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
