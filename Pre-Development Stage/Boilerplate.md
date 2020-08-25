# Does having a Boilerplate app make any sense ?

## Flutter:
1. Yes, having a boilerplate app in Flutter makes sense as it would save some time when starting out a new project. 
2. However, I'd suggest refraining from adding native dependent plugins to the boilerplate itself. 
The reasoning behind this being that if the native plugin gets an update which requires you to make some changes on the native side, then you end up doing the whole integration again, thus defeating the purpose of the boilerplate.  
3. If you feel that you definitely need such a plugin in your boilerplate then sure, go ahead, but try to keep updating the boilerplate from time to time to avoid bottlenecks when startinga monetized project.

## React Native:
1. No, a Boilerplate app for React Native makes no sense to me.
2. This is because of the manual and cruel process of updating the React Native version unlike Flutter which is mostly automatic.
3. For example, Let's say you had a boilerplate app in React Native 0.60 and you wanted to create a new app. Either you can use the boilerplate and then upgrade to the latest version (i.e. 0.63.2 at the time of writing this article), or you can simply init a new app. Guess which one's easier?
4. Updating React Native version can also create a mess with other packages as well.
5. Therefore, having a boilerplate app in React Native makes no sense.