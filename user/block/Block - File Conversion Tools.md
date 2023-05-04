# Block - File Conversion Tools
## Purpose
Block notification to be shown when a user navigates to a site designed to convert or modify a document or file; such as PDF or image compression tools or tools designed to convert from one format to another (eg: DOCX to PDF, PNG to JPG, etc).

Examples:
* [I Love PDF](https://www.ilovepdf.com/compress_pdf) [PDF Compression]
* [I Love PDF](https://www.ilovepdf.com/pdf_to_word) [PDF to Word Conversion]
* [SmallPDF](https://smallpdf.com/compress-pdf) [Multiple PDF tools]
* [Png2Jpg](https://png2jpg.com/) [PNG to JPG Image Converter]

## Preview
![preview](https://i.imgur.com/mjgb7Kt.png)

---

## Configuration
Template Name:
```
Block - File Conversion Tools
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
Blocked. Company data isn't safe with this tool!
```

Subtitle:
```

```

Message:
```
Tools like {{NS_APP}} can store and retain ownership of sensitive Company data for indefinite periods of time, so you're not able to use it for any type of company data.

This is to ensure our company and customer data is kept safe.
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
Subtitle: False
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
![config](https://i.imgur.com/hz8N9Xy.png)

---

## Example Policy
* There are two different policies where this template could be useful:
   * Completely blocking unsanctioned File Conversion tools (ILovePDF, SmallPDF, etc), OR
   * Allowing the use of these tools, but blocking company data from being uploaded there.
* Under Policies > Real-time Protection, create a new policy.
  * For the `Destination` section, select `Category` and then the `File Converter`.
  * Click `Add Criteria & Constraints` and select `App Tag`. Select `Unsanctioned` from the list. This will only target apps that are not sanctioned by the company.
  * For Activities:
     * If you want to completely hard block these sites, select `Browse` as an activity.
     * If you want to allow these use of these sites but block company data being uploaded to them, select `Upload` as an activity.
  * For the `Profile and Action` section, select `Block` as an action, and select the `Block - File Conversion Tools` template.
  * If you want to hard block these sites, then you are finished. If you want to allow them, but block company data, select `Add Profile` then `DLP Profile`, then select the sensitive content to match on.

Hard block:

![example-policy](https://i.imgur.com/drNiPc9.png)

Block only on upload of sensitive data:

![example-policy2](https://i.imgur.com/D1FSRn7.png)