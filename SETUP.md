# 📱 React Native (Expo) -- Windows + iPhone Setup Guide

This document explains exactly what to install and how to run the app on
an iPhone using Expo Go from a Windows machine.

------------------------------------------------------------------------

## 1. System Requirements

### Operating System

-   Windows 10 or Windows 11 (64-bit)

### iPhone

-   iOS 15 or newer
-   App Store access

------------------------------------------------------------------------

## 2. Required Software (Install in Order)

### 2.1 Node.js (Required)

Install Node.js LTS (18.x or 20.x):\
https://nodejs.org

Verify:

    node -v
    npm -v

Restart your terminal if these fail.

------------------------------------------------------------------------

### 2.2 Git (Required)

Install Git for Windows:\
https://git-scm.com/download/win

Verify:

    git --version

------------------------------------------------------------------------

### 2.3 Expo Go (Required on iPhone)

-   Open the App Store
-   Search for **Expo Go**
-   Install

------------------------------------------------------------------------

## 3. Project Setup

### 3.1 Clone the Repository

    git clone https://github.com/tadiday/hotspot.git
    cd hotspot

------------------------------------------------------------------------

### 3.2 Install Dependencies

    npm install

This step is mandatory.

------------------------------------------------------------------------

## 4. Running the App (Expo Go)

### 4.1 Start Expo

    npx expo start -c

------------------------------------------------------------------------

### 4.2 Enable Tunnel Mode (Important on Windows)

In the Expo terminal: - Press `s` - Select **Tunnel**

------------------------------------------------------------------------

### 4.3 Run on iPhone

1.  Open **Expo Go**
2.  Tap **Scan QR Code**
3.  Scan the QR shown in the terminal

Use Expo Go's scanner, not the Camera app.

------------------------------------------------------------------------

## 5. Common Issues

### QR Code Timeout

-   Use Tunnel mode
-   Disable VPNs
-   Ensure both devices have internet

### Unable to find expo

    npm install

### App failed to load

    npx expo start -c

------------------------------------------------------------------------

## 6. What You Do NOT Need

-   Xcode
-   macOS
-   USB cable
-   Apple Developer account
-   Docker
-   WSL

------------------------------------------------------------------------

## 7. Recommended Versions

  Tool      Version
  --------- --------------
  Node.js   18.x or 20.x
  iOS       15+
  Expo Go   Latest

------------------------------------------------------------------------

## 8. Workflow

Edit code → `npx expo start` → Scan QR → Live reload on iPhone
