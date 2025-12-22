# Labolatories Week 9: Task A

## 1. Creating a workflow

- After opening n8n, I create new workflow and name it properly

![alt text](L9_Screenshots/L9A_Screenshots/L9A_Screenshot1.png)

## 2. Setting up the nodes

- Screenshots below show step-by-step configuration of nodes. First webhook catches when user uses path to that webhook with get path 'event'. If so, Java Script code gets the event's value, while handling lack of such, as well as getting the timestamp at which it got executed and returns JSON. that JSON is later sent by respond to webhook node with HTTP code 200 (success).

![alt text](L9_Screenshots/L9A_Screenshots/L9A_Screenshot2.png)

![alt text](L9_Screenshots/L9A_Screenshots/L9A_Screenshot3.png)

![alt text](L9_Screenshots/L9A_Screenshots/L9A_Screenshot4.png)

![alt text](L9_Screenshots/L9A_Screenshots/L9A_Screenshot5.png)

![alt text](L9_Screenshots/L9A_Screenshots/L9A_Screenshot6.png)


## 3. Testing

- Below screenshots from testing the workflow: view from workflow, accessing the URL with specified 'event', then without such and lastly testing the same on activated workflow.

![alt text](L9_Screenshots/L9A_Screenshots/L9A_Screenshot7.png)

![alt text](L9_Screenshots/L9A_Screenshots/L9A_Screenshot8.png)

![alt text](L9_Screenshots/L9A_Screenshots/L9A_Screenshot9.png)

![alt text](L9_Screenshots/L9A_Screenshots/L9A_Screenshot10.png)