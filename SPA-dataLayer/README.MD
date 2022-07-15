## Initial dataLayer
The following code needs to be added to site above the Google Tag Manager script in the header on every page of the website

When creating the dataLayer, it is very important that the following is adhered to:
* Only declared/created once on page
* Must be created before/above the Google Tag Manager script

Please note this does not replace the existing dataLayer, these values should be added and merged into the current dataLayer creation across the website. Some of the keys have been re-organised and have been noted in the documentation.

**Trigger:** All pages (SPA)

**Code (JavaScript):** 

```
 var dataLayer = [{
	"route" : {
		"current" : "pageCurrent", // e.g. /new/page/path
		"previous" : "pagePrevious", // (optional) e.g. /last/page/path
		"title" : "pageTitle" // (optional) e.g. New Page Title
	}
	// +existing key values
	"content" : {
		"environment" : contentEnvironment, // e.g. prod,uat
		"type" : contentType, // e.g. page template. Home,article,listing,category,pdp
		"version" : deploymentVersion, // e.g. website deployment version
		"uiExperience" : contentUiExperience // eg. desktop,mobile,responsive
	},
	"user" : {
		"id" : userId, // e.g. A unique ID for the user..
		"type" : userType, // e.g. guest/member/admin/vip
		"postcode" : userPostcode, // e.g. 3000
		"state" : userState, // e.g. VIC
		"segment" : userSegment, // e.g. user group if applicable
		"sessionId" : userSessionId // e.g. A unique session id for the user
	}
}];

```

## Routing
**Trigger:**
* When the content updates without reloading the browser
* Required for Single Page Applications (SPA)


**Code (JavaScript): Example**

```
dataLayer.push({
  "pageType": "PageView",
  "pageUrl": "/",
  "pageTitle": "Find, connect, shape your Victorian Government | Victorian Government",
  "event": "routeChange"
});
```
