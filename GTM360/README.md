# Set up and report performance measurement for the WoVG with Google Tag Manager
Use these instructions to comply with the mandatory standard for the Victorian government for adding the Google Analytics tracking code to your website.

This process is **NOT** for Single Digital Presence sites.

## Configure Google Tag Manager (GTM)
Use Google Tag Manager to manage tags (such as measurement and marketing optimization JavaScript tags) on your site. Without editing your site code, you use the GTM user interface to add and update Google Ads, Google Analytics, Floodlight, and non-Google tags. This reduces errors and allows you to deploy tags on your site quickly.
Google Tag Manager replaces all your measurement and marketing tags with a single, asynchronously loading tag—so your tags can fire faster without getting in each other’s way.

### Google Tag Manager Account Creation
If your agency or department doesn’t have a GTM account, follow [these instructions from Google](https://support.google.com/tagmanager/answer/6103696?hl=en).

#### GTM Naming Convention
This is the WoVG naming convention for Google Tag Manager containers.

Use your primary domain name, don’t include the www from the hostname.

For the Department of Premier and Cabinet, this would be:
* **dpc.vic.gov.au**

#### GTM Installation
Then add the container to every page of your site using this [Quick Start Guide for Google Tag Manager for Web Tracking](https://developers.google.com/tag-manager/quickstart)

#### GTM Configuration
Once you have your container installed it is time to configure it.
You will need to edit the constants that give this container its flexibility. 
Open the folder, #1 - GTM  - Configuration Variables
Edit the following constants as needed.
1. Const - Hostname - For Website - WOVG - Config
    * Please set your host name in the value field, without "www." e.g. my-domain.vic.gov.au
2. Const - Hotjar Site ID - WOVG - Config
    * Please use your Hotjar Site ID e.g. 1234567. If you do not have a Hotjar Site ID / Account then leave the value as "0"
4. Const - Page Not Found - Text - WOVG - Config
    * Please update with plain text, the title or part of the title when your page returns a 404 not found. e.g. not found, 404, etc.
5. Const - UA - ID - Prod - WOVG - Config
    * Your Google Analytics Property ID e.g. UA-xxxxxxxxx-x 
6. Const - UA - ID - Test - WOVG - Config
    * Your Testing/QA Google Analytics Property ID e.g. UA-xxxxxxxxx-x 
    * This is a dedicated Google Analytics Property for test data, it is used so that your UAT or test environments don't send data into your live Google Analytics reports.
Note for constants 5 & 6:
https://support.google.com/tagmanager/answer/9207621#ga_id

Then open, #2 - GTM - Configuration Advanced, and edit as needed:
1. Click - Link - Button - CTA - WOVG - Config
2. Click - Link - External - WOVG - Config
3. Click - Link - Footer - WOVG - Config
4. Click - Link - Header - Top - Nav - Home - WOVG - Config
5. Click - Link - Header - Top - Nav - WOVG - Config
6. Const - Body Content - CSS - WOVG - Config
7. Const - Form - CSS - Selector - WOVG - Config
8. Const - Page Not Found - CSS - WOVG - Config
9. Const - Query - Accepted - WOVG - Config
10. DOM - Meta - Content Type - WOVG - Config
11. DOM - Meta - Site Section - WOVG - Config
12. GA - Event - Scroll Depth - WOVG - Config
13. LTR - Scrolling - Activated - Page - WOVG - Config

Once you have configured the container, preview it and make sure everything is working as expected.
