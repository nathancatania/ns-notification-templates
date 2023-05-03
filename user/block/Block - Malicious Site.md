# Block - Malicious Site
## Purpose
Block notification to be shown to the user if a request to a malicious or high-risk site occurs.

Examples:
* shakazahn[.]ru [Malsite]
* javsheks[.]mom [Malware Distribution Point]
* saptheurbanyard[.]accounts-receivable[.]ltd [Malsite]
* www[.]monacis[.]it/ [Phishing/Fraud]

[PhishTank](https://phishtank.org/phish_search.php?valid=y&active=y&Search=Search) can also be used for live phishing sites.

## Preview
TBA

## Configuration
Template Name:
```
Block - Malicious Site
```

Logo:
```
Medium
```

Stripe Color:
```
#FF0000
```

Title:
```
Malicious Site Blocked
```

Subtitle:
```
You have been blocked from visiting {{NS_HOST}} to ensure your safety
```

Message:
```
The site you are trying to access has been detected malicious and has been blocked.

If you believe this site is safe, or if you require further information, please contact IT Helpdesk.
```

Footer:
```
Policy: {{NS_POLICY_NAME}}
```

Options:
```yaml
Logo_Size: "medium"
Stripe_Color: "#FF0000"
Localization: False
Subtitle: True
Footer_Message: True
Justification:
  Show_Justification_Option: False
  Show_Justification_Box: False
Action Button: "block"
Acknowledge_Button: "OK"
Redirect_URL_Flag: False
Redirect_URL: None
```

Preview:
TBA

Configuration Screenshot:
TBA
