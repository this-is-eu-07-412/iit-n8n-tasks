# Labolatories Week 10: Task A

## 1. Workflow overview

- Here's the node config, as instructed with addition of error handling if request to Chat GPT returns an error.

![alt text](<L10_Screenshots/L10B_Screenshots/L10B_Screenshot (1).png>) 

## 2. Node configuration

- Webhook listens for url, url has to be valid (such error isn't accounted for) which is then sent to r.jina.ai to "decompose" the site and return it as JSON.

![alt text](<L10_Screenshots/L10B_Screenshots/L10B_Screenshot (2).png>) 
![alt text](<L10_Screenshots/L10B_Screenshots/L10B_Screenshot (3).png>) 

- That JSON is then passed with prompt to Chat GPT to summarise the website contents and present it as JSON with instruction-specified fields. Whole prompt is visible on [L10B_Screenshot (6).png](<L10_Screenshots/L10B_Screenshots/L10B_Screenshot (6).png>).

![alt text](<L10_Screenshots/L10B_Screenshots/L10B_Screenshot (4).png>)
![alt text](<L10_Screenshots/L10B_Screenshots/L10B_Screenshot (5).png>) 
![alt text](<L10_Screenshots/L10B_Screenshots/L10B_Screenshot (6).png>) 
![alt text](<L10_Screenshots/L10B_Screenshots/L10B_Screenshot (7).png>) 
![alt text](<L10_Screenshots/L10B_Screenshots/L10B_Screenshot (8).png>) 

- These two nodes take care of errors returned by r.jira.ai by displaying recevied error message.

![alt text](<L10_Screenshots/L10B_Screenshots/L10B_Screenshot (9).png>) 
![alt text](<L10_Screenshots/L10B_Screenshots/L10B_Screenshot (10).png>) 

## 3. Testing

- Testing for url=https://github.com. Results contain all requested fields but if there's too little data AI halicinates anwsers just to spit out something.

![alt text](<L10_Screenshots/L10B_Screenshots/L10B_Screenshot (11).png>) 

- Testing error handling in case website contents are too long for free version of groq.

![alt text](<L10_Screenshots/L10B_Screenshots/L10B_Screenshot (12).png>)