# Block - Upload to High Risk Cloud Storage
## Purpose
Block notification to be shown to the user if an attempt to upload a file to unsanctioned or high risk (low CCL) cloud storage is attempted.

Examples:
* [WeTransfer](https://wetransfer.com/)
* [MediaFire](https://www.mediafire.com/)
* [Send Anywhere](https://send-anywhere.com/)

Note: You should change `OneDrive` and `Sharepoint` in the subtitle and message body to reference the company's sanctioned file sharing service if different, eg: GDrive, Dropbox.

## Preview
TBA

## Configuration
Template Name:
```
Block - Upload to High Risk Cloud Storage
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
Hold Up! Files Cannot be Uploaded Here
```

Subtitle:
```
Did you know that data can be shared securely using OneDrive?
```

Message:
```
You are trying to upload data to the cloud storage service {{NS_APP}} that is considered unsafe by Security Operations. Please use Microsoft OneDrive or Sharepoint for all of your file sharing needs.

If you believe you should have access to this application, please contact IT Helpdesk.
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
