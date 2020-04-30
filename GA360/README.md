# Set up and report performance measurement for the WoVG with Google Analytics
Use these instructions to comply with the mandatory standard for the Victorian government for adding the Google Analytics tracking code to your website.

This process is **NOT** for Single Digital Presence sites.

## Configure Google Analytics
Before you start, have your Google Analytics Universal Analytics (UA) number from your site’s account ready.

If you need to set up a new UA, follow [these instructions from the Google website](https://support.google.com/analytics/answer/1042508?hl=en)

### Naming Convention
These are the WoVG naming convention for Google Analytics Accounts, Properties and Views.

#### Account Name:
Use your primary domain name, don’t include the www from the hostname.

For the Department of Premier and Cabinet, this would be:
* **dpc.vic.gov.au**

**NOTE:** Account names are just that, names. So if your department changes its name or domain the Account Name can easily be updated to reflect that without harm to your data. The same goes for Property and View Names.

#### Property:
Properties should follow this convention, domain name - environment 

Where the domain name is the that of the site you are tracking and the environment is either Production or Test.

You need two (2) Properties, one for your Live/Production site, and one for UAT/Test site
1. **dpc.vic.gov.au - Production**
2. **dpc.vic.gov.au - Test**

#### Views:
Your production property should have at least two (2) views

1. **Prod - Raw - dpc.vic.gov.au**
2. **Prod - Filtered - dpc.vic.gov.au**

##### Recomended filters
* Lowercase URL
* Lowercase Source
* Lowercase Medium
* Lowercase Search Term
* Lowercase Campaign Name
* Include Hostname only (e.g. dpc.vic.gov.au)
* Remove www from Hostname

Your Test property only needs one view, though you can set up other views to test features before moving to the production view
1. **Test - Raw - dpc.vic.gov.au**
