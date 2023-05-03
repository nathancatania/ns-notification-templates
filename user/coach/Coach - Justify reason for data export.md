# Coach - Justify reason for data export
## Purpose
Coaching notification presented to the user requiring them to provide a justification to proceed with a file download.

This notification is typically applied to a combination of high-risk data, high-risk users, unmanaged devices, and the download activity performed from a specific App Instance / Corporate Tenancy.

Examples:
* User on a personal device attempts to download a file containing PII from the Corporate OneDrive instance.


## Preview
TBA

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

Configuration Screenshot:
TBA
