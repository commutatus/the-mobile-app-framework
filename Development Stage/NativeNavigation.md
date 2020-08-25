# Using Wix Native Navigation instead of JS navigation

## Why should I use Wix Native Navigation over React Navigation?
1. JS navigation, as the name suggests works on the JavaScript thread. It is not memory optimized or performant either.
2. Native Navigation works by utilizing the native platform's capabilities. 
3. The transition animations are native to the OS and don't feel out of the place.
4. Native navigation actually helps with the RAM usage.
5. Offers everything that React Navigation offers and then some more.
6. Native Navigation features a new lifecycle method, ```DidComponentAppear```.
7. Native Navigation allows components to be animated across screens.

## Issues with Wix Native Navigation:
1. V6 had some issues with Android API level 26 on Xiaomi devices. This was recently fixed apparently. Check your app on Firebase's Testlab to be sure. Alternatively, you can use V4 of Wix Native Navigation to avoid this issue just in case.
2. Deep Linking has to be manually implemented.

## How to integrate it?
You can find the latest instructions at their official documentation here:  
<https://wix.github.io/react-native-navigation/docs/before-you-start/>