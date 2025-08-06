# VITAS Mobile Referral Application

VITAS Mobile Referral Application enables healthcare professionals to efficiently refer hospice-eligible patients with integrated clinical tools and location-based services.

## 📚 Table of Contents

- [📦 Prerequisites](#Prerequisites)
- [🏃‍♀️ How to Run (Developers)](#How-to-Run-the-App-For-Developers)
- [🚀 How to create a Build (Development)](#How-to-create-a-Build-development)
- [🧪 Testing Guide (QA)](#Testing-Guide-QA)

## Prerequisites

Make sure the following tools are installed:

- Node.js >= 16.x
- Expo CLI 
- Expo Go app (for device testing)

## How to Run the App (For Developers)

This guide is for developers working on the app locally.

### 1. Clone the Repository

```bash
git clone https://github.com/your-org/vitas-mobile-referral.git
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

### 📱 Run the App on Your Device

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

