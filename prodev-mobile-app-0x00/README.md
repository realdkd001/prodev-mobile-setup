````markdown
# React Native Environment Setup using Expo Go

## Project Overview
This project documents my experience setting up a mobile development environment for React Native using Expo Go.  
As someone new to React Native, my goal was to successfully configure all necessary tools and test my first app on a physical device.

---

## Objective
The main objective of this task was to:
- Install and configure the required tools for mobile app development.
- Use Expo Go to test React Native applications directly on a mobile device.
- Document the entire setup process and note any challenges faced.

---

## System Details
- Operating System: Windows 11  
- IDE: Visual Studio Code (VS Code)  
- Node.js Version: LTS (checked using `node -v`)  
- Device Used for Testing: Android  
- Testing Tool: Expo Go

---

## Setup Process

### Step 1: Installing Required Tools
1. **Node.js (LTS)**  
   I downloaded and installed Node.js from the [official website](https://nodejs.org/).  
   After installation, I verified it using:
   ```bash
   node -v
   npm -v
````

Both commands returned version numbers, confirming successful installation.

2. **Visual Studio Code (VS Code)**
   I already had VS Code installed. It will be my main editor for writing and testing React Native code.

3. **Check OS Compatibility**
   My system runs on Windows 11, which supports all the necessary tools.

---

### Step 2: Installing Expo Go on My Mobile Device

1. I visited the [Expo Go official page](https://expo.dev/go).
2. Selected the option for Android, which redirected me to the Google Play Store.
3. Installed Expo Go on my phone.
4. Opened the app and created an Expo account (signed in successfully).

Expo Go allows me to preview React Native apps instantly on my phone without installing any emulators.

---

### Step 3: Creating My First React Native App

With everything installed, I opened my terminal and ran the following commands:

```bash
npm install -g expo-cli
```

Then I created a new project:

```bash
npx create-expo-app my-first-app
```

Navigated into the project folder:

```bash
cd my-first-app
```

Started the development server:

```bash
npx expo start
```

A QR code appeared in my terminal/browser window.
I scanned it using the Expo Go app on my phone, and after a short moment, my test app opened successfully.

---

## Understanding Expo Go vs Expo CLI

As a beginner, I initially thought Expo Go and Expo CLI were the same thing, but here’s what I learned:

| Tool     | Description                                                                                                    |
| -------- | -------------------------------------------------------------------------------------------------------------- |
| Expo CLI | A command-line tool that runs on my computer. It starts the project and provides a QR code to connect devices. |
| Expo Go  | A mobile app that runs on my phone. It loads and previews my React Native project instantly.                   |

This distinction helped me understand how both work together to simplify testing.

---

## Challenges Faced and Solutions

| Challenge                  | Cause                                                | Solution                                          |
| -------------------------- | ---------------------------------------------------- | ------------------------------------------------- |
| QR code not scanning       | My phone and laptop were on different Wi-Fi networks | Connected both devices to the same network        |
| Slow loading of the app    | Weak Wi-Fi connection                                | Restarted router and re-ran `npx expo start`      |
| Confusion about tool usage | New to React Native environment                      | Read Expo documentation and tested multiple times |

---

## Outcome

After completing the setup:

* I can now run and test React Native apps on my physical Android device.
* VS Code is connected and ready for development.
* I understand the difference between Expo CLI and Expo Go.
* I’m ready to start building my first real React Native project.

---

## Completion Details

* Task: Setting Up and Testing Mobile Development Environment
* Framework: Expo (React Native)
* Author: Daniel (Beginner React Native Developer)

---

## Reflection

This was my first experience setting up a mobile development environment.
At first, I was nervous about compatibility issues and thought I might need an emulator. However, Expo Go made the process smooth and beginner-friendly.
Seeing my first app appear on my phone felt very rewarding, and it motivated me to continue learning React Native.

---

## Summary

* Node.js and VS Code installed successfully
* Expo Go set up on Android device
* First React Native app created and tested
* Environment verified and working correctly

This marks the beginning of my journey into mobile app development with React Native.

```