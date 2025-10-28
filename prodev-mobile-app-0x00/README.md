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
- Document the setup process and note any challenges faced.
- Record the steps I followed for scaffolding the project.
- Share my observations from using the `npx expo reset-project` command.

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

### Step 3: Scaffolding the Project

To scaffold (create) my first React Native project using Expo, I followed these steps:

1. Opened my terminal and ran:

   ```bash
   npx create-expo-app app-example
   ```

2. Navigated into the newly created project folder:

   ```bash
   cd app-example
   ```

3. Installed dependencies (in case they didn’t auto-install):

   ```bash
   npm install
   ```

4. Started the project using the local CLI (as the global `expo-cli` is deprecated):

   ```bash
   npx expo start
   ```

This successfully created a new Expo project with a preconfigured folder structure containing:

* `App.js`
* `package.json`
* `node_modules/`
* `assets/`
* `app.json`

I was able to scan the generated QR code in **Expo Go**, and the default “Welcome to React Native” screen appeared on my phone.

---

### Step 4: Observations from the `npx expo reset-project` Command

After scaffolding the project, I ran the command:

```bash
npx expo reset-project
```

Here’s what I observed:

1. The command **resets the project to its default Expo template**, removing any extra configurations or files that might have been added.
2. It **cleans up node modules** and reinitializes dependencies to ensure the project starts in a stable state.
3. It helps fix issues such as:

   * Missing dependencies
   * Project corruption
   * Incorrect configurations after updates
4. After running it, I had to reinstall dependencies using:

   ```bash
   npm install
   ```
5. When I restarted with `npx expo start`, the app loaded as if it was newly created.

In summary, the `reset-project` command is helpful for beginners to restore their project if something breaks during setup.

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

| Challenge                                   | Cause                                                | Solution                                             |
| ------------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------- |
| QR code not scanning                        | My phone and laptop were on different Wi-Fi networks | Connected both devices to the same network           |
| Slow loading of the app                     | Weak Wi-Fi connection                                | Restarted router and re-ran `npx expo start`         |
| “Unable to find expo in this project” error | Missing local dependencies                           | Ran `npm install` in the project directory           |
| Confusion about tool usage                  | New to React Native environment                      | Read Expo documentation and practiced multiple times |

---

## Outcome

After completing the setup:

* I can now run and test React Native apps on my physical Android device.
* VS Code is configured and ready for development.
* I understand the difference between Expo CLI and Expo Go.
* I’m familiar with scaffolding and resetting a React Native project.
* I’m ready to start building my first real mobile application.

---

## Completion Details

* Task: Setting Up and Testing Mobile Development Environment
* Framework: Expo (React Native)
* Date Completed: October 2025
* Author: Daniel (Beginner React Native Developer)

---

## Reflection

This was my first experience setting up a mobile development environment.
At first, I was nervous about compatibility issues and thought I might need an emulator. However, Expo Go made the process smooth and beginner-friendly.
Running my first app successfully on my phone felt rewarding, and it motivated me to continue learning React Native.

---

## Summary

* Node.js and VS Code installed successfully
* Expo Go set up on Android device
* Project scaffolded using `npx create-expo-app`
* Verified the project with `npx expo start`
* Tested and reset successfully using `npx expo reset-project`
* Environment working correctly

This marks the beginning of my journey into mobile app development with React Native.

```