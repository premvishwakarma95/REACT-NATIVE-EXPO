# REACT-NATIVE-EXPO

React native works same as react and routing same as nextjs file based and file sytem nextjs as and css different and html tags different.

## Get the starter project
Run the following command to clone a starter project locally:

```bash
npx create-expo-app my-app
cd my-app
npx eas-cli@latest login
npx eas-cli@latest init
```

## Run the project
```bash
npx expo start
```
Remember you need to install expo app and connect with same wifi and scan QR then you can see changes on phone real time changes.

---

## How to create build
Run this command to install eas-cli
```
npm install -g eas-cli
```
No you can run build command
```
eas build

// Separate buld command
// 🤖 Android Build
// .apk for testing, .aab for producton.
npx eas build -p android --profile preview      // 👉 APK (for testing)
npx eas build -p android --profile production   // 👉 AAB (for Play Store)

🍎 iOS Build `.ipa → upload to Apple App Store`
npx eas build -p ios

// 👉 Will require:
// Apple ID
// Apple Developer account
```
Then i will ask `All`, `Android` and `ios` then select `All` because we want to create build for both.

## Need to ask client
```
Hi, I’ve started working on generating Android and iOS builds using Expo.

For Android build, I can proceed using EAS without any issues.

For iOS build, I need a few details:

1. Apple Developer account access (or should I use a company account?)
2. Apple ID for signing the app
3. Any existing bundle identifier or should I create a new one?

Also, please confirm:

* App name (final)
* Package/bundle identifier (if predefined)
* Whether we want APK or AAB for Android

Let me know so I can proceed with both builds smoothly.

```
