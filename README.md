# VITAS Mobile Referral Application

A modernized mobile platform enabling healthcare professionals to efficiently refer hospice-eligible patients with integrated clinical tools and location-based services.

## 📚 Table of Contents

- [📦 Prerequisites](#Prerequisites)
- [🏃‍♀️ How to Run (Developers)](#How-to-Run-the-App-For-Developers)
- [🚀 How to create a Build (Development)](#How-to-create-a-Build-development)
- [🧪 Testing Guide (QA)](#Testing-Guide-QA)

## Prerequisites

Make sure the following tools are installed:

- Node.js
- Expo CLI
- Expo Go app (for device testing)

## How to Run the App (For Developers)

This guide is for developers working on the app locally.

### 1. Install Dependencies

```bash
npm install
# or
yarn install
```

## How to create a Build (Development)

This section explains how to generate **custom development builds** for Android and iOS using EAS Build.

### 📦 1. Common Setup

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

## Testing Guide (QA)

This section is for testers to install and test the production build.

### For Android Testing (via APK)

1. Tap the link shared with you to download the .apk file.
2. Enable installation from unknown sources in device settings.
3. Open the downloaded file and tap Install.
4. Launch the app and begin testing.

### For iOS Testing (via TestFlight)

1. **Install the TestFlight app** from the App Store (if not already installed).
2. **Accept the invite**:
   - You'll receive an email or public link → Tap **View in TestFlight**.
3. **Install the app**:
   - New testers: Tap **Accept** → **Install**
   - Existing testers: Tap **Update** or **Open**
4. **Open the app** and begin testing.
5. You can **submit feedback directly from TestFlight**.

