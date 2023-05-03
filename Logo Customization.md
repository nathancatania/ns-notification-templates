# Logo Customization

Leveraging different styles of a company logo in different notification templates can enhance readability and comprehension. This document will cover quick methods to customize a company logo in different styles for inclusion in different notifications.

Eg: Red logo for block notifications, Orange/Yellow logo for coaching/warning notifications, and a standard logo for everything else.

Block / Red Logo:

![example-red-block](https://i.imgur.com/LORNmsJ.png)


Coach / Orange Logo:

![example-orange-coach](https://i.imgur.com/fXCuNpB.png)


![logo-comparison](https://i.imgur.com/YweiYNI.jpg)

---
# Process
## 1. Obtain a company logo with transparent background (PNG)
Google Images is your friend for this, eg: `Netskope logo transparent`.

If you can't find a transparent logo, you can try using an online tool like [remove.bg](https://www.remove.bg/) to remove the background for you.

## 2. Use Photopea to alter the logo color
Photopea is a Photoshop clone accessible for free in the web browser.

1. Go to [https://www.photopea.com/](https://www.photopea.com/) and click File > Open, and select your logo.

2. Right-click on the layer called "Background" on the right-hand side (see the image below), and select **Blending Options**.
![blending-options](https://i.imgur.com/0dv2WgN.png)

3. In the _Blending Options_ window, check the **Color Overlay** option, and set the color to #FF0000 (red).
![color-overlay-red](https://i.imgur.com/TRoR6Jz.png)

4. Close the _Blending Options_ window and save your new image as a PNG by going to **File > Export As > PNG**
![save-png](https://i.imgur.com/LrCFtXW.png)

5. Ensure that you call the file something descriptive like `logo-red.png`. IMPORTANT: The filesize MUST be under 1MB. Adjust the dimensions of the image to reduce the filesize if needed. If the chain/link button between the width and height text boxes is selected, your aspect ratio will be maintained.
![save-as-menu](https://i.imgur.com/LrCFtXW.png)

6. Repeat steps 2-5 again, but this time, set the color to #FFA200 (orange).
![color-overlay-orange](https://i.imgur.com/DjLhUWz.png)

## 3. Upload the logos to the Netskope Admin Portal

### Default Logo
The standard colored company logo should be uploaded under **Settings > Tools > Templates > Edit**. This logo is used by default for ALL templates across the Netskope platform.

![default-logo-upload](https://i.imgur.com/PIcLM9L.png)

### Additional Logos
In the main admin console, navigate to **Policy > Custom Image** (located underneath the _User Notification_ and _Email Notification_ menu options under the _Templates_ sub-heading).

Select the **New Image** button and upload both the red and orange variants of the logo you created.

![custom-logo-upload](https://i.imgur.com/vEhGUtv.png)

## 4. Specify a specific logo to use
When creating a User Notification Template, you can specify the exact logo to use by selecting it from the dropdown menu under the `Logo` heading. Set the stripe color to match the color of the logo:
* `#FF0000` for the red logo & block action.
* `#FFA200` for the orange logo & coach/user-alert action.

To use the default logo, set the dropdown to the "Company Logo" option.

![logo-selection](https://i.imgur.com/lWMKVdM.png)
