# OTA Updates
 ## Why do we need OTA updates?
 The possibilities are endless with OTA updates. Here are a few use-cases for OTA updates:
 1. Fix minor bugs where making the users download the update seems redundant, especially right after a production release.
 2. Make a sneaky update to the functionality.
 3. Add new minor features.
 4. Make urgent changes.

---
## Flutter vs React Native  
OTAs are perfectly fine in case of React Native, but what about Flutter? How can you work with OTAs on Flutter?

Since OTA updates are only possible on Android  at the moment, here's a guide on how we can circumnavigate the issue:  
1. Proper and extensive testing before releasing the app to the production.
2. Since Flutter has the support for android OTA updates, release the Android variant before iOS, and wait for 2-3 days to get the feedback/reports from the users / client about potential bugs.
3. Fix those issues and make an OTA update as well as an Play Store Release.
4. Once everything has been sorted out, make the iOS release too.

