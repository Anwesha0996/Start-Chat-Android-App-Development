# Start Chat

<p align="center">
  <img src="screenshots/logo.png" alt="Start Chat Logo" width="140"/>
</p>

<p align="center">
  <b>Simple. Private. Instant Messaging.</b>
</p>

## Overview

Start Chat is a lightweight Android messaging app focused on privacy and simplicity.  
It allows users to chat instantly without requiring a phone number, email, or account.

The app is designed for users who want a fast, minimal, and private messaging experience.

## Features

- No phone number or account required
- Simple and minimal login screen
- Real-time chat using Firebase Realtime Database
- Auto-deleting messages for privacy
- Lightweight UI built with Jetpack Compose
- Fast and user-friendly interface

## App Flow

### 1. Splash Screen
- Displays the Start Chat logo
- Clean startup screen for branding
- Automatically navigates after 2 seconds

### 2. Login Screen
- Minimal design with a single button: **Go to Chat**
- No login or signup needed
- Instant access to chat

### 3. Chat Screen
- Real-time messaging
- Messages synced through Firebase
- Privacy-focused auto-delete behavior

## Tech Stack

- **Language:** Kotlin
- **UI Framework:** Jetpack Compose
- **Backend:** Firebase Realtime Database
- **Async Handling:** Kotlin Coroutines
- **IDE:** Android Studio

## Technical Implementation

This app follows a modern Android development approach:

- Built with Jetpack Compose
- Single-activity architecture
- Multiple `@Composable` screens
- State management using `remember`, `mutableStateOf`, and `LaunchedEffect`
- Firebase Realtime Database for cloud sync
- Auto-delete message behavior for privacy
- Asynchronous operations handled with Kotlin coroutines

## Firebase Integration

Firebase Realtime Database is used to store and synchronize chat messages instantly across devices.

- Messages are stored under the `messages` node
- `.push()` is used to generate unique keys
- `ChildEventListener` listens for new messages
- Chat updates appear live across emulators/devices

## Screenshots

### App Logo
![Logo](screenshots/logo.png)

### Splash Screen
![Splash Screen](screenshots/splash_screen.png)

### Login Screen
![Login Screen](screenshots/login_screen.png)

### Chat Screen
![Chat Screen](screenshots/chat_screen.png)

## Testing

The application was tested successfully on two Android emulators.

### Demo Flow
Splash Screen → Login Screen → Chat Screen → Firebase Realtime Sync

## Future Improvements

- Group chat support
- Media sharing
- Enhanced UI features
- User customization options

## Author

**Anwesha Ghosh**  
MSc Information and Communication Engineering  
TU Dresden / AAU Klagenfurt
