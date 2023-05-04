# Block - Unacceptable Use
## Purpose
Block notification to be shown to the user if a request to a site containing adult material, or pirated content is made. Such sites are typically blocked organization wide and fall outside of the company's Acceptable Use Policy.

Examples:
* [rargb.to](https://rargb.to/) [Piracy]
* [Sportsbet](https://www.sportsbet.com.au/) [Gambling]
* [OnlyFans](https://onlyfans.com/) [Adult Content (link is to login page only and is safe to test with)]

## Preview
![preview](https://i.imgur.com/Mpd5d5q.png)

---

## Configuration
Template Name:
```
Block - Unacceptable Use
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
Prohibited Site
```

Subtitle:
```
{{NS_HOST}}
```

Message:
```
Your request has been blocked as you are trying to access a website or content that is prohibited by the company's Acceptable Use Policy.

If you believe that this is in error, please contact IT Helpdesk.
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
![config](https://i.imgur.com/p3PtROz.png)

---

## Example Policy
* Under **Policies > Web**, create a new custom URL category that includes all of the categories that you wish to block for unacceptable use, eg: Adult, P2P, Abuse, etc. Call this custom category `Unacceptable Use`.
* Under Policies > Real-time Protection, create a new policy.
  * For the `Destination` section, select `Category` and then the `Unacceptable Use` category created above.
  * For the `Profile and Action` section, select `Block` as the action and `Block - Unacceptable Use` as the template.

![example-policy](https://i.imgur.com/t3lRYED.png)