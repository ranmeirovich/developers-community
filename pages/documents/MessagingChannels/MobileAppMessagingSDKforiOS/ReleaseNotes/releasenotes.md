---
pagename: Release Notes
redirect_from:
  - consumer-experience-ios-sdk-release-notes.html
Keywords:
sitesection: Documents
categoryname: "Messaging Channels"
documentname: Mobile App Messaging SDK for iOS


permalink: mobile-app-messaging-sdk-for-ios-release-notes.html
indicator: messaging
---

<div class="subscribe">Working with this SDK or planning to in the future? Make sure to <a href="https://visualping.io/?url=developers.liveperson.com/consumer-experience-ios-sdk-release-notes.html&mode=web&css=post-content">subscribe</a> to receive notifications of changes! When we update the Release Notes, you'll get a notification straight to your email of choice!</div>


### iOS Messaging SDK - Version 5.1.0
**Release Date**: January 2, 2020 

### Environmental Requirements
The iOS Mobile Messaging SDK version 5.1.0 is compatible with Xcode 11.3, Swift version 5.1.3 (swiftlang-1100.0.282.1 clang-1100.0.33.15), and supported on iOS versions 11 through 13.   

### Bugs fixed 
* Issue with background color for Agent Avatar image
* Allow ability to wrap text with in a clickable options for Structure content

#### Accesibility fixed 
* "Fill in form" button does not inform user when it is still loading
* Quick reply text is announced automatically but buttons are not
* VoiceOver begins announcing survey questions as they are published to the chat before they finish loading, causing them to be partially announced, interrupted, then announced again
* If agent sends a hyperlink, the post is announced as plain text, user has no way to know it an be activated
* Elements with functionality of hyperlinks are being announced as buttons
* Attachments are always announced as "image"
* Separator bar after completing PCS survey can receive focus

### New Features 
Scroll Behavior Configuration - clients can customize the scroll behavior for the following scenarios:
- ```showConversation``` the SDK window is shown via the call ```showConversation``` 
- ```backgroundToForeground``` the SDK Conversation is brought from background to foreground state
- ```scrollToBottomButtonPressed``` the SDK scroll to bottom button is pressed
- ```pushNotificationTapped``` a native push notification was tapped and the SDK API ```setPushNotificationTapped``` was called.

For more information, see [Scroll Behavior Configuration](mobile-app-messaging-sdk-for-ios-advanced-features-scroll-behavior-configuration.html) page. 


NOTE: 
unreadMessagesDivider no longer impacts scroll behavior or prevents scrollToBottomButton from being display.

<br>
<p style="text-align: left">
<a href="mobile-app-messaging-sdk-for-ios-all-release-notes.html" center><img src="../img/back-to-all-release-notes.png" style="height: 30px; width: auto;"></a></p>

