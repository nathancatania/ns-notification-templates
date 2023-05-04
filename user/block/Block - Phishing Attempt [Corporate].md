# Block - Phishing Attempt [Corporate]
## Purpose
Block notification to be shown to a corporate user if a request to a known or suspected phishing site is detected.

This notification aims to educate the user on phishing, how to detect it, and what to do to seek help in the future if they are unsure.

Examples:
* [PhishTank](https://phishtank.org/phish_search.php?valid=y&active=y&Search=Search) can be used for live phishing sites (use with caution!).

## Preview
![preview](https://i.imgur.com/C4ffl1M.png)

---

## Configuration
Template Name:
```
Block - Phishing Attempt
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
Blocked. This website can steal passwords 🕵️
```

Subtitle:
```
Don't worry, you're protected, but you should be careful!
```

Message:
```
A phishing attack is when a scammer tries to trick you into revealing your password, and they will do so by tricking you into entering it into a login page that looks legitimate, but actually isn't.

This website has been detected as one of these fraudulant pages, and so the company system has blocked access to protect you.

You will only ever be asked to enter your company password by Microsoft at the website https://login.microsoftonline.com. You should NEVER sign-up for services using your corporate email without obtaining permission from IT. This is to ensure that the data that our company holds is kept safe.

If you are ever in doubt, please raise a ticket with Helpdesk and they will assist you.
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
![config](https://i.imgur.com/br442OZ.png)

---

## Example Policy

![example-policy](https://i.imgur.com/gQ9D7HL.png)