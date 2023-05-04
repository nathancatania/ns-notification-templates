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
![preview](https://i.imgur.com/7CK6CyN.png)

---

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
The site you are trying to access has been detected as malicious and has been blocked.

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

## Configuration Screenshot:
![config](https://i.imgur.com/Gbqm22R.png)

---

## Example Policy
* Under **Policies > Web**, create a new custom URL category that includes all of the "_Security Risk_" categories. Call this custom category `Malicious Sites`.
* Under Policies > Real-time Protection, create a new policy.
  * For the `Destination` section, select `Category` and then the `Malicious Sites` category created above.
  * For the `Profile and Action` section, select `Block` as the action and `Block - Malicious Site` as the template.

![example-policy](https://i.imgur.com/6gbUfD6.png)
