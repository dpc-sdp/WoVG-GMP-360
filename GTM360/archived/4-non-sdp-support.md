# **4 - Non SDP Configuration Support**
**IMPORTANT**: Non SDP websites are assumed to also be non-SPA (non single page application) for the purposes of page navigation. If you are setting up GTM tracking for a Non SDP website that is an SPA website, please get in touch at analytics.team@dpc.vic.gov.au for additional guidance, as some of the below configurations will need to be different.

The below heading names mirror the names of the tags in the GTM container for easier reference. For each of these tags, please make the updates as listed.

## **Universal Analytics (if applicable)**
### **GA - Event - Error - Content - 404 - SDP**

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

### **GA - Pageview - WOVG**
Navigate to Tags:
* Tags
* Search > “GA - Pageview - WOVG”
* Click Tag

Update Paused:
* Click “Unpause”

Navigate to Tags:
* Tags
* Search > “GA - Pageview - Route Change - WOVG”
* Click Tag

Update Paused:
* Click “Stacked Dots” (Next to Save button in the top right)
* From the menu click “Pause”

### **GA - Event - Content - Feedback - Cancel - SDP**

**_Update requires developer knowledge (HTML/CSS/JavaScript)_**

Navigate to Tags:

* Tags
* Search > "GA - Event - Content - Feedback - Cancel - SDP"
* Click Tag

Update Triggering:

* Navigate to Triggering
* Click Trigger "Click - Feedback - Button - Cancel - SDP"
* Edit "Fire this trigger…" CSS selector value input
    * You will need to use CSS selectors to target the cancel button on your feedback form.
    * [https://www.w3schools.com/CSSref/CSS_selectors.asp](https://www.w3schools.com/CSSref/CSS_selectors.asp)

![alt_text](assets/image14.jpg "image_tooltip")

Move Trigger to Folder

* Click Folder Icon
* Select "Website - Non SDP - Support"

Update Variable :

* Navigate to Variables
* Scroll down to "User-Defined Variables"
* Search for "CJS - Feedback Form - Yes/No status"
* Click "CJS - Feedback Form - Yes/No status"
* Edit "document.querySelector" to target your yes/no opinion.
    * Adjust Custom Javascript as required
    * Return value should be "yes" or "no" or "no-value"

Move Variable to Folder

* Click Folder Icon
* Select "Website - Non SDP - Support"

### **GA - Event - Content - Feedback - SDP**

**_Update requires developer knowledge (HTML/CSS/JavaScript)_**

Navigate to Tags:

* Tags
* Search > "GA - Event - Content - Feedback - SDP"
* Click Tag

Update Triggering:

* Navigate to Triggering
* Click Trigger "Click - Radio Button - SDP"
* Edit "Fire this trigger…" CSS selector value input
    * You will need to use CSS selectors to target the feedback value selection element
    * [https://www.w3schools.com/CSSref/CSS_selectors.asp](https://www.w3schools.com/CSSref/CSS_selectors.asp)

![alt_text](assets/image12.jpg "image_tooltip")

Move Trigger to Folder

* Click Folder Icon
* Select "Website - Non SDP - Support"

Update Variable :

* Navigate to Variables
* Scroll down to "User-Defined Variables"
* Search for "CJS - Form - Radio - Value - SDP"
* Click "CJS - Form - Radio - Value - SDP"
* Edit custom JavaScript to target the user feedback selection element.
* Return value should be "yes" or "no" or "no-value"

Move Variable to Folder

* Click Folder Icon
* Select "Website - Non SDP - Support"

### **GA - Event - Content - Feedback - Submit - SDP**

**_Update requires developer knowledge (HTML/CSS)_**

Navigate to Tags:

* Tags
* Search > "GA - Event - Content - Feedback - SDP"
* Click Tag

Update Triggering:

* Navigate to Triggering
* Click Trigger "Click - Feedback - Button - Submit - SDP"
* Edit "Fire this trigger…" CSS selector value input
    * You will need to use CSS selectors to target the form feedback submit button
    * [https://www.w3schools.com/CSSref/CSS_selectors.asp](https://www.w3schools.com/CSSref/CSS_selectors.asp)

![alt_text](assets/image20.jpg "image_tooltip")

Move Trigger to Folder

* Click Folder Icon
* Select "Website - Non SDP - Support"

### **GA - Event - Form - Complete - WOVG**

**_Update requires developer knowledge (HTML/CSS)_**

Navigate to Tags:

* Tags
* Search > "GA - Event - Form - Complete - WOVG"
* Click Tag

Update Triggering:

* Navigate to Triggering
* Click Trigger "EV - Form Complete - Confirmation Message"
* Edit "Element Selector"
    * You will need to use CSS selectors to target the form success/complete message element that is displayed to the user.
    * [https://www.w3schools.com/CSSref/CSS_selectors.asp](https://www.w3schools.com/CSSref/CSS_selectors.asp)

![alt_text](assets/image21.jpg "image_tooltip")

Move Trigger to Folder

* Click Folder Icon
* Select "Website - Non SDP - Support"

### **GA - Event - Navigation - SDP**

**_Update requires developer knowledge (HTML/CSS)_**

Update Variable :

* Navigate to Variables
* Scroll down to "User-Defined Variables"
* Search for "LTR - Navigation Types - SDP"
* Click "LTR - Navigation Types - SDP"
* Edit the "RegEx Table" "Patterns"
    * Do not change the output
    * Change the RegEx patterns to target the html elements that best represent the Output value for each row.

![alt_text](assets/image11.jpg "image_tooltip")

Move Variable to Folder

* Click Folder Icon
* Select "Website - Non SDP - Support"

### **GA - Event - Navigation - Search - Result - Click - SDP**

**_Update requires developer knowledge (HTML/CSS)_**

Navigate to Tags:

* Tags
* Search > "GA - Event - Navigation - Search - Result - Click - SDP"
* Click Tag

Update Triggering:

* Navigate to Triggering
* Click Trigger "Click - Link - Search - Result - Click - SDP"
* Edit "Fire this trigger…" CSS selector value input
    * You will need to use CSS selectors to target the search result click
    * [https://www.w3schools.com/CSSref/CSS_selectors.asp](https://www.w3schools.com/CSSref/CSS_selectors.asp)

![alt_text](assets/image15.jpg "image_tooltip")

Move Trigger to Folder

* Click Folder Icon
* Select "Website - Non SDP - Support"

### **GA - Event - Social Media Share - SDP**

**_Update requires developer knowledge (HTML/CSS)_**

Navigate to Tags:

* Tags
* Search > "GA - Event - Social Media Share - SDP"
* Click Tag

Update Triggering:

* Navigate to Triggering
* Click Trigger "Click - Social Media - SDP"
* Edit "Fire this trigger…" CSS selector value input
    * You will need to use CSS selectors to target the social share links
    * [https://www.w3schools.com/CSSref/CSS_selectors.asp](https://www.w3schools.com/CSSref/CSS_selectors.asp)

![alt_text](assets/image6.jpg "image_tooltip")

Move Trigger to Folder

* Click Folder Icon
* Select "Website - Non SDP - Support"

Update Variable :

* Navigate to Variables
* Scroll down to "User-Defined Variables"
* Search for "CJS - Social - Media - Source - SDP"
* Click "CJS - Social - Media - Source - SDP"
* Edit custom JavaScript to target the social share links
    * The current setup uses the clicked text, however you can adjust the code to what is required for social shares.
* Return values are:
    * Twitter, Facebook, LinkedIn
    * "no-value"

Move Variable to Folder
* Click Folder Icon
* Select "Website - Non SDP - Support"
