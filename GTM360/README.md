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
Once you have your container installed it is time to configure it. You have a couple of options:
1. Basic Tracking
   * Will cover normal site usage
2. Medium Tracking
   * Basic plus more
3. Advanced tracking
   * All the bells and whistles

Download the latest version of your Container of choice (Link to Git Repo?)

##### Constants
For basic tracking simply modify the following constants.
