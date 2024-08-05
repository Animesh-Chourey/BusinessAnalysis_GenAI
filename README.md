# Business Analysis Using Generative AI with Fine-Tuning LLM

The objective of this project is to fine-tune GPT-3.5 using OpenAI API and retrain the new LLM on customer complaints data which has the ability to retrieve the required data in the needed format.

## Description
The end goal is to improve customer satisfaction by examining customer complaints, and fix the issues. For that we will need a LLM that is efficient to extract certain needed details, mainly, topic of the problem, the problem itself, and the dissatisfaction-level of the customer, ranging from 0-100 denoting the level of irritability. 


### Steps:
* Install the environment dependencies and the module and libraries. Ensure to store the API key and ORG ID in a .env file.
* Convert each row of the data in the following format to be able to use it for fine-tuning purpose.
![](JSON format.png)
* Fine-tuning the model (GPT-3.5) by training it on the data:
    * Importing the training data and creating the fine-tuning job.
    * Train the new fine-tuned model created in the step above.
    * Evaluate the results and adjust accordingly. Here we can adjust the hyperparameters, i.e. number of epochs, batch size, learning rate.
    * Employ the fine-tuned model.
* While evaluating the performance of the fine-tuned model, focus on the two aspects of the training:
    * Training loss (should be decreasing with each step taken).
    * Training mean accuracy (should be increasing with each step taken).
* Deploy the model and observe how it is performing on some test statements.