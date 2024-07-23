---
title: "Error Codes"
slug: "error-codes"
excerpt: "🛠️ Learn how to handle common errors."
hidden: false
createdAt: "Tue Jul 23 2024 17:13:28 GMT+0000 (Coordinated Universal Time)"
updatedAt: "Tue Jul 23 2024 17:13:35 GMT+0000 (Coordinated Universal Time)"
---
We dedicated this article to helping you solve errors in our API. Please review the error description below, or go straight to the causes and suggestions.

## Response Codes

We use the standard HTTP status code. Please see the table below for further information:

| Status Code                   | Description                             |
| :---------------------------- | :-------------------------------------- |
| 200 - ✅ Success               | Request successfully processed/created. |
| 400 - ❌ Bad Request           | The request was unacceptable.           |
| 401 - ❌ Unauthenticated       | Your API key is invalid.                |
| 404 - ❌ Not Found             | The requested resource doesn't exist.   |
| 500 - ❌ Internal Server Error | Something went wrong on our side.       |

## Error Troubleshoots

Here is our recommendation for handling errors:

### 400 - Bad Request

💣 **Cause**: This error occurs because of invalid syntax or missing a required parameter.  
🛠 **Solution**: Recheck the request that you input. Make sure it has followed the requirements.

### 401 - Unauthenticated

💣 **Cause**: This error occurs when you put in an invalid API key.  
🛠 **Solution**: Double-check the API key and make sure you input the correct one.

### 404 - Not Found

💣 **Cause**: This error occurs because you provided the wrong URL or the ID you requested is not associated with your account.  
🛠 **Solution**: Use the correct URL (check for typos and our API documentation carefully).

### 500 - Internal Server Error

💣 **Cause**: This error occurs when our system has encountered an internal system error.  
🛠 **Solution**: You can retry later, or please get in touch with our support if you keep getting this error.
