# **3 - Custom Dimensions**

The Google Tag Manager Container is preconfigured to send custom data points to Google Analytics via Custom Dimensions.

( [https://support.google.com/analytics/answer/2709829?hl=en](https://support.google.com/analytics/answer/2709829?hl=en))

Custom Dimensions & Metrics work on an index (number 1-200). These indexes are already setup in Google Tag Manager, however it is very likely the Google Analytics property will need to be configured to match.

The standard version of Google Analytics provides 20 custom dimensions and 20 metrics. The 360 (premium) version provides 200 each. In order to prevent conflict with pre-existing configurations index’s are started from 20+. Allowing the first 20 to be used by a department as required. If these are not required, you will still need to create them, simply use the name "holder" and set to inactive.

<table>
  <tr>
   <td><strong>Index</strong>
   </td>
   <td><strong>Name</strong>
   </td>
   <td><strong>Scope</strong>
   </td>
   <td><strong>State</strong>
   </td>
  </tr>
  <tr>
   <td>1-20
   </td>
   <td>holder/Existing Name
   </td>
   <td>Hit/Existing Scope
   </td>
   <td>Inactive/Existing State
   </td>
  </tr>
  <tr>
   <td>21
   </td>
   <td>content.site.section (h-21)
   </td>
   <td>Hit
   </td>
   <td>Active
   </td>
  </tr>
  <tr>
   <td>22
   </td>
   <td>content.publication.name (h-22)
   </td>
   <td>Hit
   </td>
   <td>Active
   </td>
  </tr>
  <tr>
   <td>23
   </td>
   <td>content.type (h-23)
   </td>
   <td>Hit
   </td>
   <td>Active
   </td>
  </tr>
  <tr>
   <td>24
   </td>
   <td>gtm.container.id (h-24)
   </td>
   <td>Hit
   </td>
   <td>Active
   </td>
  </tr>
  <tr>
   <td>25
   </td>
   <td>gtm.container.version (h-25)
   </td>
   <td>Hit
   </td>
   <td>Active
   </td>
  </tr>
  <tr>
   <td>26
   </td>
   <td>click.download.file.type (h-26)
   </td>
   <td>Hit
   </td>
   <td>Active
   </td>
  </tr>
  <tr>
   <td>27
   </td>
   <td>page.keyword (h-27)
   </td>
   <td>Hit
   </td>
   <td>Active
   </td>
  </tr>
  <tr>
   <td>28
   </td>
   <td>gtm.event (h-28)
   </td>
   <td>Hit
   </td>
   <td>Active
   </td>
  </tr>
  <tr>
   <td>29
   </td>
   <td>ga.client.id (u-29)
   </td>
   <td>User
   </td>
   <td>Active
   </td>
  </tr>
  <tr>
   <td>30
   </td>
   <td>session.id (s-30)
   </td>
   <td>Session
   </td>
   <td>Active
   </td>
  </tr>
  <tr>
   <td>31
   </td>
   <td>click.classes (h-31)
   </td>
   <td>Hit
   </td>
   <td>Active
   </td>
  </tr>
  <tr>
   <td>32
   </td>
   <td>timestamp (h-32)
   </td>
   <td>Hit
   </td>
   <td>Active
   </td>
  </tr>
  <tr>
   <td>33
   </td>
   <td>content.filters (h-33)
   </td>
   <td>Hit
   </td>
   <td>Active
   </td>
  </tr>
  <tr>
   <td>34
   </td>
   <td>url.query (h-34)
   </td>
   <td>Hit
   </td>
   <td>Active
   </td>
  </tr>
  <tr>
   <td>35
   </td>
   <td>event.data (h-35)
   </td>
   <td>Hit
   </td>
   <td>Active
   </td>
  </tr>
  <tr>
   <td>36
   </td>
   <td>department (h-36)
   </td>
   <td>Hit
   </td>
   <td>Active
   </td>
  </tr>
  <tr>
   <td>37
   </td>
   <td>content.wordcount.range (h-37)
   </td>
   <td>Hit
   </td>
   <td>Active
   </td>
  </tr>
  <tr>
   <td>38
   </td>
   <td>content.wordcount (h-38)
   </td>
   <td>Hit
   </td>
   <td>Active
   </td>
  </tr>
  <tr>
   <td>39
   </td>
   <td>content.read.time (h-39)
   </td>
   <td>Hit
   </td>
   <td>Active
   </td>
  </tr>
</table>
