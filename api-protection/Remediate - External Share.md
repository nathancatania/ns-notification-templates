# Remediate - Remove External Share
## Purpose
An email notification that can be sent to a user when it has been detected that they have shared a sensitive document externally.

Note: You will need to change the `mailto` address and any other included links in the message body.

## Preview
![preview](https://i.imgur.com/fA67S6y.png)

---

## Configuration
Template Name:
```
Remediate - External Share
```

Subject
```
ATTN: Your External Share has been Removed
```

Message:
```
Dear {{NS_USER}},

The external share link you created within {{NS_APP}} for the following documents has been removed.

<b>Security Operations has detected that this file contains highly sensitive company information that cannot be shared outside of the company.</b>

If you believe this is a mistake, please contact <a href="mailto:helpdesk@example.com">IT Helpdesk</a>.

<b>Sharing files externally to our company can be dangerous and unintentionally result in company or customer data being exposed. Please be careful when sharing data with people outside of the organization in the future.</b>

If you would like to understand the types of data that are acceptable/unacceptable to share, <a href="https://example.com" target="_blank">please see here</a>.

{{NS_FILE_DETAILS}}
```

## Configuration Screenshot:
![config](https://i.imgur.com/T7kbBGm.png)
