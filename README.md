# Neural Network Charity Analysis
Practice with unsupervised machine learning

## Overview of the analysis: 
All charities cite beneficial goals. Not all charities achieve them.

As I learned neural networking, I examined a dataset of more than 34,000 organizations that the charitable giving fund, Alphabet Soup, had supported over the years. There was a lot of data, identifying information, classifying the data by industry, type, and government classification of the organizations, among other factors. 

The key or target column of the dataset was "IS_SUCCESSFUL," the follow-up classification that Alphabet Soup had used to assess the impact of their donation.

My job was to look through the rest of the data to figure out if any criteria could help the organization predict the effectiveness of future donations.

## Results: 

### Data Preprocessing
1. **What variable(s) are considered the target(s) for your model?**
- The target variable was pretty easy to figure out. **"IS_SUCCESSFUL"** was the key to the data. It was already set up in numerical data, with the successful grants receiving a "1" score and unsuccessful grants receiving a "0."
2. **What variable(s) are considered to be the features for your model?** 
- Since Neural Networking requires numeric data, I focused on the amount requested (ASK_AMT), the type of program (APPLICATION_TYPE), Income Amount, and any special considerations the grant had received.
3. **What variable(s) are neither targets nor features, and should be removed from the input data?**
- I removed the NAME nand EIN columns, as they were mere identifiers for the grants, and I was trying to look beyond specific grants to a bigger picture of the factors that affected the success of a grant.

### Compiling, Training, and Evaluating the Model
1. How many neurons, layers, and activation functions did you select for your neural network model, and why?
- I started with 4 neurons in layer 1 and 2 neurons in layer 2. That led to a loss of 75% and an accuracy of 53%. 
- Next I tried to use 8 and 4 neurons in the two layers. But my output was even worse, increasing loss by about 1% and decreasing accuracy by the same amount. 
- In my third try, I reduced the number of neurons to 2 in the 1st layer and 1 in the 2nd layer. The loss fell to 69%, and the accuracy increased to 55%, still well below my target accuracy of 75%
- I tried changing the activation functions to have sigmoids at both layers. I was never able to increase the accuracy significantly from my first result
2. Were you able to achieve the target model performance?
- No. I never got higher than 55% accuracy.
3. What steps did you take to try and increase model performance?
- I changed the number of neurons in each layer, and I tried to vary with tanh, sigmoid and relu activation functions.
 
## Summary: Summarize the overall results of the deep learning model. 
Alphabet Soup has done an excellent job of tracking donations over the years, and performing follow-up on the success of their grants (or lack thereof). But using deep learning/neural networking failed to find the critical connections to say with 75% accuracy or greater which factors were most significant to success.

Donating is still a judgment call, based on the individuals proposing and implementing the project. It's hard to predict which grants will succeed and which will fail.

*Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.*
I think a more focused study of the factors might yield a better result than a broad, deep-learning look at critical factors. They might look at specific categories of "USE_CASE" or "AFFILIATION", for example, to find which types of grants within those sectors are most successful.
