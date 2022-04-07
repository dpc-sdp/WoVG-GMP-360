# **4 - Non SDP Configuration Support**
IMPORTANT: Non SDP websites are assumed to also be non-SPA (non single page application) for the purposes of page navigation. If you are setting up GTM tracking for a Non SDP website that is an SPA website, please get in touch at analytics.team@dpc.vic.gov.au for additional guidance, as some of the below configurations will need to be different.

The below heading names mirror the names of the tags in the GTM container for easier reference. For each of these tags, please make the updates as listed.

## **CHTML - Caretaker - message.js - WOVG**

Navigate to Tags:

* Tags
* Search > "CHTML - Caretaker - message.js - WOVG"
* Click Tag

Move Tag to Folder

* Click Folder Icon
* Select "Website - Non SDP - Support"

Update Triggering:

* Navigate to Triggering
* Click Edit Icon
* Remove "CE - routeChange - WOVG"
* Click "Choose a trigger to make…"
* Select "All Pages"

## **GA - Event - Error - Content - 404 - SDP**

Navigate to Tags:

* Tags
* Search > "GA - Event - Error - Content - 404 - SDP"
* Click Tag

Move Tag to Folder

* Click Folder Icon
* Select "Website - Non SDP - Support"

Update Triggering:

* Navigate to Triggering
* Click Edit Icon
* Remove "CE - routeChange - Page not found - WOVG"
* Click "Choose a trigger to make…"
* Select "Page - DOM Ready - Page Not Found - WOVG"
