# neural-network-challenge-2


This program read in data about a company's employes including if they were going to leave the company, and created a branched neural network to predict if they were going to attrit and what department they were from.

There were also some questions at the end of the assignment that I have answered there and will repeat here:

### Summary

In the provided space below, briefly answer the following questions.

1. Is accuracy the best metric to use on this data? Why or why not?
- I would say that accuracy is the most important measure becuase we need to know which department the people who are attriting are from, and its imparitive that we correctly guess who is going to attrit so that we do not push out anybody accidentally by treating them as if they were going to leave anyway, while likewise not wasting resources on people who are about to leave.

2. What activation functions did you choose for your output layers, and why?
- I chose sigmoid for "Department" and softmax for "Attrition". I chose sigmoid for "Department" becuase a person can only belong to one department, therefore they should be considered independently of each other, and if we add a department in the future that our system was not trained on it will show that the person does not belong to any of the existing departments by giving low values to each instead of forcing all the values to add to 1. I chose softmax for "Attrition" because it was a binary output where I had 2 output nodes. Doing it like this we can choose the higher scoring of the two outputs to say if it was a yes or a no.

3. Can you name a few ways that this model might be improved?
- Having more data would probably help, there was not very many people who worked in HR in this dataset and it probably threw off results. Adding more layers might also help, I only added 2 layers shared layers but having more might help the algorithm learn better.


## Works Cited
How to make the input layer: https://wandb.ai/ayush-thakur/dl-question-bank/reports/Input-Keras-Layer-Explanation-With-Code-Samples--VmlldzoyMDIzMDU