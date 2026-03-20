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

---


## First prompt to create UI for app
```
You are a senior React Native engineer working on a production-grade mobile app.

Your task is to convert the provided React JSX prototype file into a fully structured, scalable React Native (Expo) application UI.

IMPORTANT CONTEXT:
- The provided file already represents the final UI design (AiyuApp_v4.jsx)
- You must replicate the UI EXACTLY (pixel-perfect as much as possible)
- This is ONLY UI development for now (no real API integration yet)
- However, structure the code in a way that APIs can be easily integrated later

TECH STACK REQUIREMENTS:
- React Native with Expo (latest stable)
- TypeScript
- Expo Router (file-based navigation)
- Tailwind styling using NativeWind
- Use functional components + hooks
- Use clean, modular, scalable architecture

APP STRUCTURE REQUIREMENTS:
Create a proper folder structure:

/app
  /(tabs)
    home.tsx
    inbox.tsx
    agents.tsx
    experts.tsx
    brain.tsx
    settings.tsx
  /onboarding
    step1.tsx
    step2.tsx
    step3.tsx
    step4.tsx
    step5.tsx
  _layout.tsx

/components
  /ui
  /cards
  /chat
  /agents
  /common

/constants
/hooks
/context
/utils

CORE REQUIREMENTS:

1. Navigation
- Implement bottom tab navigation with 6 tabs:
  Home, Inbox, Agents, Experts, Brain, Settings
- Use Expo Router
- Add icons using @expo/vector-icons

2. Onboarding Flow
- 5-step onboarding screens
- Store completion state using AsyncStorage
- Redirect to app after completion

3. UI IMPLEMENTATION (STRICT)
- Recreate ALL UI from provided JSX exactly:
  - Layout
  - Spacing
  - Colors
  - Typography
  - Components
- Convert web-based styles into React Native compatible styles

4. STATE HANDLING
- Use local state only (useState/useContext)
- Do NOT integrate APIs yet
- Use mock data where needed

5. REUSABILITY
- Extract reusable components:
  - Cards
  - Buttons
  - Chat bubbles
  - Agent cards
  - Skill cards

6. ANIMATIONS
- Use React Native Reanimated or basic Animated API where needed:
  - AI avatar pulse
  - Wave animations
  - Loading states

7. THEME SUPPORT
- Implement Dark / Light mode toggle
- Store preference in AsyncStorage

8. CODE QUALITY
- Clean, readable, production-level code
- Use TypeScript types everywhere
- Avoid inline styles (use Tailwind classes via NativeWind)

9. PLACEHOLDERS FOR BACKEND
- Add comments like:
  // TODO: Integrate API here
  // TODO: Replace mock data with backend response

10. OUTPUT FORMAT
- Provide full working code
- Include:
  - package.json dependencies
  - folder structure
  - all screens and components
- Code should run directly using:
  npx expo start

INPUT FILE:
I will now provide the JSX prototype file.
You must convert it into a proper React Native Expo app as per above instructions.

DO NOT:
- Skip any UI
- Simplify layouts
- Ignore responsiveness
- Use web-only libraries

GOAL:
Create a clean, scalable, production-ready UI foundation that matches the prototype exactly and is ready for backend integration.
```
