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
```
Then i will ask `All`, `Android` and `ios` then select `All` because we want to create build for both.

## Need to ask client
```
Hi, as we are preparing for app deployment, I need the following details:

1. Access to your Google Play Store and Apple App Store developer accounts (or please add me as a developer)
2. App name, description, category, and keywords
3. App icon (1024x1024) and splash screen (if available)
4. App screenshots for listing
5. Privacy Policy URL and Terms & Conditions (if available)
6. Production API URL and any required API keys (Firebase, payment, etc.)
7. Test login credentials for app review
8. Confirmation of app permissions (camera, location, etc.)
9. Final confirmation on app name and version

This will help us complete the deployment smoothly.
```
