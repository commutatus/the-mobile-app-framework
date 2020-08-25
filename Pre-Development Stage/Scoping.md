## How to decide if the app should be in Flutter or React Native?

There is no clear cut answer to this question. Each app is different. There are a lot of factors to consider before answering this question. And each developer / client might weigh these factors differently. 

Hence, I came up with the following questionare to make this decision a tad bit easier.

## Answer the following questions and then go through the explanation to get the verdict:

**1.  How dependent will you be on OTA updates for bug fixes?**   
**2.  How intensive will the background tasks or calculations be?**  
**3.  How complex Native APIs are going to be used in the app?**  
**4.  Are complicated animations a requirement in the app?**    
**5.  Are there a lot of screens in the app but they're mostly simple?**  
**6.  Is the app small and supposed to be pushed out quickly?**  
**7.  Is the UI going to be implementing a custom UI which remains consistent over different platforms? Or will the UI implement native components?**       

## Explanation:
1. The table below will help understand the point better  
 
| React Native  | Flutter  |
|---|---|
| 1. OTA updates will be quite easy.  | OTA updates are a bit difficult.  |
| 2. Will work on both Android and iOS.  | Only works on Android at the time of writing this article (22-8-2020) |
| 3. Smaller update size due to JS bundle getting updated  |  Downloads the whole APK / IPA, thus the update will be as big as the app itself.  |
| 4. Native dependencies will not get updated | Since the whole app is getting downloaded, the native dependencies will be updated as well. |

1.  If the app is reliant on background tasks and calculations, then Flutter would be a better choice over React Native. 
2.  Mostly both of the Frameworks are same in terms of basic Native API usage. But Flutter shines when the app requires complex Native APIs like Bluetooth.
3.  If the app requires basic transitions and layout animations then React Native is good to go. Complicated animations can be implemented via Lottie. Otherwise if the app is heavily reliant on complicated transition and shared animations then Flutter is better suited to the need.
4.  If the app is mostly simple and only huge in terms of screens/content then React Native seems to be a better choice as that would allow you to use Codepush without sacrificing any performance gains that Flutter would offer over React Native.
5.  If the app is small and has a quick timeline then sticking to Flutter can be benficial over React Native as Flutter has unbeatable Time-To-Market durations.
6. If the app is going to have a custom UI which will remain consistent across platforms then sticking to Flutter would make more sense, whereas, if the app implements the Native UI Components then React Native should be better off here.
  
### Steps to get the verdict:
1. Arrange these points in the order of priority, which makes sense to the project and the client's requirements.
2. Multiply the result of the top priority with 7, the 2nd one with 6 and so on..
3. The framework with a greater score should be your answer.

## Example:
For the default priority order mentioned above the score for MyCaptain app would be:
1. 7x React Native 
2. 6x React native
3. 5x React native
4. 4x React native
5. 3x React Native
6. 2x React Native
7. 1x Flutter

**Score**:  
  *React Native* = 27  
  *Flutter* = 1 

Thus, MyCaptain app should be on React Native.

This, under no circumstances, should be considered as the final verdict. The final decision should be made after proper research and thorough examination of available plugins to get the job done.   
Treat this guide's result as a suggestion alone.

### [OTA updates are further discussed in  OTA section of Development Stage. Click Here to give it a read and further understand the issue.](../Development%20Stage/OTA.md)
