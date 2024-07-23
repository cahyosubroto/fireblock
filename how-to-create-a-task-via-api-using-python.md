---
title: "How to Create a Task via API"
slug: "how-to-create-a-task-via-api-using-python"
excerpt: ""
hidden: false
createdAt: "Tue Jul 23 2024 17:57:39 GMT+0000 (Coordinated Universal Time)"
updatedAt: "Tue Jul 23 2024 18:38:05 GMT+0000 (Coordinated Universal Time)"
---
In this guide, you will learn how to create a task using our API in Python and JavaScript.

### Step 1. Create a Fireblock account and generate an API key

1. Login/Sign up to [Fireblock console](https://console.fireblocks.io/v2/).
2. Navigate to the API section.
3. Add a new user and generate a new API key.

### Step 2. Perform an API request

Copy the snippet below and replace the `YOUR_API_KEY`, `taskname`, `tasktitle`, `taskdescription`, `OPEN`, `API_DOCS`, and `connectedtask` value with the real value. For details, please refer [here](https://fireblock-cayo.readme.io/reference/addtask).

```javascript
const options = {
  method: 'POST',
  headers: {
    accept: 'application/json',
    'content-type': 'application/json',
    'X-API-KEY': 'YOUR_API_KEY'
  },
  body: JSON.stringify({
    task_id: 'taskname',
    title: 'tasktitle',
    description: 'taskdescription',
    status: 'OPEN',
    component: 'API_DOCS',
    connected_tasks: [{task_id: 'connectedtask'}]
  })
};

fetch('https://api.techwriter.xyz/task', options)
  .then(response => response.json())
  .then(response => console.log(response))
  .catch(err => console.error(err));
```
```python
import requests

url = "https://api.techwriter.xyz/task"

payload = {
    "task_id": "taskname",
    "title": "tasktitle",
    "description": "taskdescription",
    "status": "OPEN",
    "component": "API_DOCS",
    "connected_tasks": [{ "task_id": "connectedtask" }]
}
headers = {
    "accept": "application/json",
    "content-type": "application/json",
    "X-API-KEY": "YOUR_API_KEY"
}

response = requests.post(url, json=payload, headers=headers)

print(response.text)
```
