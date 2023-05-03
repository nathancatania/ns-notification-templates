# Remediate - Document Classification
## Purpose
An email notification that can be sent to a user when it has been detected that they have saved a document and either:
* Not applied any document classification labels
* Applied an incorrect document classification label

Note: You will need to change the `mailto` address and any other included links in the message body.

## Preview
![preview](https://i.imgur.com/K207RSV.png)

---

## Configuration
Template Name:
```
Remediate - Document Classification
```

Subject
```
ATTN: Your document has been classified
```

Message:
```
Dear {{NS_USER}},

<b>Security Operations has detected that the file detailed below was uploaded to {{NS_APP}} without any sensitivity labeling, or the correct sensitivity labeling, applied.</b>

<b>This has been corrected for you.</b>

As a reminder, as of August 2022, all employees must ensure that all documents created are appropriately labelled based on their intended audience. This is to ensure that sensitive company data and customer data remains safe.

If you are still unsure as to how to classify and label documents correctly, we encourage you to chat to your manager, reach out to <a href="mailto:helpdesk@lightwave.cloud">IT Helpdesk</a>, or <a href="https://example.com" target="_blank">watch a short video here</a>.

Thank you for your understanding. Together, we can help keep our company secure.

{{NS_FILE_DETAILS}}
```

## Configuration Screenshot:
![config](https://i.imgur.com/49t9GRU.png)
