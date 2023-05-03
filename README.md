# Netskope Notification Templates
This repository contains templates for different user popups and email notifications, for both block and coachingactions, for a variety of different scenarios.

> Disclaimer: Any thoughts or opinions in this repository are my own and do not reflect those of Netskope. I am a Netskope SE who put this together in his own time to assist Netskope customers and employees. Please submit an [issue](https://github.com/nathancatania/ns-notification-templates/issues) to correct any mistakes or inaccuracies, or a PR to contribute.

### Sample User Notification Popup:
![sample-user-notification](https://i.imgur.com/fXCuNpB.png)


### Sample Email Coaching Notification:
![sample-email-notification](https://i.imgur.com/5PHIY3b.png)

---
# Using these Templates
1. From the repository, select either the **`user`** or **`email`** folders. These contain templates for User Notifications and Email Notifications respectively.
2. Templates are categorized as either **`block`** or **`coach`**:
  * Block templates represent a denied action. For User Notifications, the user cannot proceed. For Email Notifications, the user is warned that an action performed was reverted or denied.
  * Coach templates represent a warning. For User Notifications, the user can proceed past the warning (optionally requiring justification) to continue. For Email notifications, the user is warned that an action performed was remediated or fixed to be inline with company policy.
3. Open a template and copy/paste the relevant fields into the Add Template window inside the relevant area of the Netskope admin portal (see below).

---

# Create a new Template
From the Netskope admin UI, navigate to **Policies** and then under the _Templates_ subheading, select either **User Notifications** or **Email Notifications**. You may need to scroll down the menu to find these options as they are at the bottom.

![1](https://i.imgur.com/TYuqv8D.png)

## User Notifications
User Notifications are the messages that Netskope will pop-up and front to the user in real-time as they interact with the internet.

User Notifications can be configured to be hard blocking (ie: the request is blocked and the user cannot proceed), or coaching (ie: the request is stopped and the user is prompted to proceed or go back).

User Notifications can be customized on a per-policy basis, meaning that you can create and tailor different messages to users for each individual policy. This provides a much better end-user experience than traditional universal block pages.

There are 4 sub-types of User Notifications you can create; each of which is used for a different feature of the Netskope platform:
| Type             | Description                                                                                                                                                                                          |
|------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Cloud Apps & Web | Most notifications you create will be of this type. These notifications can be selected in your real-time protection policies, which are triggered as user's interact with the internet.             |
| Private Apps     | These notifications can be selected when creating a policy for Netskope Private Access (NPA) and are triggered as users interact with internal company apps that Netskope facilitates access to.     |
| Endpoint Device  | These notifications are used for Endpoint DLP capability and are triggered if the user attempts to perform a prohibited action on their device (eg: plug in a USB drive, or print a sensitive file). |
| Endpoint Content | These notifications are also used for Endpoint DLP capability and are triggered if a user attempts to move sensitive data locally on the device (eg: copy to USB, AirDrop, etc).                     |

Note that depending on your Netskope subscription, not all of the above notification types will be visible to you.

![user-notification-screen](https://i.imgur.com/NIAgc55.png)

## Email Notifications
Email Notifications are messages that Netskope can send to specified parties, whether that be the user or admin, under certain conditions.

Email Notifications are not hard blocking, and should be used to either coach the user on appropriate actions, or alert administrators that a specific policy has been triggered.

Email Notifications can be triggered on a per-policy basis, and can be triggered in addition to a User Notification (see above).

There are two sub-types of Email Notifications you can create:
| Type                 | Description                                                                                                                                                                                                                                                                                                                                                                                                                              |
|----------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Real-Time Protection | These notifications can be selected in your real-time protection policies, which are triggered as your user's interact with the internet. Typically you will use these to alert someone other than the user that an incident or policy trigger has occurred.                                                                                                                                                                             |
| API Data Protection  | These notifications are can be selected in your API protection policies, which are triggered as your user's interact with your company data within managed SaaS apps (eg: OneDrive, Sharepoint, etc). These are typically used to coach the user when a remediation action occurs (eg: The user shares some data externally which isn't allowed. Netskope remediates the public share and triggers a coaching notification to the user). |

Note that depending on your Netskope subscription, not all of the above notification types will be visible to you.

![email-notification-screen](https://i.imgur.com/YFaKfD8.png)

---
# Custom Logos
## Add a Default Logo
To begin, you should ensure that the you have uploaded a company logo under **Settings > Tools > Templates > Edit**. This logo is used by default for ALL templates across the Netskope platform.

![set-default-logo](https://i.imgur.com/PIcLM9L.png)

## Add Additional Logos/Images
The logo/image used can be set on a per-notification basis. For example, it can be good practice to use a red styled company logo for events that are hard blocked (eg: malware), and an orange styled company logo for user alerts and coaching prompts that the user can opt to proceed through.

Additional Logos and imagry can be uploaded under **Policy > Custom Image** (located underneath the _User Notification_ and _Email Notification_ menu options under the _Templates_ sub-heading).

For more information on how to quickly customize a logo in different colors, see [Logo Customization](https://github.com/nathancatania/ns-notification-templates/blob/402d66b7f079a7d8971a64833f82fb085bae3e60/Logo%20Customization.md).

![set-additional-logos](https://i.imgur.com/vEhGUtv.png)

