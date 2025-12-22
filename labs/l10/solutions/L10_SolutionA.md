# Labolatories Week 10: Task A

## 1. Workflow overview

- Required configuration as specified in the instruction. **Some parts of the exercise are adjusted on the fly**, since the specified JSON input and output formats are different between current API and the one from the instruction but the core result is exactly the same. Modified parts are listed in section four.

![alt text](<L10_Screenshots/L10A_Screenshots/L10A_Screenshot (1).png>) 

## 2. Node configuration

- The workflow listens for user input at it's address with parameters with GET method. Then input from the query serves as input for http request to Chat GPT model which is tasked to tell a joke, on topic that has to be specified in earlier GET request, optionally temperature can also be provided. If request fails it's repeated 2 times before workflow throws an error.

![alt text](<L10_Screenshots/L10A_Screenshots/L10A_Screenshot (2).png>) 

![alt text](<L10_Screenshots/L10A_Screenshots/L10A_Screenshot (3).png>) 

![alt text](<L10_Screenshots/L10A_Screenshots/L10A_Screenshot (4).png>) 

![alt text](<L10_Screenshots/L10A_Screenshots/L10A_Screenshot (5).png>) 

- The response is then mapped into JSON that will be displayed as end result via respond to webhook node.

![alt text](<L10_Screenshots/L10A_Screenshots/L10A_Screenshot (6).png>) 

![alt text](<L10_Screenshots/L10A_Screenshots/L10A_Screenshot (7).png>) 

## 3. Testing

- Here are two results from executing the workflow, last of them is pasted into [requested JSON file](L10_ExerciseA.json). If topic is invalid or not specified, AI will only ask to specify it.

![alt text](<L10_Screenshots/L10A_Screenshots/L10A_Screenshot (8).png>) 

![alt text](<L10_Screenshots/L10A_Screenshots/L10A_Screenshot (9).png>)

## 4. Modifications 

1. Input has been modified in order to be acceptable for the API. Modified JSON request is visible [L10A_Screenshot (4).png](<L10_Screenshots/L10A_Screenshots/L10A_Screenshot (4).png>).

2. The output differs from instruction example and requested data isn't returned, so to compensate different data is displayed. 