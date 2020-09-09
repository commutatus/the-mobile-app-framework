# What is Semantic Versioning?
It is a globally accepted set of rules followed by developers to version their products in a uniform and a descriptive manner which makes sense to the bulk of the users.

### How does it work?
You might have seen apps having a version number like **2.9.4** or even **1.0.0**.
This is an example of Semantic versioning.

Semantic versioning can be written as:
**Major.Minor.Patch**

Let's consider an app version **2.9.4**.
In this case, **2** would be a **Major** version, **9** would be a minor version and **4** would be a **Patch** version.

### What does Major, Minor and Patch mean here?
**Major:** Refers to a non backward compatible feature or an API that has been added to the app.
Releasing this would essentially break the previous versions of the app.

**Minor:** Refers to a new feature that has been added to the app which is backward compatible. Releasing this won't break the previous versions of the app, albeit they'll be sans the new features.

**Patch:** Refers to a bug fix that has been made to the existing code. Releasing this will neither break the app nor add new features. It will simply fix an undesirable behaviour.

### Rules:
1. You can only increment these version numbers with each release according to the change.
2. Using a version number lesser than the version currently on production isn't allowed and is strictly enforced by the App/Play Store.

## Note:
1. A Pre-Release Major version 0.x.x can be used before releasing to the production.
2. There's a build number on iOS and version code on android that is simply the count of builds that have been built till now. These don't get resetted and should be incremented with build. These don't follow the semantic versioning.
For Example: 1 -> 2 -> 3 -> ..... -> 98 -> 99 -> 100 and so on.
3. Each version number is not only limited from 0 to 9. 2.65.12 is a completely valid version number.
4. 1.9.8 < 1.11.0 < 2.0.0 

You can read more about it [here](https://semver.org/).