# Magento 2 Google Consent Mode v2 Extension

The **Google Consent Mode v2** extension helps Magento 2 store owners comply with privacy regulations and manage cookie consent for analytics and advertising purposes. It enables users to opt in or opt out of different types of cookies and ensures compliance with privacy laws such as GDPR.

## How It Works

Upon the user's first visit to your site, a cookie consent banner is displayed. This allows users to set their preferences for cookie usage, including groups such as marketing, analytics, and advertising. The default consent state is sent to Google via the data layer, and users can update their preferences anytime via the cookie settings icon. This ensures full compliance and flexibility for users regarding their data privacy.

## Key Features

- **Lightweight Cookie Banner**: Optimized for both desktop and mobile devices, with minimal design to ensure a superior user experience.
- **Choose Cookie Preferences**: Users can set preferences for individual cookie categories and later update them using a cookie settings icon.
- **Customize Design & Content**: Customize the banner’s colors, button labels, and icon styles to match your site's branding.
- **Manage Cookie Groups**: Define cookie groups (e.g., marketing, analytics, advertisement) for users to accept or deny.
- **Custom Consent Types**: Add custom consent parameters and modify the default state for different consent types.
- **Seamless Google Tags Integration**: Real-time integration with Google Tags, sending consent states during page load and updating via the data layer.

### 1. **Lightweight Cookie Banner**
The extension displays a lightweight cookie consent banner that is optimized for both desktop and mobile devices. The banner features a minimal design that enhances the user experience while providing essential cookie options like accepting or rejecting cookies. 

### 2. **Choose Cookie Preferences**
The extension allows users to control their cookie preferences for multiple groups such as:
- Marketing
- Analytics
- Advertisement

Users can easily choose which cookie groups to accept or reject. They can also update their preferences at any time using the cookie settings icon that you can configure to display on your website.

### 3. **Customize Design & Content**
You can fully customize the cookie consent banner to match your site’s aesthetic. The following elements are customizable:
- **Background Color**: Customize the background color to fit your theme.
- **Button Background & Text Colors**: Change the button background and text colors to suit your site’s design.
- **Button Label**: Modify the text displayed on the buttons (e.g., "Accept" or "Decline").
- **Preferences Icon Color**: Adjust the icon color to match your brand.

### 4. **Manage Cookie Groups**
Define multiple cookie groups (e.g., marketing, analytics, advertisement) and display them to users on the cookie preferences screen. Users will be able to accept or reject cookies based on the group, ensuring better control over their privacy preferences.

### 5. **Custom Consent Types**
The extension includes default parameters for the following Google consent types:
- **ad_storage**
- **analytics_storage**
- **ad_user_data**
- **ad_personalization**

You can also add custom parameters and modify the default consent state for each, giving you flexibility in managing user consent for different types of data.

### 6. **Seamless Google Tags Integration**
The extension integrates seamlessly with Google Tags. When the page loads, the user's consent state is sent to Google, and any changes made by the user are updated via the data layer in real-time. You can also configure the extension to remember the user's preferences for a specified number of days, reducing the need for repeated consent requests.


## Extension Installation:

1. **Download and Extract**:
   - Download the extension’s zip file from Meetanshi, then extract it to your Magento root directory.

2. **Run Setup Commands**:
   - Log in to your SSH terminal and run the following commands:
     ```bash
     php bin/magento setup:upgrade
     ```
   - For Magento version 2.0.x to 2.1.x:
     ```bash
     php bin/magento setup:static-content:deploy
     ```
   - For Magento version 2.2.x and above:
     ```bash
     php bin/magento setup:static-content:deploy -f
     ```

3. **Clear Cache**:
   - Complete the installation by flushing the cache:
     ```bash
     php bin/magento cache:flush



## How to Set Up Magento 2 Google Consent Mode v2 Extension

### Step 1: Head to the Magento Admin Panel

To begin configuring the **Google Consent Mode v2** extension, log into your **Magento Admin Panel**.

1. Open your web browser and go to your Magento Admin URL.
2. Enter your credentials to log in.

Once logged in, navigate to the **Stores** menu in the left sidebar.

### Step 2: Click Configuration

In the **Stores** menu, select **Configuration** under the **Settings** section. This will open the configuration page for your store settings.

### Step 3: Enable & Customize the Cookie Banner

Next, go to **Meetanshi > Cookie Consent V2** from the Configuration menu to enable the extension.

**Enable Google Cookie Consent**:
   - Set the option to **Yes** to enable the Google Cookie Consent functionality for your store.
   - Once enabled, the **Google Cookie Consent banner** will appear on your website for users to interact with.

Navigate to: Stores > Configuration > Meetanshi > Cookie Consent V2

### Step 4: Customize Cookie Consent Banner

Once the extension is installed and enabled, you can customize the cookie consent banner according to your store's theme and branding. Navigate to the **Cookie Consent Settings** under **Meetanshi > Cookie Consent V2** in the **Magento Admin Panel** to access the customization options.

- **Show Cookie Preferences Button**: Enable or disable the button that allows users to change their cookie preferences after their initial selection.
- **Button Background Color**: Set the background color of the button to match your store's color scheme.
- **Button Text Color**: Customize the button text color to ensure it aligns with the overall design.

**Example of Customized Cookie Banner:**
The cookie consent banner will now appear on your website, matching the custom settings you’ve applied.

![Example of Customized Cookie Banner](https://github.com/user-attachments/assets/0330ae71-b43b-40eb-bace-b19d09fa76ef)

---

### Step 5: Customize Cookie Notice

You can also modify the content of the cookie notice that is displayed when users first visit your store. The cookie notice informs users about your cookie usage and provides them with options to accept or manage their preferences.

*Cookie Notice Settings:*
- **Notification Text**: Enter a brief message that will be shown in the cookie notice.
- **More Information Link**: Add a link to your website’s cookie policy or privacy policy page for more details on the cookies used.
- **Consent Restriction Timeline**: Set the number of days for which the user’s consent preferences will be stored. After the set period, the cookie notice will be displayed again.

*Example of Cookie Notice Customization:*
The cookie notice will be displayed with the following configuration.

![Example of Cookie Notice Customization](https://github.com/user-attachments/assets/af62fd83-9f26-49a8-850f-67992bbce13f)

---

### Step 6: Edit or Create a New Cookie Group
- Go to **Cookie Consent V2 > Manage Cookie Groups** in the Magento Admin Panel.
- Here, you can see all the existing cookie groups. To add a new group, click the **Add a New Group** button.
- Configure the following settings for each cookie group:
  - **Enabled**: Turn the group on or off.
  - **Set as Essential**: Mark the group as essential if users cannot disable it.
  - **Cookie Group Code**: Provide a unique identifier for the group.
  - **Cookie Group Name**: Name the group that will appear on the cookie preferences pop-up.
  - **Description**: Optionally, add a description for the cookie group.
  - **Sort Order**: Determine the display order of the groups in the preferences pop-up.

*Example of Cookie Group Configuration:*
This section allows you to manage and organize cookie groups efficiently.

![Example of Cookie Group Configuration](https://github.com/user-attachments/assets/911a10b0-29d2-438b-b4ce-3b7e81173c7b)

---

### Step 7: Assign Consent Types to Cookie Groups
Each cookie group can have multiple **consent parameters** associated with it. These consent parameters define which cookies are used for specific purposes (e.g., advertising, analytics).

- Go to **Cookie Consent V2 > Manage Consent Parameters** in the Magento Admin Panel.
- Here, you can find existing consent parameters or create new ones by clicking the **Add a New Consent Parameter** button.
- For each consent parameter, configure the following:
  - **Parameter Code**: Define the consent code that will be sent to Google Tag.
  - **Default Status**: Set the default status of the consent type (either **granted** or **denied**).
  - **Cookie Group**: Assign the consent parameter to a cookie group.

Once configured, click **Save Parameter** to apply the changes.

![Save Parameter](https://github.com/user-attachments/assets/84438fc8-26a1-414f-8bc0-bf4665e55cc3)

---

## Step 8: Set Cookie Preferences on the Front-End

Once the extension is properly configured, the **cookie consent notice** will be active on your website's front end.

- On a user’s first visit, the default consent preferences will be sent to Google tags and the consent notice will be shown.
- After users set their preferences, their choices will be stored and sent to Google tags via the data layer.
- Users can either accept all cookies, only essential cookies or select custom preferences.

If you enable the **Cookie Preferences Button**, users can modify their preferences anytime.

Use the **Google Tag Assistant** tool to debug the consent states in real time. You can check how consent states are passed to Google tags.

Here’s an example of how the cookie preferences popup appears on the front end of the website.

![example of how the cookie preferences popup appears on the front end of the website](https://github.com/user-attachments/assets/fdbb6e29-cabc-4681-840d-b2c5f5a87a6f)

---

## Step 9: View Cookie Consent Logs

To analyze user consent preferences, Magento 2 provides a log of user consent choices under the **Cookie Consent V2 > Cookie Consent Logs** section.

- This feature gives store owners insights into the cookies accepted or denied by users.
- You can view the **date** of consent and track the **preferences** for better compliance with privacy regulations.

#### Example of Cookie Consent Logs:
This grid allows you to view detailed logs of user consent, helping ensure that you are compliant with regulations.

![ Example of Cookie Consent Logs](https://github.com/user-attachments/assets/2202fdef-0025-4a00-b212-aa7e30f13941)

---

By following these steps, you can ensure that your Magento store complies with privacy regulations like GDPR and provides users with control over their cookie preferences.


## Download our [Magento 2 Google Consent Mode v2 Extension](https://meetanshi.com/magento-2-google-consent-mode.html)
