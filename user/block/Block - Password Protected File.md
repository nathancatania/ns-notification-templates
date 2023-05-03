# Block - Password Protected File
## Purpose
Block notification to be shown when a user attempts to upload/download a password protected (or encrypted) file.

Note: You should change `OneDrive` in the subtitle to reference the company's sanctioned file sharing service if different, eg: GDrive, Dropbox.

## Preview
![preview](https://i.imgur.com/3AMXfQC.png)

## Configuration
Template Name:
```
Block - Password Protected File
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
Blocked. This file is locked and can't be shared.
```

Subtitle:
```
Did you know that data can be shared securely using OneDrive?
```

Message:
```
It looks like you are trying to transfer a file that is password protected or encrypted.

These types of files commonly contain malware and as such have been blocked.

If you need to securely share a file with another person, please use the company OneDrive and Sharepoint accounts.
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
![config](https://i.imgur.com/zqoalHj.png)
