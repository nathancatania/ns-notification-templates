# Coach - Justify Access to a Potentially Malicious Site
## Purpose
Coaching notification presented to the user alerting them that the requested destination is potentially malicious, but allowing them to proceed after entering a justification.

This notification is typically used when targeting the categories:
* Miscellaneous
* Newly Registered Domains
* Newly Observed Domains
* Uncategorized


## Preview
![preview](https://i.imgur.com/27pQCg1.png)

---

## Configuration
Template Name:
```
Coach - Justify Access to a Potentially Malicious Site
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
WARNING: Potentially Malicious Site Ahead!
```

Subtitle:
```
{{NS_ACTIVITY}} to {{NS_HOST}}
```

Message:
```
The site you are trying to access is considered to be high risk.

Attackers may trick you into doing something dangerous like installing software or revealing sensitive company or personal information (eg: passwords, phone numbers, credit cards).

If you understand the risks to your security, you can enter a justification reason below and proceed. This action will be audited by IT Security Operations.
```

Footer:
```
Policy: {{NS_POLICY_NAME}}
```

Justification Hint:
```
Enter a reason why you need access to this site
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
  Justification_Hint: "Enter a reason why you need access to this site"
Action Button: "useralert"
Stop_Button: "Go back"
Proceed_Button: "Proceed"
Redirect_URL_Flag: False
Redirect_URL: None
```

## Configuration Screenshot:
![config](https://i.imgur.com/8e1XTDX.png)

---

## Example Policy
* Under **Policies > Web**, create a new custom URL category that includes the categories:
  * Miscellaneous
  * Uncategorized
  * Newly Registered Domain
  * Newly Observed Domain
  * Call this custom category `Potentially Malicious Sites`.
  * Important: Make sure you include in a custom URL List as a bypass/whitelist for this custom category any company sites that might be caught in the above categories. `autodiscover.company.com` is a typical one.
* Under Policies > Real-time Protection, create a new policy.
  * For the `Destination` section, select `Category` and then the `Potentially Malicious Sites` category created above.
  * For `Activities`, select `Browse`.
  * For the `Profile and Action` section, select `User Alert` as the action and `Coach - Justify Access to a Potentially Malicious Site` as the template.

![example-policy](https://i.imgur.com/HWdgM4I.png)