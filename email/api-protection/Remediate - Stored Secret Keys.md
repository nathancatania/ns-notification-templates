# Remediate - Stored Secret Keys
## Purpose
An email notification that can be sent to a user when it has been detected that they have saved a secret key, API key, or SSH key to a code repository or document in plaintext.

> Give a developer a secret and eventually it will end up in your source code...
> 
> -- Unknown

Note: You will need to change the `mailto` address and any other included links in the message body.

## Preview
![preview](https://i.imgur.com/VitTcci.png)

---

## Configuration
Template Name:
```
Block - Shared Company Secrets
```

Subject
```
ATTN: Secret keys were detected in a file you recently modified
```

Message:
```
Dear {{NS_USER}},

The file you created or modified within {{NS_APP}} for the following documents has been removed.

<b>Security Operations has detected that this file contained highly sensitive API keys and/or Private SSH Keys that cannot be stored outside of approved systems or in plaintext.</b>

If you believe this is a mistake, please contact <a href="mailto:helpdesk@example.com">IT Helpdesk</a>.

<b>Sharing secret keys requires explicit approval and oversight of the company CISO and CDO, as failure to safeguard such keys can result in catastrophic damage and leakage of confidential data.</b>

If you would like to understand the types of data that are acceptable/unacceptable to share, <a href="https://example.com" target="_blank">please see here</a>.

{{NS_FILE_DETAILS}}
```

## Configuration Screenshot:
![config](https://i.imgur.com/GWplsZn.png)

---

## Example Policy

![example-policy](https://i.imgur.com/WFZjTL7.png)