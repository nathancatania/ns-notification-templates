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

---

## Example Policy
* First, create a File Profile that specifically looks for password protected or encrypted files:
   * Under Policies > File, select `New File Profile`.
   * On the left side of the window, select `Password/Encrypted` and **CHECK** the following options:
      * `File is password-protected`
      * `File is protected by AIP/RMS`
   * Click `Next`, give the profile a name (eg: `Password Protected File Profile`), and click save.
   * Make sure that you click the `Apply Changes` button.
* Next, create a new DLP Profile that only targets your Password Protected File profile.
   * Under Policies > DLP, select `New Profile`.
   * On the first screen, select the `Password Protected File Profile` you created above.
   * Click `Next`, then `Next` again to skip to the end. Give the profile a name, eg: `Protected Files` and click `Save`.
* Next, create a new policy to tie everything together. Go to Policies > Real-time Protection and select `New Policy`.
   * For the `Destination` section, select `Category` and then select every category (to target the entire internet) or specific categories like `Cloud Storage` and `Webmail`.
   * For `Activities`, select `Upload`.
   * For the `Profile and Action` section, select `Block` as an action, and select the `Block - Password Protected File` template.
   * Select `Add Profile` then `DLP Profile`, then select the `Protected Files` DLP Profile you created above.


![example-policy](https://i.imgur.com/2FAqPzO.png)