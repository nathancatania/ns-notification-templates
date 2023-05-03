# Block - Specific Action
## Purpose
A generic block notification to be shown to the user if a specific action or activity they are performing is blocked.

Example:
* Browse to Dropbox is allowed, but Upload is blocked.

## Preview
![preview](https://i.imgur.com/6QzEnAP.png)

---

## Configuration
Template Name:
```
Block - Specific Action
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
This action is disabled
```

Message:
```
For security reasons, the ability to {{NS_ACTIVITY}} within {{NS_APP}} has been disabled. This assists us in securing sensitive company information.

You can safely close this message.

For additional information, or if you believe you require access to this action, please contact IT Helpdesk.
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
![config](https://i.imgur.com/O0QVrlN.png)
