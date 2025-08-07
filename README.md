# VITAS Mobile Application

VITAS Mobile Application is a versatile healthcare app designed to streamline hospice and palliative care workflows. It offers tools for clinical support, referral management, educational resources, and secure access.

##  Table of Contents

- [Prerequisites](#Prerequisites)
- [How to Run the App (Developers)](#How-to-Run-the-App-For-Developers)
- [How to create a Build (Development)](#How-to-create-a-Build-development)


## Prerequisites

Make sure the following tools are installed:

- Node.js (v22.18.0)
- Expo CLI – use the latest via **npx expo** (no global install needed) 
- Expo Go app (Latest from App Store/Play Store)

## How to Run the App (For Developers)

This guide is for developers working on the app locally.

### 1. Clone the Repository

```bash
git clone https://github.com/your-org/project-name.git
```

### 2. Install Dependencies

```bash
npm install
# or
yarn install
```

### 3. Install Expo CLI (if not already)

```bash
npm install -g expo-cli
```

### 4. Start the Development Server
```bash
npx expo start
```

This will open Expo Developer Tools in your browser.

### Run the App on Your Device

#### Option 1: Using Expo Go (iOS/Android)
1. Install the **Expo Go** app from the App Store or Play Store.
2. Scan the QR code shown in your terminal using Expo Go Scanner.
3. The app will open and reload automatically with your latest code.

#### Option 2: Using Emulator/Simulator
1. Press a to open the Android emulator (if installed).
2. Press i to open the iOS simulator (macOS only, requires Xcode).
3. Press w to run on Web (optional).

## How to create a Build (Development)

This section explains how to generate **custom development builds** for Android and iOS using EAS Build.

###  1. Common Setup

#### Install Required Tools
```bash
# Install expo-dev-client
npx expo install expo-dev-client

# Install EAS CLI globally
npm install -g eas-cli
```
#### Login to Expo

```bash
eas login
```

#### Configure EAS Build

```bash
eas build:configure
```

### 2. Android Development Build

``` bash
eas build --platform android --profile development
```

### 3. iOS Development Build

#### Register your iOS device

```bash
eas device:create
```

#### Run the build

```bash
eas build --platform ios --profile development
```

