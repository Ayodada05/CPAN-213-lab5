# **PlatformSettingsApp**

A cross-platform React Native app demonstrating **platform-specific UI design** for iOS and Android.  
Developed for **CPAN 213 – Cross-Platform Mobile Application Development (Lab 5)**.

---

## **📱 Overview**

This project implements a **Platform-Specific Settings Screen** that adapts its interface to match both **iOS** and **Android** design guidelines.  
It highlights key differences such as button styles, shadows vs elevation, typography, and component layout.

---

## **🧩 Features**

- Platform detection using `Platform.OS` and `Platform.select()`
- Separate button implementations for each platform
  - **iOS**: Rounded corners, shadows, lowercase text
  - **Android**: Sharp corners, elevation, uppercase text
- Dynamic color themes using a shared utility file
- Settings screen with toggles for Notifications, Dark Mode, and Location Services
- Platform info section showing current OS details
- Reusable button components with primary and secondary variants

---

## **🗂 Project Structure**

```
PlatformSettingsApp/
├── App.js
├── src/
│   ├── components/
│   │   └── PlatformButton/
│   │       ├── index.js
│   │       ├── PlatformButton.ios.js
│   │       └── PlatformButton.android.js
│   ├── screens/
│   │   └── SettingsScreen.js
│   └── utils/
│       └── platform.js
└── ios/
└── android/
```

---

## **⚙️ Installation and Setup**

### **1. Clone the Repository**

```bash
git clone https://github.com/Ayodada05/CPAN-213-lab5.git
cd CPAN-213-lab5/PlatformSettingsApp
```

### **2. Install Dependencies**

```bash
npm install
```

### **3. Install iOS Pods**

```bash
cd ios
pod install
cd ..
```

---

## **🚀 Run the App**

### **For iOS**

```bash
npx react-native run-ios
```

### **For Android**

```bash
npx react-native run-android
```

> ⚠️ Make sure your folder path does not contain spaces to avoid Gradle and Xcode errors.

---

## **🧠 Learning Objectives**

- Implement platform-specific UI using file naming conventions
- Apply `Platform.OS` and `Platform.select()` for conditional styling
- Handle shadows vs elevation differences
- Follow native design guidelines for iOS and Android

---

## **🧪 Testing Checklist**

### **iOS**

- Rounded buttons (12pt radius)
- Shadows applied
- San Francisco font with normal casing
- Large header title (34pt)

### **Android**

- Sharp buttons (4pt radius)
- Elevation for depth
- Roboto font with uppercase text
- Standard header title (24pt)

---

## **🧱 Technologies Used**

- **React Native 0.82.0**
- **JavaScript (ES6)**
- **react-native-vector-icons**
- **react-native-safe-area-context**

---

## **📸 Deliverables**

- 4 screenshots (iOS and Android)
- Written report (Platform Differences, Implementation Approach, Code Quality)
- GitHub repository link in `GITHUB_LINK.txt`

---

## **👤 Author**

**Student:** Abdulbasit Dada  
**Course:** CPAN 213 – Cross-Platform Mobile Application Development  
**Instructor:** Horia Humaila  
**Date:** October 2025
