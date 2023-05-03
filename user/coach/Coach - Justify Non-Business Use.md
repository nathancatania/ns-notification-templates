# Coach - Justify Non-Business Use
## Purpose
Coaching notification presented to the user alerting them that the requested destination falls outside of acceptable or business use, but allows them to proceed WITH justification.

Examples:
* [Sportsbet](https://www.sportsbet.com.au/) [Gambling]


## Preview
![preview](https://i.imgur.com/TjGaP4o.png)

---

## Configuration
Template Name:
```
Coach - Justify Non-Business Use
```

Logo:
```
Medium
```

Stripe Color:
```
#FFA200
```

Title:
```
Heads up! This website falls outside of Acceptable Use!
```

Subtitle:
```
{{NS_ACTIVITY}} to {{NS_HOST}}
```

Message:
```
The site {{NS_HOST}} falls outside acceptable use or business use. You are allowed to proceed, but please enter a reason as to why you need access to this site below.
```

Footer:
```
Policy: {{NS_POLICY_NAME}}
```

Justification Hint:
```

```

Stop Button:
```
Go back
```

Proceed Button:
```
Proceed
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
  Show_Justification_Box: True
  Input_Optional_Stop_Button: True
  Input_Optional_Proceed_Button: False
  Justification_Hint: ""
Action Button: "useralert"
Stop_Button: "Go back"
Proceed_Button: "Proceed"
Redirect_URL_Flag: False
Redirect_URL: None
```

## Configuration Screenshot:
![config](https://i.imgur.com/la4axKc.png)
