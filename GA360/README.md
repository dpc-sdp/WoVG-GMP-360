# Set up and report performance measurement for the WoVG with Google Analytics
Use these instructions to comply with the standard for the Victorian government for adding the Google Analytics tracking code to your website.

This process is **NOT** for Single Digital Presence sites.

## Configure Google Analytics
Before you start, have your Google Analytics Universal Analytics (UA-XXXXXXXX-X) number from your site’s account ready.

If you need to set up a new UA, follow [these instructions from the Google website](https://support.google.com/analytics/answer/1042508?hl=en) or log a [support ticket with the Analytics Team](https://digital-engagement.atlassian.net/servicedesk/customer/portal/11/group/16/create/69).

### Naming Convention
These are the WoVG naming convention for Google Analytics Accounts, Properties and Views.

#### Account Name:
Create any new properties under your Departmental Account. 
* Department of Education and Training
* Department of Environment, Land, Water and Planning 
* Department of Families, Fairness and Housing
* Department of Health
* Department of Jobs, Precincts and Regions
* Department of Justice and Community Safety
* Department of Premier and Cabinet
* Department of Transport
* Department of Treasury and Finance

If your agency doesn't fall directly under one of the nine departments then or you don't know who your departmental account admin is, then log a [support ticket with the Analytics Team](https://digital-engagement.atlassian.net/servicedesk/customer/portal/11/group/16/create/69) and we will assist you.

For the Department of Premier and Cabinet, this would be:
* **Department of Premier and Cabinet**

**NOTE:** Account names are just that, names. So if your department changes its name or domain the Account Name can easily be updated to reflect that without harm to your data. The same goes for Property and View Names.

#### Property:
Properties should follow this convention, domain name - environment 

Where the domain name is that of the site you are tracking and the environment is either Production or Test.

You need two (2) Properties, one for your Live/Production site, and one for UAT/Test site
1. **dpc.vic.gov.au - Production**
2. **dpc.vic.gov.au - Test**

If you are using the [WoVG GTM Container](https://github.com/dpc-sdp/WoVG-GMP-360/tree/master/GTM360), you will need to add the required custom dimensions.
In Google Analytics, open Property >> Custom Definitions and configure your Custom Dimensions
If you aren't currently using custom dimensions you will need to pre-fill Dimension 01 to 20 with "holder.reuse (h-01)" and set to inactive.
If you can't add more than 20 custom dimensions then you haven't been upgraded to Google Analytics 360, log a [support ticket with the Analytics Team](https://digital-engagement.atlassian.net/servicedesk/customer/portal/11/group/16/create/69).

Name | Scope | State
------ | ------ | ------
holder.reuse (h-01) | HIT | Inactive
...|...
holder.reuse (h-20) | HIT | Inactive
content.site.section (h-21) | HIT | Active
content.publication.name (h-22) | HIT | Active
content.type (h-23) | HIT | Active
gtm.container.id (h-24) | HIT | Active
gtm.container.version (h-25) | HIT | Active
click.download.file.type (h-26) | HIT | Active
page.keyword (h-27) | HIT | Active
gtm.event (h-28) | HIT | Active
ga.client.id (u-29) | USER | Active
session.id (s-30) | SESSION | Active
click.classes (h-31) | HIT | Active
timestamp (h-32) | HIT | Active
content.filters (h-33) | HIT | Active
url.query (h-34) | HIT | Active
event.data (h-35) | HIT | Active
department (h-36) | HIT | Active
content.wordcount.range (h-37) | HIT | Active
content.wordcount (h-38) | HIT | Active
content.read.time (h-39) | HIT | Active

#### Views:
Your production property should have at least two (2) views

1. **Prod - Raw - dpc.vic.gov.au** In the view settings:
  * Uncheck **Bot Filtering**
  * Turn on **Site search Tracking** but don't strip the query 
2. **Prod - Filtered - dpc.vic.gov.au**

##### Recomended filters
* Lowercase Campaign Source
* Lowercase Campaign Medium
* Lowercase Campaign Name
* Lowercase Hostname
* Lowercase Request URI
* Lowercase Search Term
* Lowercase Event Category
* Lowercase Event Action
* Lowercase Event Label
* Lowercase Page Title
* Remove www from Hostname ([?](https://user-images.githubusercontent.com/32256920/116497240-37fbe200-a8ea-11eb-88d5-83258603e2be.png))

Your Test property only needs one view, though you can set up other views to test features before moving to the production view
1. **Test - Raw - dpc.vic.gov.au** Use the same settings as your **Prod - Raw** view.
