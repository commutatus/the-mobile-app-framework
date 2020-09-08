# How do we structure the directories, screens, components and other files?

There's 2 kinds of architecture that we may use depending upon the size of the app.
Let's call these apps:
1. Slim apps
2. Jumbo apps

Now, a question arises. 

**_How do we differentiate between the two?_**
Well the answer is pretty simple. We provide a threshold to differentiate between the two.

#### Threshold for Slim Flutter Apps
**Components:** 15-20
**Screens:** 10
#### Threshold for Slim React Native Apps
**Components:** 25
**Screens:** 20

If your app demands components/screens more than the threshold mentioned above, then it should be categorised as a **Jumbo app**. Otherwise it's a **Slim app**.

Moving on, let's call the root directory (**src** in React Native and **lib** in Flutter) as **Root**.
This is where all our code stays. The architecture here will be dependent on the type of the app and will influence the directories. 
However, there's a few things that remain constant regardless of app type.

## Architecture for Slim Apps:
- root (src / lib)
    - screens
        - Splash.js / Splash.dart
        - Login.js / Login.dart
    - components
        - Button.js / Button.dart
        - CustomInput.js / CustomInput.dart
    - global
        - style.js / style.dart
        - constants.js / constants.dart
    - configs
        - firebase.js / firebase.dart
        - sentry.js / sentry.dart
    - redux
        - store
        - actions
        - reducers
    - assets
        - images
        - sounds

## Architecture for Jumbo Apps:
- root (src / lib)
    - Login
        - screens
            - Login.js / Login.dart
            - Signup.js / Signup.dart
        - components
            - Button.js / Button.dart
        - assets
            - loginLogo.png
    - Profile
        - screens
            - Profile.js / Profile.dart
            - EditProfile.js / EditProfile.dart
        - components
            - Avatar.js / Avatar.dart
        - assets
            - profile.png
    - global
        - style.js / style.dart
        - constants.js / constants.dart
    -  redux
        - store
        - actions
        - reducers
    - assets
        - images
        - sounds
  


### Explanation:
The only difference between the architecture of slim and jumbo apps is about the placement of the screens and components.

Basically, if your app has lesser number of components or screens then a single folder to hold the category is enough. 

If there are quite a few files then it makes much more sense to divide the app into smaller sections and hold the related screens and components within those smaller sections.s