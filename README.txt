wear what? - native app build

This project can be installed as a native Android or iPhone app. The app runs
inside the platform's embedded WebView, not in a separate browser app, and its
web files are bundled into the install so the core app works offline.

Build prerequisites:
- Node.js 22 or newer
- Android Studio with Android SDK and JDK 21 for Android
- macOS with Xcode for building/signing the iPhone app

Setup:
1. Run npm install.
2. Run npm run cap:sync after changing the app files.
3. Open android/ in Android Studio or ios/App/App.xcodeproj in Xcode to run,
   build, and sign the app for your phone. The native projects are included.

Android APK:
- In Android Studio, choose Build > Build Bundle(s) / APK(s) > Build APK(s).
- For a release APK, configure a signing key in Android Studio and build a
  signed APK. Do not share your private signing key.

iPhone:
- Building and installing on a device requires macOS, Xcode, and Apple signing.

For a browser-installable version instead, host this folder over HTTPS and
follow the browser's Add to Home Screen / Install app option.
Use More > Export backup now and then to keep a copy of your wardrobe.
