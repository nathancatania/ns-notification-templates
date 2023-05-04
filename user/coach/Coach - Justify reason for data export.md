# Coach - Justify reason for data export
## Purpose
Coaching notification presented to the user requiring them to provide a justification to proceed with a file download.

This notification is typically applied to a combination of high-risk data, high-risk users, unmanaged devices, and the download activity performed from a specific App Instance / Corporate Tenancy.

Examples:
* User on a personal device attempts to download a file containing PII from the Corporate OneDrive instance.


## Preview
![preview](https://i.imgur.com/ksEs0yp.png)

---

## Configuration
Template Name:
```
Coach - Justify reason for data export
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
You have privileged permission to export data from {{NS_APP}
```

Subtitle:
```

```

Message:
```
This data must only be exported for specific internal use and must stored in compliance with company security policy. Failure to comply with company policy, including the safeguard of all sensitive data, may result in disciplinary action - up to and including termination.

You must justify your intended use of this data in order to proceed. This action has been recorded and your response will be audited.
```

Footer:
```
Policy: {{NS_POLICY_NAME}}
```

Justification Hint:
```
Justify your need for this data
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
Subtitle: False
Footer_Message: True
Justification:
  Show_Justification_Option: False
  Show_Justification_Box: True
  Input_Optional_Stop_Button: True
  Input_Optional_Proceed_Button: False
  Justification_Hint: "Justify your need for this data"
Action Button: "useralert"
Stop_Button: "Go back"
Proceed_Button: "Proceed"
Redirect_URL_Flag: False
Redirect_URL: None
```

## Configuration Screenshot:
![config](https://i.imgur.com/ZGY5eWL.png)

---

## Example Policy
* Under Policies > Real-time Protection, create a new policy.
  * For the `Destination` section, select `Category`, `App Instance`, `Cloud App`, or `Application`, and then select the category, instance, or app definition that you wish to restrict data exporting from.
  * For `Activities`, select `Download`.
  * For the `Profile and Action` section, select `User Alert` as the action and `Coach - Justify reason for data export` as the template.
  * Pro-tip: Apply a DLP Profile to this rule so that only sensitive data being exported is targeted.
  * Pro-tip #2: You can target this policy at specific AD Groups or employees above a specific risk level under the `Source` section.

![example-policy](https://i.imgur.com/xGtPcRO.png)