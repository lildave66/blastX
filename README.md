# 🚀 BlastX – Smart Blast Scheduler

![React Native](https://img.shields.io/badge/React%20Native-0.7+-blue?logo=react)
![Expo](https://img.shields.io/badge/Expo-Framework-black?logo=expo)
![Firebase](https://img.shields.io/badge/Firebase-Backend-orange?logo=firebase)
![License](https://img.shields.io/badge/License-MIT-green)

BlastX is a mobile application that allows users to **schedule and manage timed blast events**.  
Instead of sending bulk messages, it focuses on **push notifications**, ensuring users are notified exactly when important events occur.

---

## ✨ Features

- 🔐 Firebase Authentication (Email & Password)
- 📋 Blast List (Scheduled events)
- 🕒 History tracking (Triggered blasts)
- ⚙️ Setup page (Create & schedule blasts)
- 🔔 Push notifications (FCM + Expo)
- ☁️ Cloud Functions (Automatic scheduling)
- 👥 Multi-tenant system (Company-based data)
- 🎨 Clean dark UI (navy + orange theme)

---

## 🧱 Tech Stack

| Layer       | Technology |
|------------|-----------|
| Frontend   | React Native (Expo) |
| Backend    | Firebase |
| Database   | Cloud Firestore |
| Auth       | Firebase Authentication |
| Scheduling | Firebase Cloud Functions |
| Notifications | Firebase Cloud Messaging + Expo |

---

### 📂 Folder Breakdown
- **screens/**
  - `Login.js` → User login screen  
  - `Signup.js` → User registration screen  
  - `BlastList.js` → Main dashboard or feed  
  - `History.js` → Past activity logs  
  - `Setup.js` → Onboarding or initial configuration  

- **navigation/**
  - `Tabs.js` → Tab-based navigation setup  

- **firebase.js** → Firebase configuration (auth, Firestore, storage)  
- **theme.js** → Centralized styling (colors, typography, spacing)  
- **notifications.js** → Push/local notification handling  
- **App.js** → Entry point tying everything together  

---

Would you like me to also add **Markdown links** to each file (so they can be clicked in docs), or keep it as a plain tree diagram?

## ⚙️ Installation

```bash
git clone https://github.com/lildave66/blastx.git
cd blastx
npm install
```
## 🔑 Firebase Setup

To configure Firebase for BlastX, follow the steps below:

### 1. Create a Firebase Project
- Go to the [Firebase Console](https://console.firebase.google.com/)
- Click **"Add Project"**
- Follow the setup wizard

---

### 2. Enable Required Services

Within your Firebase project, enable the following:

- **Authentication**
  - Method: Email & Password

- **Cloud Firestore**
  - Start in production or test mode (based on your needs)

- **Cloud Functions**
  - Required for scheduling and triggering notifications

- **Cloud Messaging (FCM)**
  - Used for push notifications

---

### 3. Add Firebase Configuration

Create a `firebase.js` file in your project and add your Firebase configuration:

```js
// firebase.js
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_AUTH_DOMAIN",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_STORAGE_BUCKET",
  messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  appId: "YOUR_APP_ID"
};


