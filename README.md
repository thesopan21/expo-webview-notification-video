# React Native App 👋

This is an [Expo](https://expo.dev) project created with [`create-expo-app`](https://www.npmjs.com/package/create-expo-app).

---

## React Native (Expo) Assignment: WebView + Notifications + Video Player

### Objective

Build an Expo React Native app that:

1. Embeds a website using **WebView**.
2. Triggers **local notifications** based on user interaction.
3. Plays an **HLS video stream** on a separate page.

---

### Requirements

#### 1. WebView Page

- Embed a website inside the app.  
- Add two buttons under the WebView that trigger different local notifications.

#### 2. Notifications

- Implement at least **two distinct notification messages**.  
- Notifications should trigger with a **delay of 2–5 seconds**.

#### 3. Video Player Page

- Add a new page that plays an HLS video using Expo’s video player.  
- Use this test URL:  

## ⚙️ Implementation Choices

### 1. WebView

Used react-native-webview to embed a website inside the app.
Chosen for its simplicity and support for both iOS and Android.
Added two buttons below the WebView to trigger notifications, keeping UI consistent and user-friendly.

### 2. Notifications

Used Expo Notifications API for scheduling local notifications.
Chose delayed notifications (2–5 seconds) to demonstrate async scheduling.
Implemented two distinct messages to showcase flexibility.

### 3. Video Player

Used expo-av's Video component to play the HLS stream.
Chosen because Expo supports HLS out-of-the-box, with controls like play, pause, and fullscreen.
Tested with the sample stream:
<https://test-streams.mux.dev/x36xhzz/x36xhzz.m3u8>

### 4. Navigation

Used @react-navigation/native with a Stack Navigator for page-to-page navigation.
This allows smooth switching between WebView + Notifications and Video Player screens.

### 5. Project Structure

app/ → contains screens and navigation setup.
components/ → reusable UI components.
assets/ → images, icons, and screenshots.
