---
title: "Rate Limits"
slug: "rate-limits"
excerpt: ""
hidden: false
createdAt: "Tue Jul 23 2024 17:50:10 GMT+0000 (Coordinated Universal Time)"
updatedAt: "Tue Jul 23 2024 18:26:31 GMT+0000 (Coordinated Universal Time)"
---
Given the nature of our business, security is our utmost priority when serving our clients.

To protect sensitive information and maintain a secure environment, we have implemented advanced measures within our API. These measures allow us to set rate limits on specific functions, providing enhanced control over transaction activities.

### Daily Rate Limit

We have introduced a flexible rate limit feature to [create a task](https://fireblock-cayo.readme.io/reference/addtask) or [list all task](https://fireblock-cayo.readme.io/reference/gettasks) endpoints within a 24-hour period. This empowers clients to configure rate limits for different divisions, tailoring the system to their specific needs.

The following rate limits can be set:

[block:parameters]
{
  "data": {
    "h-0": "Configuration",
    "h-1": "Details",
    "0-0": "Environment Rate Limit",
    "0-1": "Across the entire environment, only a maximum of 2000 requests can be performed per day.  \n  \n(The default limit is set to 1000 downloads per day.)",
    "1-0": "User Rate Limit",
    "1-1": "Only 100 requests can be made per day by each individual user who can access the APIs.  \n  \n(The default limit is set to 50 requests per day.)"
  },
  "cols": 2,
  "rows": 2,
  "align": [
    "left",
    "left"
  ]
}
[/block]
