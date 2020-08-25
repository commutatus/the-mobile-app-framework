# Do I need Codepush?
 Yes. You do. You don't know it yet but you do.

 ## Why do I need it?
You need it to release OTA updates for the reasons mentioned [here](OTA.md).

## Installation
Codepush is a part of App Center so you'll need to install both App Center and Codepush. 

1. Create two apps on [App Center](https://appcenter.ms/apps) for Android and iOS variant.
2. Go into the android app and install the app center dependencies.
3. Go to `Distribute` and select `CodePush`. Install the dependencies and make the native changes required.
4. If you're using Wix Native Navigation then follow the steps mentioned over [here](https://github.com/microsoft/react-native-code-push/blob/master/docs/setup-android.md#wix-react-native-navigation-applications).
5. You might have to check the format of `MainApplication.java` file to select the correct approach.

## Making a CodePush release
1. You'll need to have `appcenter-cli` installed.
2. Run `appcenter apps set-current` followed with the app name to select the app center app which will get the CodePush update.
3. You can release the update by `appcenter codepush release-react`.
4. It will get released to the staging track on App Center. 
5. Verify if the release is working fine on the staging build and then release the update to production.