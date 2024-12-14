# Expo CLI Android Build Failure: SDK Build Tools and Gradle Version Mismatch

This repository demonstrates a common but elusive bug encountered when building Android apps using the Expo CLI. The issue stems from an incompatibility between the Android SDK build tools version and the Gradle version specified in your project's `android/gradle` files.  While the error messages may not always clearly indicate this root cause, they often manifest as general build failures or errors concerning signing, dependencies, or the overall build process.

The `bug.js` file showcases a typical Expo project setup where the versions might conflict, and `bugSolution.js` offers a solution to resolving the issue.

**To reproduce the bug:**
1. Install and run the project as it is in `bug.js`
2. Try running `expo build:android` and observe the build failure.
3. Apply the solution in `bugSolution.js` and rebuild the app.

**Note:**  This error may require adjusting Gradle versions, Android SDK build tools versions, and potentially other Android-related settings in your project's `android/` directory.  The precise solution will depend on your app's specific dependencies and configurations.  Consult the official Expo documentation for the most up-to-date guidance on Android build requirements.