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
