---
title: "Authentication"
slug: "authentication"
excerpt: "🔑 Authenticate using our API key"
hidden: false
createdAt: "Tue Jul 23 2024 17:18:13 GMT+0000 (Coordinated Universal Time)"
updatedAt: "Tue Jul 23 2024 18:21:32 GMT+0000 (Coordinated Universal Time)"
---
Authentication enables you to manage all aspects of user identity, such as accessing API endpoints. We use basic authentication using the API key. 

All API requests must be made over HTTPS, and API requests without authentication will fail.

### How to Get API Key

[block:html]
{
  "html": "<style>\n\t.api_key_instruct_ban {\n\t\tbackground: #2C2B3D;\n\t\tborder-radius: 12px;\n\t\t-webkit-border-radius: 12px;\n\t\tdisplay: flex;\n\t\tflex-wrap: wrap;\n\t\tpadding: 33px;\n\t}\n\n\t.api_key_instruct_ban_lft h3 {\n\t\tfont-size: 24px;\n    line-height: 1.3;\n    color: white;\n\t\tletter-spacing: -0.03em;\n    font-weight: 700;\n\t\tfont-family: 'Inter', sans-serif;\n\t\tmargin-bottom: 7px;\n\t\tmargin-top: 0px;\n\t}\n\n\t.api_key_instruct_ban_lft h3:last-child {\n\t\tmargin-bottom: 0;\n\t}\n\n\t.api_key_instruct_ban_lft p {\n\t\tfont-size: 14px;\n\t\tline-height: 1.3;\n\t\tcolor: white;\n\t\tfont-family: 'Inter', sans-serif;\n\t\tfont-weight: 400;\n\t}\n  \n  .api_key_instruct_ban_lft {\n  \tflex-basis: 80%;\n   \tmax-width: 80%;\n  \tpadding-right: 15px;\n                                }\n  \n  .api_key_instruct_ban_rtt {\n     flex-basis: 20%;\n     max-width: 20%;\n     padding-left: 15px;\n     align-self: center;\n                                }\n  \n\t.gt_startd_vbtn {\n\t\tdisplay: inline-block;\n    white-space: nowrap;\n\t\tcolor: #FFFFFF !important;\n\t\tbackground: linear-gradient(126.33deg, #3D1C8C 5.38%, #6C48C3 108.32%);\n\t\tborder-radius: 6px;\n\t\tfont-size: 16px;\n\t\tline-height: 1.3;\n\t\tfont-weight: 600;\n\t\tfont-family: 'Inter', sans-serif;\n    text-decoration: none !important;\n\t\tpadding: 10px 16px;\n\n\t}\n\n\t.gt_startd_vbtn:hover {\n\t\tbackground: #211B4E;\n\t\tcolor: #fff;\n\t}\n  \n  @media only screen and (max-width:768px) {\n    .api_key_instruct_ban {\n    \tdisplay: block;\n    }\n    \n    .api_key_instruct_ban_rtt {\n    \tpadding-left: 0;\n    }\n  }\n</style>\n\n<!-- dont_have_api_sec_start -->\n<div class=\"api_key_instruct_ban\">\n\t<div class=\"api_key_instruct_ban_lft\">\n\t\t<h3>Need a Free API key?</h3>\n\t\t\t<p>Enjoy Scalable Task Management Solutions with our APIs.</p>\n\t</div>\n\n\t<div class=\"api_key_instruct_ban_rtt\">\n\t\t<a href=\"fireblocks.com" class=\"gt_startd_vbtn\">Get Started</a>\n\t</div>\n</div>\n\n<!-- dont_have_api_sec_end -->"
}
[/block]


<br />

### API Key Details

Authentication to the API is performed via HTTP Basic Auth. To authenticate with the API, you must provide the API Key in the header, as shown below.

```curl Authentication Header
'x-api-key: <Your_API_Key>'
```

For example, when you want to get all the tasks, you will use the `GET - List all tasks` endpoint. In this scenario, you can send an API request by adding your API Key in the Authentication header as shown below. Please be sure to change the `YOUR_API_KEY`.

```curl Sample
curl --request GET \
     --url https://api.techwriter.xyz/tasks \
     --header 'X-API-KEY: YOUR_API_KEY' \
     --header 'accept: application/json'
```

> 🚧 Alert!
> 
> Your API keys carry many concessions, so keep them safe! Do not share your secret API keys on publicly accessible sites.
